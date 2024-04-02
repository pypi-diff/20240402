# Comparing `tmp/outsetapy-0.1.4.tar.gz` & `tmp/outsetapy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outsetapy-0.1.4.tar", last modified: Mon Apr  1 15:51:44 2024, max compression
+gzip compressed data, was "outsetapy-0.1.5.tar", last modified: Tue Apr  2 16:00:38 2024, max compression
```

## Comparing `outsetapy-0.1.4.tar` & `outsetapy-0.1.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-01 15:51:44.970419 outsetapy-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-01 15:51:39.000000 outsetapy-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:51:44.970419 outsetapy-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.958419 outsetapy-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.962419 outsetapy-0.1.4/src/outsetapy/
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.962419 outsetapy-0.1.4/src/outsetapy/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/__inti__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.962419 outsetapy-0.1.4/src/outsetapy/api/billing/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/invoices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/plan_families.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.962419 outsetapy-0.1.4/src/outsetapy/api/crm/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/crm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/crm/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/crm/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/crm/deals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/crm/people.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.962419 outsetapy-0.1.4/src/outsetapy/api/marketing/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/marketing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/marketing/email_list_subscriptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.966419 outsetapy-0.1.4/src/outsetapy/api/support/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/support/cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.966419 outsetapy-0.1.4/src/outsetapy/api/user/
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/user/password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/user/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.966419 outsetapy-0.1.4/src/outsetapy/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.966419 outsetapy-0.1.4/src/outsetapy/models/billing/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/add_on.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/billing_add_on_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/billing_renewal_term.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/billing_transaction_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/charge_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/invoice_display_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/invoice_line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/plan_add_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/plan_family.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/subscription_add_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/usage_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy/models/crm/
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/account.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/account_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/activity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/deal.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/deal_person.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/deal_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/deal_pipeline_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/person_account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy/models/marketing/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/marketing/email_list_person.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/marketing/emaillist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/shared/address.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/shared/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy/models/support/
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/support/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/support/case_history.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/support/case_source.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/support/case_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy/models/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/wrappers/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/wrappers/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/util/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/util/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/util/store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-01 15:51:44.000000 outsetapy-0.1.4/src/outsetapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-01 15:51:44.000000 outsetapy-0.1.4/src/outsetapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:51:44.000000 outsetapy-0.1.4/src/outsetapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 15:51:44.000000 outsetapy-0.1.4/src/outsetapy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.934439 outsetapy-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-02 16:00:38.934439 outsetapy-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 16:00:30.000000 outsetapy-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:00:38.934439 outsetapy-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.922438 outsetapy-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.922438 outsetapy-0.1.5/src/outsetapy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.926438 outsetapy-0.1.5/src/outsetapy/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/__inti__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.926438 outsetapy-0.1.5/src/outsetapy/api/billing/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/billing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/billing/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/billing/plan_families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/billing/plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/billing/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/billing/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/billing/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.926438 outsetapy-0.1.5/src/outsetapy/api/crm/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/crm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/crm/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/crm/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/crm/deals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/crm/people.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.926438 outsetapy-0.1.5/src/outsetapy/api/marketing/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/marketing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/marketing/email_list_subscriptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.926438 outsetapy-0.1.5/src/outsetapy/api/support/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/support/cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.926438 outsetapy-0.1.5/src/outsetapy/api/user/
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/user/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/api/user/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.926438 outsetapy-0.1.5/src/outsetapy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.930439 outsetapy-0.1.5/src/outsetapy/models/billing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/add_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/billing_add_on_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/billing_renewal_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/billing_transaction_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/charge_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/invoice_display_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/invoice_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/plan_add_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/plan_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/subscription_add_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/billing/usage_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.930439 outsetapy-0.1.5/src/outsetapy/models/crm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/crm/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/crm/account_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/crm/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/crm/activity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/crm/deal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/crm/deal_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/crm/deal_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/crm/deal_pipeline_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/crm/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/crm/person_account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.934439 outsetapy-0.1.5/src/outsetapy/models/marketing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/marketing/email_list_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/marketing/emaillist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.934439 outsetapy-0.1.5/src/outsetapy/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/shared/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/shared/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.934439 outsetapy-0.1.5/src/outsetapy/models/support/
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/support/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/support/case_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/support/case_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/support/case_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.934439 outsetapy-0.1.5/src/outsetapy/models/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/wrappers/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/models/wrappers/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.934439 outsetapy-0.1.5/src/outsetapy/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/util/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 16:00:30.000000 outsetapy-0.1.5/src/outsetapy/util/store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:00:38.934439 outsetapy-0.1.5/src/outsetapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-02 16:00:38.000000 outsetapy-0.1.5/src/outsetapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-02 16:00:38.000000 outsetapy-0.1.5/src/outsetapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:00:38.000000 outsetapy-0.1.5/src/outsetapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 16:00:38.000000 outsetapy-0.1.5/src/outsetapy.egg-info/top_level.txt
```

### Comparing `outsetapy-0.1.4/pyproject.toml` & `outsetapy-0.1.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "outsetapy"
-version = "0.1.4"
+version = "0.1.5"
 
 authors = [
   { name="Roborian, Inc", email="info@roborian.com" },
 ]
 description = "A SDK for building applications with Outseta"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `outsetapy-0.1.4/src/outsetapy/__init__.py` & `outsetapy-0.1.5/src/outsetapy/__init__.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/billing/__init__.py` & `outsetapy-0.1.5/src/outsetapy/api/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/billing/invoices.py` & `outsetapy-0.1.5/src/outsetapy/api/billing/invoices.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/billing/plan_families.py` & `outsetapy-0.1.5/src/outsetapy/api/billing/plan_families.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/billing/plans.py` & `outsetapy-0.1.5/src/outsetapy/api/billing/plans.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/billing/subscriptions.py` & `outsetapy-0.1.5/src/outsetapy/api/billing/subscriptions.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/billing/transactions.py` & `outsetapy-0.1.5/src/outsetapy/api/billing/transactions.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/billing/usage.py` & `outsetapy-0.1.5/src/outsetapy/api/billing/usage.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/crm/accounts.py` & `outsetapy-0.1.5/src/outsetapy/api/crm/accounts.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/crm/activities.py` & `outsetapy-0.1.5/src/outsetapy/api/crm/activities.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/crm/deals.py` & `outsetapy-0.1.5/src/outsetapy/api/crm/deals.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/crm/people.py` & `outsetapy-0.1.5/src/outsetapy/api/crm/people.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/marketing/email_list_subscriptions.py` & `outsetapy-0.1.5/src/outsetapy/api/marketing/email_list_subscriptions.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/support/cases.py` & `outsetapy-0.1.5/src/outsetapy/api/support/cases.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/user/__init__.py` & `outsetapy-0.1.5/src/outsetapy/api/user/__init__.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/user/password.py` & `outsetapy-0.1.5/src/outsetapy/api/user/password.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/api/user/profile.py` & `outsetapy-0.1.5/src/outsetapy/api/user/profile.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/billing/add_on.py` & `outsetapy-0.1.5/src/outsetapy/models/billing/add_on.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/billing/charge_summary.py` & `outsetapy-0.1.5/src/outsetapy/models/billing/charge_summary.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/billing/invoice_line_item.py` & `outsetapy-0.1.5/src/outsetapy/models/billing/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/billing/plan.py` & `outsetapy-0.1.5/src/outsetapy/models/billing/plan.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/billing/subscription.py` & `outsetapy-0.1.5/src/outsetapy/models/billing/subscription.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,18 @@
         self.IsPlanUpgradeRequired = None
         self.PlanUpgradeRequiredMessage = None
         self.Created = None
         self.Updated = None
         if "_objectType" in data and data["_objectType"] == "Subscription":
             self.Uid = data["Uid"]
             self.BillingRenewalTerm = data["BillingRenewalTerm"]
-            self.Account_Uid = data["Account"]['Uid']
+            if "Account" in data and data['Account'] is not None and '_objectType' in data["Account"] and data["Account"]["_objectType"] == 'Account':
+                self.Account_Uid = data["Account"]['Uid']
+            else:
+                self.Account_Uid = data["Account"]
             self._plan = data["Plan"]['Uid']
             self.Quantity = data["Quantity"]
             self.StartDate = data["StartDate"]
             self.EndDate = data["EndDate"]
             self.RenewalDate = data["RenewalDate"]
             self.NewRequiredQuantity = data["NewRequiredQuantity"]
             self.IsPlanUpgradeRequired = data["IsPlanUpgradeRequired"]
```

