# Comparing `tmp/cuenca-0.9.4.dev0.tar.gz` & `tmp/cuenca-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuenca-0.9.4.dev0.tar", last modified: Tue May 10 23:27:35 2022, max compression
+gzip compressed data, was "cuenca-1.0.0.tar", last modified: Mon Apr  1 23:57:56 2024, max compression
```

## Comparing `cuenca-0.9.4.dev0.tar` & `cuenca-1.0.0.tar`

### file list

```diff
@@ -1,103 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 23:27:35.871389 cuenca-0.9.4.dev0/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4596 2022-05-10 23:27:35.871389 cuenca-0.9.4.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4034 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 23:27:35.859388 cuenca-0.9.4.dev0/cuenca/
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 23:27:35.863388 cuenca-0.9.4.dev0/cuenca/http/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4149 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/http/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 23:27:35.863388 cuenca-0.9.4.dev0/cuenca/resources/
--rw-r--r--   0 runner    (1001) docker     (121)     2516 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/api_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/arpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/balance_entries.py
--rw-r--r--   0 runner    (1001) docker     (121)     5932 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/bill_payments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/card_activations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/card_transactions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/card_validations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2915 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/cards.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/commissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/curp_validations.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/deposits.py
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/file_batches.py
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/files.py
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/identities.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/identity_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/kyc_verifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/limited_wallets.py
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/login_tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/savings.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/service_providers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/sessions.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/statements.py
--rw-r--r--   0 runner    (1001) docker     (121)     3156 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/transfers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/user_credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/user_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/user_logins.py
--rw-r--r--   0 runner    (1001) docker     (121)     3457 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/users.py
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/verifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/wallet_transactions.py
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/resources/whatsapp_transfers.py
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/cuenca/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 23:27:35.859388 cuenca-0.9.4.dev0/cuenca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4596 2022-05-10 23:27:35.000000 cuenca-0.9.4.dev0/cuenca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-05-10 23:27:35.000000 cuenca-0.9.4.dev0/cuenca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-10 23:27:35.000000 cuenca-0.9.4.dev0/cuenca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-05-10 23:27:35.000000 cuenca-0.9.4.dev0/cuenca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-10 23:27:35.000000 cuenca-0.9.4.dev0/cuenca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-05-10 23:27:35.871389 cuenca-0.9.4.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 23:27:35.867389 cuenca-0.9.4.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 23:27:35.867389 cuenca-0.9.4.dev0/tests/http/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/http/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2594 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/http/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 23:27:35.871389 cuenca-0.9.4.dev0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2281 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_arpc.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_balance_entries.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_bill_payments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_card_activations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_card_transactions.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_card_validations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_commissions.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_curp_validations.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_deposits.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_file_batches.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_files.py
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_identities.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_identity_events.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_kyc_verifications.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_limited_wallets.py
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_login_tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_savings.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_service_providers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_statements.py
--rw-r--r--   0 runner    (1001) docker     (121)     4157 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_transfers.py
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_user_credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_user_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_user_logins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_users.py
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_verifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     3945 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_wallet_transactions.py
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/resources/test_whatsapp_transfers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/test_cuenca.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-05-10 23:27:27.000000 cuenca-0.9.4.dev0/tests/test_jwt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.632049 cuenca-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 23:57:50.000000 cuenca-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-01 23:57:56.632049 cuenca-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-01 23:57:50.000000 cuenca-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.612049 cuenca-1.0.0/cuenca/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.612049 cuenca-1.0.0/cuenca/http/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.620050 cuenca-1.0.0/cuenca/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/arpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/balance_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/bill_payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/card_activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/card_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/card_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/cash_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/clabes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/commissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/curp_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/deposits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/file_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/identities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/identity_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/kyc_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/kyc_verifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/limited_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/login_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/questionnaires.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/savings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/service_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/user_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/user_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/user_lists_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/user_logins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/verifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/wallet_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/whatsapp_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.632049 cuenca-1.0.0/cuenca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-01 23:57:56.000000 cuenca-1.0.0/cuenca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-01 23:57:56.000000 cuenca-1.0.0/cuenca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 23:57:56.000000 cuenca-1.0.0/cuenca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 23:57:56.000000 cuenca-1.0.0/cuenca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 23:57:56.000000 cuenca-1.0.0/cuenca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-01 23:57:56.632049 cuenca-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-01 23:57:50.000000 cuenca-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.624050 cuenca-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.624050 cuenca-1.0.0/tests/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/http/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/http/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.632049 cuenca-1.0.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_arpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_balance_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_bill_payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_card_activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_card_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_card_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_cash_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_clabes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_commissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_curp_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_deposits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_file_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_identities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_identity_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_kyc_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_kyc_verifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_limited_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_login_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_questionnaires.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_savings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_service_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_user_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_user_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_user_lists_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_user_logins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_verifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_wallet_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_whatsapp_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/test_cuenca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/test_jwt.py
```

### Comparing `cuenca-0.9.4.dev0/LICENSE` & `cuenca-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/PKG-INFO` & `cuenca-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cuenca
-Version: 0.9.4.dev0
+Version: 1.0.0
 Summary: Cuenca API Client
 Home-page: https://github.com/cuenca-mx/cuenca-python
 Author: Cuenca
 Author-email: dev@cuenca.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests<28,>=2.24