### Comparing `outsetapy-0.1.4/src/outsetapy/models/billing/subscription_add_on.py` & `outsetapy-0.1.5/src/outsetapy/models/billing/subscription_add_on.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/billing/transaction.py` & `outsetapy-0.1.5/src/outsetapy/models/billing/transaction.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/billing/usage_item.py` & `outsetapy-0.1.5/src/outsetapy/models/billing/usage_item.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/crm/account.py` & `outsetapy-0.1.5/src/outsetapy/models/crm/account.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 from datetime import datetime
 import importlib
 from outsetapy.util.store import Store
 from outsetapy.models.shared.address import Address
-from .deal import Deal
-from .person_account import PersonAccount
-from .account_stage import AccountStage
-
-
-class Subscription:
-    def __init__(self, subscription_id: str, subscription_name: str):
-        self.subscription_id = subscription_id
-        self.subscription_name = subscription_name
+from outsetapy.models.billing.subscription import Subscription
 
+# from .deal import Deal
 
 class Account:
     def __init__(self, data: object, store: Store):
         self.__store = store
         self.Name = None
         self.ClientIdentifier = None
         self.IsDemo = False
-        self.BillingAddress = Address("", "", "", "")
-        self.MailingAddress = Address("", "", "", "")
-        self.AccountStage = AccountStage("", "")
+        self.BillingAddress = Address()
+        self.MailingAddress = Address()
+        self.AccountStage = None
         self.PaymentInformation = None
         self.PersonAccount = []
         self.Subscriptions = []
         self.Deals = []
         self.LastLoginDateTime = None
         self.AccountSpecificPageUrl1 = ""
         self.AccountSpecificPageUrl2 = ""
@@ -64,26 +57,48 @@
             self.AccountSpecificPageUrl4 = data["AccountSpecificPageUrl4"]
             self.AccountSpecificPageUrl5 = data["AccountSpecificPageUrl5"]
             self.RewardFulReferralId = data["RewardFulReferralId"]
             self.HasLoggedIn = data["HasLoggedIn"]
             self.AccountStageLabel = data["AccountStageLabel"]
             self.DomainName = data["DomainName"]
             self.LatestSubscription = data["LatestSubscription"]
-            if "CurrentSubscription" in data and data["CurrentSubscription"] and "Uid" in data["CurrentSubscription"]:
-                self._current_subscription = data["CurrentSubscription"]['Uid']
+            if "CurrentSubscription" in data and data["CurrentSubscription"] is not None and "Uid" in data["CurrentSubscription"]:
+                self._current_subscription = data["CurrentSubscription"]["Uid"]
             else:
-                self._current_subscription = None
+                self._current_subscription = data["CurrentSubscription"]
+
+            # if "CurrentSubscription" in data and '_objectType' in data["CurrentSubscription"] and data["Account"]["_objectType"] == 'Subscription':
+            #     self.CurrentSubscription = Subscription(data["CurrentSubscription"], self.__store)
+            # else:
+            #     self.CurrentSubscription = data["CurrentSubscription"]
             self.PrimaryContact = data["PrimaryContact"]
             self.PrimarySubscription = data["PrimarySubscription"]
             self.RecaptchaToken = data["RecaptchaToken"]
             self.LifetimeRevenue = data["LifetimeRevenue"]
             self.Uid = data["Uid"]
             self.Created = data["Created"]
             self.Updated = data["Updated"]
         elif "_objectType" in data:
             raise Exception(f"Invalid object type: {data['_objectType']}")
-        
+
+    # @property
+    # async def CurrentSubscription(self):
+    #     subscription_api = importlib.import_module("outsetapy.api.billing.subscriptions").Subscriptions(self.__store)
+    #     CurrentSubscription = await subscription_api.get(self._current_subscription)
+    #     return CurrentSubscription
     @property