+Requires-Dist: dataclasses>=0.7; python_version < "3.8"
+Requires-Dist: cuenca-validations<0.12.0,>=0.11.3
 
 # Cuenca – Python client library
 
 [![test](https://github.com/cuenca-mx/cuenca-python/workflows/test/badge.svg)](https://github.com/cuenca-mx/cuenca-python/actions?query=workflow%3Atest)
 [![codecov](https://codecov.io/gh/cuenca-mx/cuenca-python/branch/main/graph/badge.svg)](https://codecov.io/gh/cuenca-mx/cuenca-python)
 [![PyPI](https://img.shields.io/pypi/v/cuenca.svg)](https://pypi.org/project/cuenca/)
```

### Comparing `cuenca-0.9.4.dev0/README.md` & `cuenca-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/cuenca/__init__.py` & `cuenca-1.0.0/cuenca/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,33 +5,39 @@
     'Arpc',
     'BalanceEntry',
     'BillPayment',
     'Card',
     'CardActivation',
     'CardTransaction',
     'CardValidation',
+    'CashReference',
+    'Clabe',
     'CurpValidation',
     'Commission',
     'Deposit',
     'Endpoint',
     'File',
     'FileBatch',
     'Identity',
     'IdentityEvent',
+    'KYCValidation',
     'KYCVerification',
     'LimitedWallet',
     'LoginToken',
+    'Platform',
+    'Questionnaires',
     'Saving',
     'ServiceProvider',
     'Session',
     'Statement',
     'Transfer',
     'User',
     'UserCredential',
     'UserEvent',
+    'UserListsValidation',
     'UserLogin',
     'Verification',
     'WalletTransaction',
     'Webhook',
     'WhatsappTransfer',
     'configure',
     'get_balance',
@@ -46,33 +52,39 @@
     Arpc,
     BalanceEntry,
     BillPayment,
     Card,
     CardActivation,
     CardTransaction,
     CardValidation,
+    CashReference,
+    Clabe,
     Commission,
     CurpValidation,
     Deposit,
     Endpoint,
     File,
     FileBatch,
     Identity,
     IdentityEvent,
+    KYCValidation,
     KYCVerification,
     LimitedWallet,
     LoginToken,
+    Platform,
+    Questionnaires,
     Saving,
     ServiceProvider,
     Session,
     Statement,
     Transfer,
     User,
     UserCredential,
     UserEvent,
+    UserListsValidation,
     UserLogin,
     Verification,
     WalletTransaction,
     Webhook,
     WhatsappTransfer,
 )
 from .version import __version__
```

### Comparing `cuenca-0.9.4.dev0/cuenca/exc.py` & `cuenca-1.0.0/cuenca/exc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 
 from cuenca_validations.typing import DictStrAny
 
 
 class CuencaException(Exception):
-    ...
+    """Base Exception Class"""
 
 
 class MalformedJwtToken(CuencaException):
     """An invalid JWT token was obtained during authentication"""
 
 
 class NoResultFound(CuencaException):
```

### Comparing `cuenca-0.9.4.dev0/cuenca/http/client.py` & `cuenca-1.0.0/cuenca/http/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import datetime as dt
 import json
 import os
 from typing import Optional, Tuple
 from urllib.parse import urljoin
 
 import requests
 from cuenca_validations.errors import ERROR_CODES
+from cuenca_validations.types import JSONEncoder
 from cuenca_validations.typing import (
     ClientRequestParams,
     DictStrAny,
     OptionalDict,
 )
 from requests import Response
 
@@ -20,26 +20,23 @@
 API_HOST = 'api.cuenca.com'
 SANDBOX_HOST = 'sandbox.cuenca.com'
 
 
 class Session:
 
     host: str = API_HOST
+    headers: DictStrAny = {}
     basic_auth: Tuple[str, str]
     jwt_token: Optional[Jwt] = None
-    session: requests.Session
 
     def __init__(self):
-        self.session = requests.Session()
-        self.session.headers.update(
-            {
-                'X-Cuenca-Api-Version': API_VERSION,
-                'User-Agent': f'cuenca-python/{CLIENT_VERSION}',
-            }
-        )
+        self.headers = {
+            'X-Cuenca-Api-Version': API_VERSION,
+            'User-Agent': f'cuenca-python/{CLIENT_VERSION}',
+        }
 
         # basic auth
         api_key = os.getenv('CUENCA_API_KEY', '')
         api_secret = os.getenv('CUENCA_API_SECRET', '')
         self.basic_auth = (api_key, api_secret)
 
     @property
@@ -71,18 +68,18 @@
             api_secret or self.basic_auth[1],
         )
 
         if use_jwt:
             self.jwt_token = Jwt.create(self)
 
         if login_token:
-            self.session.headers['X-Cuenca-LoginToken'] = login_token
+            self.headers['X-Cuenca-LoginToken'] = login_token
 
         if session_token:
-            self.session.headers['X-Cuenca-SessionId'] = session_token
+            self.headers['X-Cuenca-SessionId'] = session_token
 
     def get(
         self, endpoint: str, params: ClientRequestParams = None
     ) -> DictStrAny:
         return self._request_json('get', endpoint, params=params)
 
     def post(self, endpoint: str, data: DictStrAny, **kwargs) -> DictStrAny:
@@ -101,32 +98,30 @@
         self,
         method: str,
         endpoint: str,
         params: ClientRequestParams = None,
         data: OptionalDict = None,
         **kwargs,
     ) -> bytes:
-        if self.jwt_token:
-            if self.jwt_token.is_expired:
-                self.jwt_token = Jwt.create(self)
-            self.session.headers['X-Cuenca-Token'] = self.jwt_token.token
-
-        if data is not None:
-            for key, value in data.items():
-                if isinstance(value, dt.date):
-                    data[key] = value.isoformat()
-
-        resp = self.session.request(
-            method=method,
-            url='https://' + self.host + urljoin('/', endpoint),
-            auth=self.auth,
-            json=data,
-            params=params,
-            **kwargs,
-        )
+        resp = None
+        with requests.Session() as session:
+            session.headers = self.headers  # type: ignore
+            if self.jwt_token:
+                if self.jwt_token.is_expired:
+                    self.jwt_token = Jwt.create(self)
+                self.headers['X-Cuenca-Token'] = self.jwt_token.token
+                session.headers = self.headers  # type: ignore
+            resp = session.request(  # type: ignore
+                method=method,
+                url='https://' + self.host + urljoin('/', endpoint),
+                auth=self.auth,
+                json=json.loads(JSONEncoder().encode(data)),
+                params=params,
+                **kwargs,
+            )
         self._check_response(resp)
         return resp.content
 
     @staticmethod
     def _check_response(response: Response):
         if response.ok:
             return
```

### Comparing `cuenca-0.9.4.dev0/cuenca/jwt.py` & `cuenca-1.0.0/cuenca/jwt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import base64
 import binascii
 import datetime as dt
 import json
-from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
+from pydantic import BaseModel
+
 from .exc import MalformedJwtToken
 
 if TYPE_CHECKING:
     from .http import Session
 
 
-@dataclass
-class Jwt:
+class Jwt(BaseModel):
     expires_at: dt.datetime
     token: str
 
     @property
     def is_expired(self) -> bool:
         return self.expires_at - dt.datetime.utcnow() <= dt.timedelta(
             minutes=5
@@ -38,11 +38,11 @@
         # Expiration timestamp can be found in the `exp` key in the payload
         exp_timestamp = payload['exp']
         return dt.datetime.utcfromtimestamp(exp_timestamp)
 
     @classmethod
     def create(cls, session: 'Session') -> 'Jwt':
         session.jwt_token = None
-        session.session.headers.pop('X-Cuenca-Token', None)
+        session.headers.pop('X-Cuenca-Token', None)
         token = session.post('/token', dict())['token']
         expires_at = Jwt.get_expiration_date(token)
-        return cls(expires_at, token)
+        return cls(expires_at=expires_at, token=token)
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/__init__.py` & `cuenca-1.0.0/cuenca/resources/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,33 +4,39 @@
     'Arpc',
     'BalanceEntry',
     'BillPayment',
     'Card',
     'CardActivation',
     'CardTransaction',
     'CardValidation',
+    'CashReference',
+    'Clabe',
     'Commission',
     'CurpValidation',
     'Deposit',
     'Endpoint',
     'File',
     'FileBatch',
     'Identity',
     'IdentityEvent',
+    'KYCValidation',
     'KYCVerification',
     'LimitedWallet',
     'LoginToken',
+    'Platform',
+    'Questionnaires',
     'Saving',
     'ServiceProvider',
     'Session',
     'Statement',
     'Transfer',
     'User',
     'UserEvent',
     'UserLogin',
+    'UserListsValidation',
     'Verification',
     'WalletTransaction',
     'Webhook',
     'WhatsappTransfer',
 ]
 
 from .accounts import Account
@@ -38,33 +44,39 @@
 from .arpc import Arpc
 from .balance_entries import BalanceEntry
 from .bill_payments import BillPayment
 from .card_activations import CardActivation
 from .card_transactions import CardTransaction
 from .card_validations import CardValidation
 from .cards import Card
+from .cash_references import CashReference
+from .clabes import Clabe
 from .commissions import Commission
 from .curp_validations import CurpValidation
 from .deposits import Deposit
 from .endpoints import Endpoint
 from .file_batches import FileBatch
 from .files import File
 from .identities import Identity
 from .identity_events import IdentityEvent
+from .kyc_validations import KYCValidation
 from .kyc_verifications import KYCVerification
 from .limited_wallets import LimitedWallet
 from .login_tokens import LoginToken
+from .platforms import Platform
+from .questionnaires import Questionnaires
 from .resources import RESOURCES
 from .savings import Saving
 from .service_providers import ServiceProvider
 from .sessions import Session
 from .statements import Statement
 from .transfers import Transfer
 from .user_credentials import UserCredential
 from .user_events import UserEvent
+from .user_lists_validation import UserListsValidation
 from .user_logins import UserLogin
 from .users import User
 from .verifications import Verification
 from .wallet_transactions import WalletTransaction
 from .webhooks import Webhook
 from .whatsapp_transfers import WhatsappTransfer
 
@@ -75,34 +87,40 @@
     Arpc,
     BalanceEntry,
     BillPayment,
     Card,
     CardActivation,
     CardTransaction,
     CardValidation,
+    CashReference,
+    Clabe,
     CurpValidation,
     Commission,
     Deposit,
     Endpoint,
     File,
     FileBatch,
     Identity,
     IdentityEvent,
+    KYCValidation,
     KYCVerification,
     LimitedWallet,
     LoginToken,
+    Questionnaires,
     Saving,
     Session,
     ServiceProvider,
     Statement,
     Transfer,
     User,
     UserCredential,
     UserEvent,
+    UserListsValidation,
     UserLogin,
     Verification,
     WalletTransaction,
     WhatsappTransfer,
     Webhook,
+    Platform,
 ]
 for resource_cls in resource_classes:
     RESOURCES[resource_cls._resource] = resource_cls  # type: ignore
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/api_keys.py` & `cuenca-1.0.0/cuenca/resources/api_keys.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 import datetime as dt
 from typing import ClassVar, Optional, cast
 
 from cuenca_validations.types import ApiKeyQuery, ApiKeyUpdateRequest
-from pydantic.dataclasses import dataclass
 
 from ..http import Session, session as global_session
 from .base import Creatable, Queryable, Retrievable, Updateable
 
 
-@dataclass
 class ApiKey(Creatable, Queryable, Retrievable, Updateable):
     _resource: ClassVar = 'api_keys'
     _query_params: ClassVar = ApiKeyQuery
 
     secret: str
     deactivated_at: Optional[dt.datetime]
     user_id: Optional[str]
 
+    class Config:
+        schema_extra = {
+            'example': {
+                'id': 'AKNEUInh69SuKXXmK95sROwQ',
+                'updated_at': '2021-08-24T14:15:22Z',
+                'created_at': '2021-08-24T14:15:22Z',
+                'secret': 'super-secret-random-string',
+                'deactivated_at': None,
+                'user_id': 'USWqY5cvkISJOxHyEKjAKf8w',
+            }
+        }
+
     @property
     def active(self) -> bool:
         return (
             self.deactivated_at is None
             or self.deactivated_at > dt.datetime.utcnow()
         )
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/arpc.py` & `cuenca-1.0.0/cuenca/resources/arpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import datetime as dt
 from typing import ClassVar, Optional, cast
 
 from cuenca_validations.types.requests import ARPCRequest
-from pydantic.dataclasses import dataclass
 
 from ..http import Session, session as global_session
 from .base import Creatable
 
 
-@dataclass
 class Arpc(Creatable):
     """
     An ARPC (Authorisation Response Cryptogram) is generated by the issuer
     to authorize EMV transactions (Chip, Contactless)
 
     The point of sales terminal or ATM generate an ARQC (Authorization Request
     Cryptogram) to obtain authorization for transactions.
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/balance_entries.py` & `cuenca-1.0.0/cuenca/resources/balance_entries.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from typing import ClassVar, TypeVar, cast
 
 from cuenca_validations.types import BalanceEntryQuery, EntryType
-from pydantic.dataclasses import dataclass
 
 from .accounts import Account
 from .base import Queryable, Retrievable, Transaction
 from .cards import Card
 from .resources import retrieve_uri
 from .service_providers import ServiceProvider
 
 FundingInstrument = TypeVar(
     'FundingInstrument', Account, ServiceProvider, Card
 )
 
 
-@dataclass
 class BalanceEntry(Retrievable, Queryable):
     _resource: ClassVar = 'balance_entries'
     _query_params: ClassVar = BalanceEntryQuery
 
     amount: int  # negative in the case of a debit
     descriptor: str
     name: str
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/base.py` & `cuenca-1.0.0/cuenca/resources/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 import base64
 import datetime as dt
 import json
-from dataclasses import asdict, dataclass, fields
 from io import BytesIO
 from typing import ClassVar, Dict, Generator, Optional, Union
 from urllib.parse import urlencode
 
 from cuenca_validations.types import (
     FileFormat,
     QueryParams,
     SantizedDict,
     TransactionQuery,
     TransactionStatus,
 )
+from pydantic import BaseModel
 
 from ..exc import MultipleResultsFound, NoResultFound
 from ..http import Session, session as global_session
 
 
-@dataclass
-class Resource:
+class Resource(BaseModel):
     _resource: ClassVar[str]
 
     id: str
 
-    # purely for MyPy
-    def __init__(self, **_):  # pragma: no cover
-        ...
-
     @classmethod
     def _from_dict(cls, obj_dict: Dict[str, Union[str, int]]) -> 'Resource':
         cls._filter_excess_fields(obj_dict)
         return cls(**obj_dict)
 
     @classmethod
     def _filter_excess_fields(cls, obj_dict):
         """
         dataclasses don't allow __init__ to be called with excess fields. This
         method allows the API to add fields in the response body without
         breaking the client
         """
-        excess = set(obj_dict.keys()) - {f.name for f in fields(cls)}
+        excess = set(obj_dict.keys()) - set(
+            cls.schema().get("properties").keys()
+        )
         for f in excess:
             del obj_dict[f]
 
     def to_dict(self):
-        return asdict(self, dict_factory=SantizedDict)
+        return SantizedDict(self.dict())
 
 
 class Retrievable(Resource):
     @classmethod
     def retrieve(
         cls, id: str, *, session: Session = global_session
     ) -> Resource:
@@ -65,28 +62,26 @@
 class Creatable(Resource):
     @classmethod
     def _create(cls, *, session: Session = global_session, **data) -> Resource:
         resp = session.post(cls._resource, data)
         return cls._from_dict(resp)
 
 
-@dataclass
 class Updateable(Resource):
 
     updated_at: dt.datetime
 
     @classmethod
     def _update(
         cls, id: str, *, session: Session = global_session, **data
     ) -> Resource:
         resp = session.patch(f'/{cls._resource}/{id}', data)
         return cls._from_dict(resp)
 
 
-@dataclass
 class Deactivable(Resource):
     deactivated_at: Optional[dt.datetime]
 
     @classmethod
     def deactivate(
         cls, id: str, *, session: Session = global_session, **data
     ) -> Resource:
@@ -94,41 +89,39 @@
         return cls._from_dict(resp)
 
     @property
     def is_active(self):
         return not self.deactivated_at
 
 
-@dataclass
 class Downloadable(Resource):
     @classmethod
     def download(
         cls,
-        instance,
-        file_format: FileFormat,
+        id: str,
+        file_format: FileFormat = FileFormat.any,
         *,
         session: Session = global_session,
     ) -> BytesIO:
         resp = session.request(
             'get',
-            f'/{cls._resource}/{instance.id}',
+            f'/{cls._resource}/{id}',
             headers=dict(Accept=file_format.value),
         )
         return BytesIO(resp)
 
     @property
     def pdf(self) -> bytes:
-        return self.download(self, file_format=FileFormat.pdf).read()
+        return self.download(self.id, file_format=FileFormat.pdf).read()
 
     @property
     def xml(self) -> bytes:
-        return self.download(self, file_format=FileFormat.xml).read()
+        return self.download(self.id, file_format=FileFormat.xml).read()
 
 
-@dataclass
 class Uploadable(Resource):
     @classmethod
     def _upload(
         cls,
         file: bytes,
         user_id: str,
         *,
@@ -144,15 +137,14 @@
                 user_id=(None, user_id),
                 **{k: (None, v) for k, v in data.items()},
             ),
         )
         return cls._from_dict(json.loads(resp))
 
 
-@dataclass
 class Queryable(Resource):
     _query_params: ClassVar = QueryParams
 
     created_at: dt.datetime
 
     @classmethod
     def one(
@@ -199,25 +191,23 @@
         next_page_uri = f'{cls._resource}?{urlencode(q.dict())}'
         while next_page_uri:
             page = session.get(next_page_uri)
             yield from (cls._from_dict(item) for item in page['items'])
             next_page_uri = page['next_page_uri']
 
 
-@dataclass
 class Transaction(Retrievable, Queryable):
     _query_params: ClassVar = TransactionQuery
 
     user_id: str
     amount: int  # in centavos
     status: TransactionStatus
     descriptor: str  # how it appears for the customer
 
 
-@dataclass
 class Wallet(Creatable, Deactivable, Retrievable, Queryable):
     user_id: str
     balance: int
 
     @property
     def wallet_uri(self):
         return f'/{self._resource}/{self.id}'
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/bill_payments.py` & `cuenca-1.0.0/cuenca/resources/bill_payments.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from typing import ClassVar, cast
 
 from cuenca_validations.types import BillPaymentQuery
-from pydantic.dataclasses import dataclass
 
 from .base import Transaction
 from .resources import retrieve_uri
 from .service_providers import ServiceProvider
 
 
-@dataclass
 class BillPayment(Transaction):
     _resource: ClassVar = 'bill_payments'
     _query_params: ClassVar = BillPaymentQuery
 
     account_number: str
     provider_uri: str
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/card_activations.py` & `cuenca-1.0.0/cuenca/resources/card_activations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import datetime as dt
-from dataclasses import dataclass
 from typing import ClassVar, Optional, cast
 
 from cuenca_validations.types.requests import CardActivationRequest
 
 from ..http import Session, session as global_session
 from .base import Creatable
 from .cards import Card
 from .resources import retrieve_uri
 
 
-@dataclass
 class CardActivation(Creatable):
     _resource: ClassVar = 'card_activations'
 
     created_at: dt.datetime
     user_id: str
     ip_address: str
     card_uri: Optional[str]
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/card_transactions.py` & `cuenca-1.0.0/cuenca/resources/card_transactions.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 from cuenca_validations.types import (
     CardErrorType,
     CardNetwork,
     CardTransactionQuery,
     CardTransactionType,
     CardType,
 )
-from pydantic.dataclasses import dataclass
 
 from .base import Transaction
 from .cards import Card
 from .resources import retrieve_uri, retrieve_uris
 
 
-@dataclass
 class CardTransaction(Transaction):
     _resource: ClassVar = 'card_transactions'
     _query_params: ClassVar = CardTransactionQuery
 
     type: CardTransactionType
     network: CardNetwork
     related_card_transaction_uris: List[str]
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/card_validations.py` & `cuenca-1.0.0/cuenca/resources/card_validations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import datetime as dt
 from typing import ClassVar, Optional, cast
 
 from cuenca_validations.types import CardStatus, CardType
 from cuenca_validations.types.requests import CardValidationRequest
-from pydantic.dataclasses import dataclass
 
 from ..http import Session, session as global_session
 from .base import Creatable
 from .cards import Card
 from .resources import retrieve_uri
 
 
-@dataclass
 class CardValidation(Creatable):
     _resource: ClassVar = 'card_validations'
 
     created_at: dt.datetime
     card_uri: str
     user_id: str
     card_status: CardStatus
@@ -23,14 +21,15 @@
     is_valid_cvv: Optional[bool]
     is_valid_cvv2: Optional[bool]
     is_valid_icvv: Optional[bool]
     is_valid_pin_block: Optional[bool]
     is_valid_exp_date: Optional[bool]
     is_pin_attempts_exceeded: bool
     is_expired: bool
+    platform_id: Optional[str] = None
 
     @classmethod
     def create(
         cls,
         number: str,
         cvv: Optional[str] = None,
         cvv2: Optional[str] = None,
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/cards.py` & `cuenca-1.0.0/cuenca/resources/cards.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,46 @@
+import datetime as dt
 from typing import ClassVar, Optional, cast
 
 from cuenca_validations.types import (
     CardFundingType,
     CardIssuer,
     CardStatus,
     CardType,
 )
 from cuenca_validations.types.queries import CardQuery
 from cuenca_validations.types.requests import CardRequest, CardUpdateRequest
-from pydantic.dataclasses import dataclass
 
 from cuenca.resources.base import Creatable, Queryable, Retrievable, Updateable
 
 from ..http import Session, session as global_session
 
 MAX_PIN_ATTEMPTS = 3
 
 
-@dataclass
 class Card(Retrievable, Queryable, Creatable, Updateable):
     _resource: ClassVar = 'cards'
     _query_params: ClassVar = CardQuery
 
     user_id: Optional[str]
     number: str
     exp_month: int
     exp_year: int
     cvv2: str
     pin: Optional[str]
     type: CardType
     status: CardStatus
     issuer: CardIssuer
     funding_type: CardFundingType
+    dcvv: Optional[str] = None
+    dcvv_expires_at: Optional[dt.datetime] = None
     pin_attempts_failed: Optional[int] = None
+    platform_id: Optional[str] = None
+    card_holder_user_id: Optional[str] = None
+    is_dynamic_cvv: bool = False
 
     @property
     def last_4_digits(self):
         return self.number[-4:]
 
     @property
     def bin(self):
@@ -52,52 +56,60 @@
 
     @classmethod
     def create(
         cls,
         issuer: CardIssuer,
         funding_type: CardFundingType,
         user_id: str = 'me',
+        card_holder_user_id: Optional[str] = None,
+        is_dynamic_cvv: bool = False,
         *,
         session: Session = global_session,
     ) -> 'Card':
         """
         Assigns user_id and ledger_account_id to a existing virtual card
 
-        :param user_id: associated user id
+        :param user_id: associated user id (Owner of card)
         :param funding_type: debit or credit
         :param issuer:
+        :param card_holder_user_id: Holder user of card, not is the owner
         :return: New assigned card
         """
         req = CardRequest(
             user_id=user_id,
             issuer=issuer,
             funding_type=funding_type,
+            card_holder_user_id=card_holder_user_id,
+            is_dynamic_cvv=is_dynamic_cvv,
         )
         return cast('Card', cls._create(session=session, **req.dict()))
 
     @classmethod
     def update(
         cls,
         card_id: str,
         status: Optional[CardStatus] = None,
         pin_block: Optional[str] = None,
+        is_dynamic_cvv: bool = False,
         *,
         session: Session = global_session,
     ) -> 'Card':
         """
         Updates card properties that are not sensitive or fixed data. It allows
         reconfigure properties like status, and manufacturer.
 
         :param card_id: existing card_id
         :param status:
         :param pin_block
         :param session:
         :return: Updated card object
         """
-        req = CardUpdateRequest(status=status, pin_block=pin_block)
+        req = CardUpdateRequest(
+            status=status, pin_block=pin_block, is_dynamic_cvv=is_dynamic_cvv
+        )
         resp = cls._update(card_id, session=session, **req.dict())
         return cast('Card', resp)
 
     @classmethod
     def deactivate(
         cls, card_id: str, *, session: Session = global_session
     ) -> 'Card':
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/commissions.py` & `cuenca-1.0.0/cuenca/resources/commissions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from typing import ClassVar, cast
 
 from cuenca_validations.types import CommissionType, EntryType
-from pydantic.dataclasses import dataclass
 
 from .base import Transaction
 from .resources import retrieve_uri
 
 mapper = {CommissionType.cash_deposit: EntryType.credit}
 
 
-@dataclass
 class Commission(Transaction):
     _resource: ClassVar = 'commissions'
 
     type: CommissionType
     related_transaction_uri: str
 
     @property  # type: ignore
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/deposits.py` & `cuenca-1.0.0/cuenca/resources/deposits.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from typing import ClassVar, Optional, cast
 
 from cuenca_validations.types import DepositNetwork, DepositQuery
-from pydantic.dataclasses import dataclass
 
 from .accounts import Account
 from .base import Transaction
 from .resources import retrieve_uri
 
 
-@dataclass
 class Deposit(Transaction):
     _resource: ClassVar = 'deposits'
     _query_params: ClassVar = DepositQuery
 
     network: DepositNetwork
     source_uri: str
     tracking_key: Optional[str]  # clave rastreo if network is SPEI
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/endpoints.py` & `cuenca-1.0.0/cuenca/resources/endpoints.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,65 +2,99 @@
 
 from cuenca_validations.types.enums import WebhookEvent
 from cuenca_validations.types.requests import (
     EndpointRequest,
     EndpointUpdateRequest,
 )
 from pydantic import HttpUrl
-from pydantic.dataclasses import dataclass
 
 from ..http import Session, session as global_session
 from .base import Creatable, Deactivable, Queryable, Retrievable, Updateable
 
 
-@dataclass()
 class Endpoint(Creatable, Deactivable, Retrievable, Queryable, Updateable):
     _resource: ClassVar = 'endpoints'
 
     url: HttpUrl
     secret: str
     is_enable: bool
     events: List[WebhookEvent]
 
+    class Config:
+        fields = {
+            'url': {'description': 'HTTPS url to send webhooks'},
+            'secret': {
+                'description': 'token to verify the webhook is sent by Cuenca '
+                'using HMAC algorithm'
+            },
+            'is_enable': {
+                'description': 'Allows user to turn-off the endpoint '
+                'without the need of deleting it'
+            },
+            'events': {
+                'description': 'list of enabled events. If None, '
+                'all events will be enabled for this Endpoint'
+            },
+        }
+        schema_extra = {
+            'example': {
+                '_id': 'ENxxne2Z5VSTKZm_w8Hzffcw',
+                'platform_id': 'PTZoPrrPT6Ts-9myamq5h1bA',
+                'created_at': '2022-06-29T22:00:00Z',
+                'updated_at': '2022-06-29T22:00:00Z',
+                'secret': '1234',
+                'url': 'https://webhook.site/714ed1d8',
+                'events': [
+                    'transaction.create',
+                    'transaction.update',
+                    'user.create',
+                    'user.update',
+                    'user.delete',
+                ],
+                'is_enable': True,
+            }
+        }
+
     @classmethod
     def create(
         cls,
         url: HttpUrl,
         events: Optional[List[WebhookEvent]] = None,
         *,
         session: Session = global_session,
     ) -> 'Endpoint':
         """
         Creates and Endpoint, allowing to recieve Webhooks with the specified
         events.
-
         :param url: HTTPS url to send webhooks
         :param events: list of enabled events. If None, all events will be
             enabled for this Endpoint
         :param session:
         :return: New active endpoint
         """
         req = EndpointRequest(url=url, events=events)
         return cast('Endpoint', cls._create(session=session, **req.dict()))
 
     @classmethod
     def update(
         cls,
         endpoint_id: str,
         url: Optional[HttpUrl] = None,
+        events: Optional[List[WebhookEvent]] = None,
         is_enable: Optional[bool] = None,
         *,
         session: Session = global_session,
     ) -> 'Endpoint':
         """
         Updates endpoint properties. It allows reconfigure properties
         like url and is_active.
-
         :param endpoint_id: existing endpoint_id
         :param url
         :param is_enable
         :param session
         :return: Updated endpoint object
         """
-        req = EndpointUpdateRequest(url=url, is_enable=is_enable)
+        req = EndpointUpdateRequest(
+            url=url, is_enable=is_enable, events=events
+        )
         resp = cls._update(endpoint_id, session=session, **req.dict())
         return cast('Endpoint', resp)
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/file_batches.py` & `cuenca-1.0.0/cuenca/resources/file_batches.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from typing import ClassVar, Dict, List, cast
 
 from cuenca_validations.types import BatchFileMetadata, FileBatchUploadRequest
-from pydantic.dataclasses import dataclass
 
 from ..http import Session, session as global_session
 from .base import Creatable, Queryable
 
 
-@dataclass
 class FileBatch(Creatable, Queryable):
     _resource: ClassVar = 'file_batches'
 
     received_files: List[BatchFileMetadata]
     uploaded_files: List[BatchFileMetadata]
     user_id: str
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/files.py` & `cuenca-1.0.0/cuenca/resources/files.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 from io import BytesIO
 from typing import ClassVar, Optional, cast
 
-from cuenca_validations.types import (
-    FileFormat,
-    FileQuery,
-    FileUploadRequest,
-    KYCFileType,
-)
+from cuenca_validations.types import FileQuery, FileUploadRequest, KYCFileType
 from pydantic import HttpUrl
-from pydantic.dataclasses import dataclass
 
 from ..http import Session, session as global_session
 from .base import Downloadable, Queryable, Uploadable
 
 
-@dataclass
 class File(Downloadable, Queryable, Uploadable):
     _resource: ClassVar = 'files'
     _query_params: ClassVar = FileQuery
 
     extension: str
     type: KYCFileType
     url: HttpUrl
@@ -61,15 +54,15 @@
 
     @property
     def file(self) -> bytes:
         """
         Bytes of the decrypted file.
         Format of the file is found on `file_type` property.
         """
-        return self.download(self, file_format=FileFormat.any).read()
+        return self.download(self.id).read()
 
     @property
     def pdf(self) -> bytes:
         """
         Override from `Downloadable`, this property does not apply.
         """
         raise NotImplementedError
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/identities.py` & `cuenca-1.0.0/cuenca/resources/identities.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,18 @@
     KYCFile,
     State,
     TOSAgreement,
     UserStatus,
     VerificationStatus,
 )
 from cuenca_validations.types.identities import CurpField
-from pydantic.dataclasses import dataclass
 
 from .base import Queryable, Retrievable
 
 
-@dataclass
 class Identity(Retrievable, Queryable):
     _resource: ClassVar = 'identities'
     _query_params: ClassVar = IdentityQuery
 
     created_at: dt.datetime
     names: str
     first_surname: str
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/limited_wallets.py` & `cuenca-1.0.0/cuenca/resources/limited_wallets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-from dataclasses import dataclass
 from typing import ClassVar, Optional, cast
 
 from clabe import Clabe
 from cuenca_validations.types import (
     AccountQuery,
     CurpField,
     LimitedWalletRequest,
     Rfc,
 )
 
 from .base import Wallet
 
 
-@dataclass
 class LimitedWallet(Wallet):
     _resource: ClassVar = 'limited_wallets'
     _query_params: ClassVar = AccountQuery
     account_number: Clabe
-    allowed_rfc: Rfc
+    allowed_rfc: Optional[Rfc]
     allowed_curp: CurpField
 
     @classmethod
     def create(
         cls,
         allowed_curp: Optional[CurpField] = None,
         allowed_rfc: Optional[Rfc] = None,
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/login_tokens.py` & `cuenca-1.0.0/cuenca/resources/login_tokens.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import ClassVar, cast
 
-from pydantic.dataclasses import dataclass
-
 from ..http import Session, session as global_session
 from .base import Creatable
 
 
-@dataclass
 class LoginToken(Creatable):
     _resource: ClassVar = 'login_tokens'
 
+    class Config:
+        schema_extra = {'example': {'id': 'LTNEUInh69SuKXXmK95sROwQ'}}
+
     @classmethod
     def create(cls, session: Session = global_session) -> 'LoginToken':
         """
         Use this method to create a token that will last for 7 days
         Make sure to store this token in a safe place
         :return: Token that you can use in cuenca.configure
         """
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/resources.py` & `cuenca-1.0.0/cuenca/resources/resources.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/savings.py` & `cuenca-1.0.0/cuenca/resources/savings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import datetime as dt
-from dataclasses import dataclass
 from typing import ClassVar, Optional, cast
 
 from cuenca_validations.types import (
     SavingCategory,
     SavingRequest,
     SavingUpdateRequest,
     StrictPositiveInt,
     WalletQuery,
 )
 
 from .base import Updateable, Wallet
 
 
-@dataclass
 class Saving(Wallet, Updateable):
     _resource: ClassVar = 'savings'
     _query_params: ClassVar = WalletQuery
     name: str
     category: SavingCategory
     goal_amount: Optional[StrictPositiveInt]
     goal_date: Optional[dt.datetime]
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/transfers.py` & `cuenca-1.0.0/cuenca/resources/transfers.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,22 @@
 
 from cuenca_validations.types import (
     TransferNetwork,
     TransferQuery,
     TransferRequest,
 )
 from cuenca_validations.typing import DictStrAny
-from pydantic.dataclasses import dataclass
 from requests import HTTPError
 
 from ..exc import CuencaException
 from .accounts import Account
 from .base import Creatable, Transaction
 from .resources import retrieve_uri
 
 
-@dataclass
 class Transfer(Transaction, Creatable):
     _resource: ClassVar = 'transfers'
     _query_params: ClassVar = TransferQuery
 
     updated_at: dt.datetime
     recipient_name: str
     account_number: str
@@ -37,22 +35,24 @@
     def create(
         cls,
         account_number: str,
         amount: int,
         descriptor: str,
         recipient_name: str,
         idempotency_key: Optional[str] = None,
+        user_id: Optional[str] = None,
     ) -> 'Transfer':
         """
         :param account_number: CLABE
         :param amount: needs to be in centavos (not pesos)
         :param descriptor: how it'll appear for the recipient
         :param recipient_name: name of recipient
         :param idempotency_key: must be unique for each transfer to avoid
             duplicates
+        :param user_id: Source user to take the funds
         :return: Transfer object
 
         The recommended idempotency_key scheme:
         1. create a transfer entry in your own database with the status
             created
         2. call this method with the unique id from your database as the
             idempotency_key
@@ -63,14 +63,15 @@
             idempotency_key = cls._gen_idempotency_key(account_number, amount)
         req = TransferRequest(
             account_number=account_number,
             amount=amount,
             descriptor=descriptor,
             recipient_name=recipient_name,
             idempotency_key=idempotency_key,
+            user_id=user_id,
         )
         return cast('Transfer', cls._create(**req.dict()))
 
     @classmethod
     def create_many(cls, requests: List[TransferRequest]) -> DictStrAny:
         transfers: DictStrAny = dict(submitted=[], errors=[])
         for req in requests:
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/user_credentials.py` & `cuenca-1.0.0/cuenca/resources/user_credentials.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import datetime as dt
 from typing import ClassVar, Optional, cast
 
 from cuenca_validations.types.requests import (
     UserCredentialRequest,
     UserCredentialUpdateRequest,
 )
-from pydantic.dataclasses import dataclass
 
 from ..http import Session, session as global_session
 from .base import Creatable, Updateable
 
 
-@dataclass
 class UserCredential(Creatable, Updateable):
     _resource: ClassVar = 'user_credentials'
 
     is_active: bool
     created_at: dt.datetime
 
     @classmethod
     def create(
-        cls, password: str, *, session: Session = global_session
+        cls,
+        password: str,
+        user_id: Optional[str] = None,
+        *,
+        session: Session = global_session,
     ) -> 'UserCredential':
-        req = UserCredentialRequest(password=password)
+        req = UserCredentialRequest(password=password, user_id=user_id)
         return cast(
             'UserCredential', cls._create(**req.dict(), session=session)
         )
 
     @classmethod
     def update(
         cls,
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/user_logins.py` & `cuenca-1.0.0/cuenca/resources/user_logins.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 import datetime as dt
-from dataclasses import dataclass
 from typing import ClassVar, Optional, cast
 
-from cuenca_validations.types.requests import UserCredentialRequest
+from cuenca_validations.types.requests import UserLoginRequest
 
 from ..http import Session, session as global_session
 from .base import Creatable
 
 
-@dataclass
 class UserLogin(Creatable):
     _resource: ClassVar = 'user_logins'
 
     last_login_at: Optional[dt.datetime]
     success: bool
 
+    class Config:
+        schema_extra = {
+            'example': {
+                'id': 'ULNEUInh69SuKXXmK95sROwQ',
+                'last_login_at': '2022-01-01T14:15:22Z',
+                'success': True,
+            }
+        }
+
     @classmethod
     def create(
-        cls, password: str, *, session: Session = global_session
+        cls,
+        password: str,
+        user_id: Optional[str] = None,
+        *,
+        session: Session = global_session,
     ) -> 'UserLogin':
-        req = UserCredentialRequest(password=password)
+        req = UserLoginRequest(password=password, user_id=user_id)
         login = cast('UserLogin', cls._create(session=session, **req.dict()))
         if login.success:
-            session.session.headers['X-Cuenca-LoginId'] = login.id
+            session.headers['X-Cuenca-LoginId'] = login.id
         return login
 
     @classmethod
     def logout(
         cls, user_id: str = 'me', *, session: Session = global_session
     ) -> None:
         # Using user_id vs user_login_id to avoid needing to store
         # user_login_id or perform a query to fetch it
         session.delete(f'{cls._resource}/{user_id}', dict())
-        session.session.headers.pop('X-Cuenca-LoginId', None)
+        session.headers.pop('X-Cuenca-LoginId', None)
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/users.py` & `cuenca-1.0.0/cuenca/resources/platforms.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,79 @@
 import datetime as dt
-from typing import ClassVar, List, Optional, cast
+from typing import ClassVar, Optional, cast
 
-from cuenca_validations.types import (
-    Address,
-    AddressUpdateRequest,
-    Beneficiary,
-    KYCFile,
-    KYCFileUpdateRequest,
-    PhoneNumber,
-    TOSAgreement,
-    TOSUpdateRequest,
-    UserQuery,
-    UserRequest,
-    UserStatus,
-    UserUpdateRequest,
-)
-from cuenca_validations.types.identities import CurpField
-from pydantic import EmailStr
-from pydantic.dataclasses import dataclass
+from cuenca_validations.types import Country, PlatformRequest, State
 
 from ..http import Session, session as global_session
-from .base import Creatable, Queryable, Retrievable, Updateable
-from .identities import Identity
-from .resources import retrieve_uri
+from .base import Creatable
 
 
-@dataclass
-class User(Creatable, Retrievable, Updateable, Queryable):
-    _resource: ClassVar = 'users'
-    _query_params: ClassVar = UserQuery
+class Platform(Creatable):
+    _resource: ClassVar = 'platforms'
 
-    identity_uri: str
-    level: int
     created_at: dt.datetime
-    phone_number: Optional[PhoneNumber]
-    email_address: Optional[EmailStr]
-    profession: Optional[str]
-    terms_of_service: Optional[TOSAgreement]
-    status: Optional[UserStatus]
-    address: Optional[Address]
-    govt_id: Optional[KYCFile]
-    proof_of_address: Optional[KYCFile]
-    proof_of_life: Optional[KYCFile]
-    beneficiaries: Optional[List[Beneficiary]]
-    platform_id: Optional[str] = None
+    name: str
+    rfc: Optional[str] = None
+    establishment_date: Optional[dt.date] = None
+    country: Optional[Country] = None
+    state: Optional[State] = None
+    economic_activity: Optional[str] = None
+    email_address: Optional[str] = None
+    phone_number: Optional[str] = None
+
+    class Config:
+        fields = {
+            'name': {'description': 'name of the platform being created'},
+            'rfc': {'description': 'RFC or CURP of the platform'},
+            'establishment_date': {
+                'description': 'when the platform was established'
+            },
+            'country': {'description': 'country where the platform resides'},
+            'state': {'description': 'state where the platform resides'},
+            'economic_activity': {'description': 'what the platform does'},
+            'phone_number': {
+                'description': 'phone number to contact the platform'
+            },
+            'email_address': {
+                'description': 'email address to contact the platform'
+            },
+        }
+        schema_extra = {
+            'example': {
+                'id': 'PT0123456789',
+                'name': 'Arteria',
+                'created_at': '2021-08-24T14:15:22Z',
+                'rfc': 'ART123456FFF',
+                'establishment_date': '2021-08-24T14:15:22Z',
+                'country': 'MX',
+                'state': 'DF',
+                'economic_activity': 'fiinances and technologies',
+                'phone_number': '+525555555555',
+                'email_address': 'art@eria.com',
+            }
+        }
 
     @classmethod
     def create(
         cls,
-        curp: CurpField,
-        phone_number: Optional[PhoneNumber] = None,
-        email_address: Optional[EmailStr] = None,
-        profession: Optional[str] = None,
-        address: Optional[Address] = None,
-        email_verification_id: Optional[str] = None,
-        phone_verification_id: Optional[str] = None,
-        *,
-        session: Session = global_session,
-    ) -> 'User':
-        req = UserRequest(
-            curp=curp,
-            phone_number=phone_number,
-            email_address=email_address,
-            profession=profession,
-            address=address,
-            email_verification_id=email_verification_id,
-            phone_verification_id=phone_verification_id,
-        )
-        return cast('User', cls._create(session=session, **req.dict()))
-
-    @classmethod
-    def update(
-        cls,
-        user_id: str,
-        phone_number: Optional[PhoneNumber] = None,
+        name: str,
+        rfc: Optional[str] = None,
+        establishment_date: Optional[str] = None,
+        country: Optional[Country] = None,
+        state: Optional[State] = None,
+        economic_activity: Optional[str] = None,
+        phone_number: Optional[str] = None,
         email_address: Optional[str] = None,
-        profession: Optional[str] = None,
-        address: Optional[AddressUpdateRequest] = None,
-        beneficiaries: Optional[List[Beneficiary]] = None,
-        govt_id: Optional[KYCFileUpdateRequest] = None,
-        proof_of_address: Optional[KYCFileUpdateRequest] = None,
-        proof_of_life: Optional[KYCFileUpdateRequest] = None,
-        terms_of_service: Optional[TOSUpdateRequest] = None,
-        verification_id: Optional[str] = None,
         *,
         session: Session = global_session,
-    ):
-        request = UserUpdateRequest(
+    ) -> 'Platform':
+        req = PlatformRequest(
+            name=name,
+            rfc=rfc,
+            establishment_date=establishment_date,
+            country=country,
+            state=state,
+            economic_activity=economic_activity,
             phone_number=phone_number,
             email_address=email_address,
-            profession=profession,
-            address=address,
-            beneficiaries=beneficiaries,
-            govt_id=govt_id,
-            proof_of_address=proof_of_address,
-            proof_of_life=proof_of_life,
-            terms_of_service=terms_of_service,
-            verification_id=verification_id,
         )
-        return cast(
-            'User',
-            cls._update(id=user_id, **request.dict(), session=session),
-        )
-
-    @property
-    def identity(self) -> Identity:
-        return cast(Identity, retrieve_uri(self.identity_uri))
+        return cast('Platform', cls._create(session=session, **req.dict()))
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/verifications.py` & `cuenca-1.0.0/cuenca/resources/questionnaires.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 import datetime as dt
-from typing import ClassVar, Optional, Union, cast
+from typing import ClassVar, cast
 
-from cuenca_validations.types import (
-    VerificationAttemptRequest,
-    VerificationRequest,
-    VerificationType,
-)
-from cuenca_validations.types.identities import PhoneNumber
-from pydantic import EmailStr
-from pydantic.dataclasses import dataclass
+from cuenca_validations.types import QuestionnairesRequest
 
 from ..http import Session, session as global_session
-from .base import Creatable, Updateable
+from .base import Creatable, Retrievable
 
 
-@dataclass
-class Verification(Creatable, Updateable):
-    _resource: ClassVar = 'verifications'
+class Questionnaires(Creatable, Retrievable):
+    _resource: ClassVar = 'questionnaires'
 
-    recipient: Union[EmailStr, PhoneNumber]
-    type: VerificationType
     created_at: dt.datetime
-    deactivated_at: Optional[dt.datetime]
+    token: str
+    form_id: str
+    user_id: str
+
+    class Config:
+        schema_extra = {
+            'example': {
+                'user_id': 'US234i23jh23h4h23',
+                'token': '3223j23ij23ij3',
+                'alert_id': 'ALewifjwiejf',
+            }
+        }
 
     @classmethod
     def create(
         cls,
-        recipient: str,
-        type: VerificationType,
-        platform_id: str,
+        user_id: str,
+        token: str,
+        form_id: str,
+        *,
         session: Session = global_session,
-    ) -> 'Verification':
-        req = VerificationRequest(
-            recipient=recipient, type=type, platform_id=platform_id
+    ) -> 'Questionnaires':
+        req = QuestionnairesRequest(
+            user_id=user_id,
+            token=token,
+            form_id=form_id,
         )
-        return cast('Verification', cls._create(**req.dict(), session=session))
-
-    @classmethod
-    def verify(
-        cls,
-        id: str,
-        code: str,
-        session: Session = global_session,
-    ) -> 'Verification':
-        req = VerificationAttemptRequest(code=code)
         return cast(
-            'Verification',
-            cls._update(id=id, **req.dict(), session=session),
+            'Questionnaires', cls._create(session=session, **req.dict())
         )
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/wallet_transactions.py` & `cuenca-1.0.0/cuenca/resources/wallet_transactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from dataclasses import dataclass
 from typing import ClassVar, Optional, cast
 
 from cuenca_validations.types import (
     WalletTransactionQuery,
     WalletTransactionRequest,
     WalletTransactionType,
 )
 
 from cuenca.resources.base import Creatable, Transaction
 from cuenca.resources.resources import retrieve_uri
 
 from .base import Wallet
 
 
-@dataclass
 class WalletTransaction(Transaction, Creatable):
     _resource: ClassVar = 'wallet_transactions'
     _query_params: ClassVar = WalletTransactionQuery
 
     transaction_type: WalletTransactionType
     wallet_uri: str
```

### Comparing `cuenca-0.9.4.dev0/cuenca/resources/whatsapp_transfers.py` & `cuenca-1.0.0/cuenca/resources/whatsapp_transfers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import datetime as dt
 from typing import ClassVar, Optional, cast
 
 from cuenca_validations.types import TransferNetwork
-from pydantic.dataclasses import dataclass
 
 from .accounts import Account
 from .base import Transaction
 from .resources import retrieve_uri
 
 
-@dataclass
 class WhatsappTransfer(Transaction):
     _resource: ClassVar = 'whatsapp_transfers'
 
     updated_at: dt.datetime
     recipient_name: str
     phone_number: str
     claim_url: Optional[str]
```

### Comparing `cuenca-0.9.4.dev0/cuenca.egg-info/PKG-INFO` & `cuenca-1.0.0/cuenca.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cuenca
-Version: 0.9.4.dev0
+Version: 1.0.0
 Summary: Cuenca API Client
 Home-page: https://github.com/cuenca-mx/cuenca-python
 Author: Cuenca
 Author-email: dev@cuenca.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests<28,>=2.24
+Requires-Dist: dataclasses>=0.7; python_version < "3.8"
+Requires-Dist: cuenca-validations<0.12.0,>=0.11.3
 
 # Cuenca – Python client library
 
 [![test](https://github.com/cuenca-mx/cuenca-python/workflows/test/badge.svg)](https://github.com/cuenca-mx/cuenca-python/actions?query=workflow%3Atest)
 [![codecov](https://codecov.io/gh/cuenca-mx/cuenca-python/branch/main/graph/badge.svg)](https://codecov.io/gh/cuenca-mx/cuenca-python)
 [![PyPI](https://img.shields.io/pypi/v/cuenca.svg)](https://pypi.org/project/cuenca/)
```

### Comparing `cuenca-0.9.4.dev0/cuenca.egg-info/SOURCES.txt` & `cuenca-1.0.0/cuenca.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -21,33 +21,39 @@
 cuenca/resources/balance_entries.py
 cuenca/resources/base.py
 cuenca/resources/bill_payments.py
 cuenca/resources/card_activations.py
 cuenca/resources/card_transactions.py
 cuenca/resources/card_validations.py
 cuenca/resources/cards.py
+cuenca/resources/cash_references.py
+cuenca/resources/clabes.py
 cuenca/resources/commissions.py
 cuenca/resources/curp_validations.py
 cuenca/resources/deposits.py
 cuenca/resources/endpoints.py
 cuenca/resources/file_batches.py
 cuenca/resources/files.py
 cuenca/resources/identities.py
 cuenca/resources/identity_events.py
+cuenca/resources/kyc_validations.py
 cuenca/resources/kyc_verifications.py
 cuenca/resources/limited_wallets.py
 cuenca/resources/login_tokens.py
+cuenca/resources/platforms.py
+cuenca/resources/questionnaires.py
 cuenca/resources/resources.py
 cuenca/resources/savings.py
 cuenca/resources/service_providers.py
 cuenca/resources/sessions.py
 cuenca/resources/statements.py
 cuenca/resources/transfers.py
 cuenca/resources/user_credentials.py
 cuenca/resources/user_events.py
+cuenca/resources/user_lists_validation.py
 cuenca/resources/user_logins.py
 cuenca/resources/users.py
 cuenca/resources/verifications.py
 cuenca/resources/wallet_transactions.py
 cuenca/resources/webhooks.py
 cuenca/resources/whatsapp_transfers.py
 tests/__init__.py
@@ -63,32 +69,38 @@
 tests/resources/test_arpc.py
 tests/resources/test_balance_entries.py
 tests/resources/test_bill_payments.py
 tests/resources/test_card_activations.py
 tests/resources/test_card_transactions.py
 tests/resources/test_card_validations.py
 tests/resources/test_cards.py
+tests/resources/test_cash_references.py
+tests/resources/test_clabes.py
 tests/resources/test_commissions.py
 tests/resources/test_curp_validations.py
 tests/resources/test_deposits.py
 tests/resources/test_endpoints.py
 tests/resources/test_file_batches.py
 tests/resources/test_files.py
 tests/resources/test_identities.py
 tests/resources/test_identity_events.py
+tests/resources/test_kyc_validations.py
 tests/resources/test_kyc_verifications.py
 tests/resources/test_limited_wallets.py
 tests/resources/test_login_tokens.py
+tests/resources/test_platforms.py
+tests/resources/test_questionnaires.py
 tests/resources/test_resources.py
 tests/resources/test_savings.py
 tests/resources/test_service_providers.py
 tests/resources/test_sessions.py
 tests/resources/test_statements.py
 tests/resources/test_transfers.py
 tests/resources/test_user_credentials.py
 tests/resources/test_user_events.py
+tests/resources/test_user_lists_validation.py
 tests/resources/test_user_logins.py
 tests/resources/test_users.py
 tests/resources/test_verifications.py
 tests/resources/test_wallet_transactions.py
 tests/resources/test_webhooks.py
 tests/resources/test_whatsapp_transfers.py
```

### Comparing `cuenca-0.9.4.dev0/tests/conftest.py` & `cuenca-1.0.0/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,10 +60,21 @@
             country=Country.MX,
         ),
     )
     return user_dict
 
 
 @pytest.fixture
+def user_lists_request() -> Dict:
+    user_dict = dict(
+        curp='LOHJ660606HDFPRS02',
+        names='Alejandro',
+        first_surname='Martinez',
+        second_surname='Viquez',
+    )
+    return user_dict
+
+
+@pytest.fixture
 def file() -> BytesIO:
     with open('tests/data/test_file.jpeg', 'rb') as image_file:
         return BytesIO(image_file.read())
```

### Comparing `cuenca-0.9.4.dev0/tests/http/test_client.py` & `cuenca-1.0.0/tests/http/test_client.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_api_keys.py` & `cuenca-1.0.0/tests/resources/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_balance_entries.py` & `cuenca-1.0.0/tests/resources/test_balance_entries.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_card_activations.py` & `cuenca-1.0.0/tests/resources/test_card_activations.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_card_transactions.py` & `cuenca-1.0.0/tests/resources/test_card_transactions.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_card_validations.py` & `cuenca-1.0.0/tests/resources/test_card_validations.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_cards.py` & `cuenca-1.0.0/tests/resources/test_cards.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import datetime as dt
+
 import pytest
 from cuenca_validations.types import (
     CardFundingType,
     CardIssuer,
     CardStatus,
     CardType,
 )
@@ -16,32 +18,61 @@
 @pytest.mark.vcr
 def test_card_create():
     card = Card.create(CardIssuer.cuenca, CardFundingType.credit, user_id)
     assert card.id
     assert len(card.number) == 16
     assert card.type == CardType.virtual
     assert card.user_id == user_id
+    assert card.is_dynamic_cvv is False
+
+
+@pytest.mark.vcr
+def test_card_create_dcvv():
+    card = Card.create(
+        CardIssuer.cuenca, CardFundingType.credit, user_id, is_dynamic_cvv=True
+    )
+    assert card.id
+    assert len(card.number) == 16
+    assert card.type == CardType.virtual
+    assert card.user_id == user_id
+    assert card.is_dynamic_cvv is True
 
 
 @pytest.mark.vcr
 def test_can_not_assign_new_virtual_card():
     with pytest.raises(CuencaResponseException) as exc:
         Card.create(CardIssuer.cuenca, CardFundingType.credit, user_id)
     assert exc.value
 
 
 @pytest.mark.vcr
 def test_card_retrieve():
     card: Card = Card.retrieve(card_id)
     assert card.id == card_id
     assert len(card.number) == 16
-    assert card.last_4_digits == '9849'
+    assert card.last_4_digits == '7265'
+    assert card.bin == '544875'
+    assert card.type == CardType.virtual
+    assert not card.pin_attempts_exceeded
+    assert card.is_dynamic_cvv is False
+    assert card.dcvv is None
+
+
+@pytest.mark.vcr
+def test_card_retrieve_dcvv():
+    card: Card = Card.retrieve(card_id)
+    assert card.id == card_id
+    assert len(card.number) == 16
+    assert card.last_4_digits == '7265'
     assert card.bin == '544875'
     assert card.type == CardType.virtual
     assert not card.pin_attempts_exceeded
+    assert card.is_dynamic_cvv is True
+    assert card.dcvv.isdigit()
+    assert isinstance(card.dcvv_expires_at, dt.datetime)
 
 
 @pytest.mark.vcr
 def test_card_not_found():
     with pytest.raises(CuencaResponseException) as exc:
         Card.retrieve('not-existing-id')
     assert exc.value.status_code == 404
```

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_commissions.py` & `cuenca-1.0.0/tests/resources/test_commissions.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_curp_validations.py` & `cuenca-1.0.0/tests/resources/test_curp_validations.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_endpoints.py` & `cuenca-1.0.0/tests/resources/test_endpoints.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,18 +32,21 @@
         assert exc.json['error'] == 'Usuario ya tiene webhook asociado'
 
 
 @pytest.mark.vcr
 def test_endpoint_update():
     id_endpoint = 'EN02'
     endpoint: Endpoint = Endpoint.update(
-        endpoint_id=id_endpoint, url='https://url.io', is_enable=False
+        endpoint_id=id_endpoint,
+        url='https://url.io',
+        is_enable=False,
+        events=['user.create', 'cash_deposit.create'],
     )
     assert endpoint.id == id_endpoint
-    assert endpoint.events
+    assert len(endpoint.events) == 2
     assert endpoint.url == 'https://url.io'
     assert not endpoint.is_enable
     assert endpoint.is_active
 
 
 @pytest.mark.vcr
 def test_endpoint_deactivate():
```

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_file_batches.py` & `cuenca-1.0.0/tests/resources/test_file_batches.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_files.py` & `cuenca-1.0.0/tests/resources/test_files.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 @pytest.mark.vcr
 def test_file_download():
     file: File = File.first(type=KYCFileType.ine)
     assert isinstance(file.file, bytes)
 
 
 @pytest.mark.vcr
+def test_file_download_only_bytes():
+    # Only download Bytes
+    downloaded_file = File.download('EFXXX')
+    assert isinstance(downloaded_file.read(), bytes)
+
+
+@pytest.mark.vcr
 def test_file_error_on_xml_pdf():
     file: File = File.first(type=KYCFileType.ine)
     with pytest.raises(NotImplementedError):
         file.xml
 
     with pytest.raises(NotImplementedError):
         file.pdf
```

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_kyc_verifications.py` & `cuenca-1.0.0/tests/resources/test_kyc_verifications.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_limited_wallets.py` & `cuenca-1.0.0/tests/resources/test_limited_wallets.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_login_tokens.py` & `cuenca-1.0.0/tests/resources/test_login_tokens.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pytest
 
 from cuenca import LoginToken, Transfer, UserLogin
 from cuenca.http.client import Session
 
 
-@pytest.fixture
+@pytest.fixture(scope='function')
 def session():
     session = Session()
     session.configure(
         'api_key',
         'api_secret',
         sandbox=True,
     )
     return session
 
 
 @pytest.mark.vcr
 def test_login_token(session):
     UserLogin.create('222222', session=session)
     login_token = LoginToken.create(session=session)
-    session.session.headers.pop('X-Cuenca-LoginId')
+    session.headers.pop('X-Cuenca-LoginId')
     session.configure(login_token=login_token.id)
     Transfer.count(session=session)
```

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_savings.py` & `cuenca-1.0.0/tests/resources/test_savings.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_service_providers.py` & `cuenca-1.0.0/tests/resources/test_service_providers.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_sessions.py` & `cuenca-1.0.0/tests/resources/test_sessions.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_transfers.py` & `cuenca-1.0.0/tests/resources/test_transfers.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_user_credentials.py` & `cuenca-1.0.0/tests/resources/test_user_credentials.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_user_logins.py` & `cuenca-1.0.0/tests/resources/test_user_logins.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 
 @pytest.mark.vcr
 def test_valid_login(session: Session):
     login = UserLogin.create('222222', session=session)
     assert login.success
     assert login.last_login_at is not None
     assert login.id is not None
-    assert session.session.headers['X-Cuenca-LoginId'] == login.id
+    assert session.headers['X-Cuenca-LoginId'] == login.id
 
 
 @pytest.mark.vcr
 def test_invalid_login(session: Session):
     login = UserLogin.create('111111', session=session)
     assert not login.success
     assert login.last_login_at is None
     assert login.id is not None
-    assert 'X-Cuenca-LoginId' not in session.session.headers
+    assert 'X-Cuenca-LoginId' not in session.headers
 
 
 @pytest.mark.vcr
 def test_logout(session: Session):
     UserLogin.create('222222', session=session)
     UserLogin.logout(session=session)
-    assert 'X-Cuenca-LoginId' not in session.session.headers
+    assert 'X-Cuenca-LoginId' not in session.headers
```

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_verifications.py` & `cuenca-1.0.0/tests/resources/test_verifications.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_wallet_transactions.py` & `cuenca-1.0.0/tests/resources/test_wallet_transactions.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/resources/test_whatsapp_transfers.py` & `cuenca-1.0.0/tests/resources/test_whatsapp_transfers.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/test_cuenca.py` & `cuenca-1.0.0/tests/test_cuenca.py`

 * *Files identical despite different names*

### Comparing `cuenca-0.9.4.dev0/tests/test_jwt.py` & `cuenca-1.0.0/tests/test_jwt.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'expires_at, should_be_expired',
     [
         (dt.datetime.utcnow() + dt.timedelta(days=-1), True),
         (dt.datetime.utcnow() + dt.timedelta(days=1), False),
     ],
 )
 def test_expired(expires_at: dt.datetime, should_be_expired: bool):
-    jwt = Jwt(expires_at, '_')
+    jwt = Jwt(expires_at=expires_at, token='_')
     assert jwt.is_expired == should_be_expired
 
 
 def test_get_expiration_date():
     assert Jwt.get_expiration_date(TEST_TOKEN) == dt.datetime(2020, 11, 25)
```