-    async def CurrentSubscription(self):
+    def CurrentSubscription(self) -> Subscription:
+        if type(self._current_subscription) == Subscription:
+            return self._current_subscription
+        if self._current_subscription is None:
+            return None
         subscription_api = importlib.import_module("outsetapy.api.billing.subscriptions").Subscriptions(self.__store)
-        CurrentSubscription = await subscription_api.get(self._current_subscription)
-        return CurrentSubscription
+        return subscription_api.get(self._current_subscription)
+    @CurrentSubscription.setter
+    def CurrentSubscription(self, value):
+        if type(value) == Subscription:
+            self._current_subscription = value
+        else:
+            if hasattr(value, "Uid"):
+                self._current_subscription = value.Uid
+            else:
+                self._current_subscription = value
```

### Comparing `outsetapy-0.1.4/src/outsetapy/models/crm/activity.py` & `outsetapy-0.1.5/src/outsetapy/models/crm/activity.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/crm/activity_type.py` & `outsetapy-0.1.5/src/outsetapy/models/crm/activity_type.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/crm/deal.py` & `outsetapy-0.1.5/src/outsetapy/models/crm/deal.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/crm/deal_person.py` & `outsetapy-0.1.5/src/outsetapy/models/crm/deal_person.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/crm/deal_pipeline_stage.py` & `outsetapy-0.1.5/src/outsetapy/models/crm/deal_pipeline_stage.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/crm/person_account.py` & `outsetapy-0.1.5/src/outsetapy/models/crm/person_account.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/marketing/email_list_person.py` & `outsetapy-0.1.5/src/outsetapy/models/marketing/email_list_person.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/marketing/emaillist.py` & `outsetapy-0.1.5/src/outsetapy/models/marketing/emaillist.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/support/case.py` & `outsetapy-0.1.5/src/outsetapy/models/support/case.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/support/case_history.py` & `outsetapy-0.1.5/src/outsetapy/models/support/case_history.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/models/wrappers/validation_error.py` & `outsetapy-0.1.5/src/outsetapy/models/wrappers/validation_error.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/util/credentials.py` & `outsetapy-0.1.5/src/outsetapy/util/credentials.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.4/src/outsetapy/util/request.py` & `outsetapy-0.1.5/src/outsetapy/util/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         self.url = urljoin(store.base_url, endpoint)
         self._options = {
             "headers": {
                 "Content-Type": "application/json",
                 "user-agent": "OutsetaPy/" + OUTSETAPY_VERSION,
             }
         }
+        self._body = None
 
     def authenticate_as_user(self):
         self._options["headers"][
             "Authorization"
         ] = self.store.user_auth.authorization_header
         return self
 
@@ -43,18 +44,18 @@
         return self
 
     def with_params(self, params: Dict[str, str]):
         self.url += "?" + urlencode(params)
         return self
 
     def with_body(self, body: Dict[str, Any]):
-        if "body" in self._options:
-            existing_body = self._options["body"]
+        if self._body:
+            existing_body = self._body
             body = {**existing_body, **body}
-        self._options["body"] = body
+        self._body = body
         return self
 
     def get(self) -> requests.Response:
         return self.execute("GET")
 
     def post(self) -> requests.Response:
         return self.execute("POST")
@@ -65,16 +66,16 @@
     def patch(self) -> requests.Response:
         return self.execute("PATCH")
 
     def delete(self) -> requests.Response:
         return self.execute("DELETE")
 
     def execute(self, method) -> requests.Response:
-        self._options["method"] = method
-        return requests.request(**self._options, url=self.url)
+        self._options["method"] = method 
+        return requests.request(**self._options, url=self.url, json=self._body)
 
 
 def hasMoreResults(meta) -> bool:
     return (
         meta["metadata"]["total"]
         > meta["metadata"]["offset"] + meta["metadata"]["limit"]
     )
```

### Comparing `outsetapy-0.1.4/src/outsetapy.egg-info/SOURCES.txt` & `outsetapy-0.1.5/src/outsetapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

