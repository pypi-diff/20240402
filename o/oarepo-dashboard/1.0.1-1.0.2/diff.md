# Comparing `tmp/oarepo-dashboard-1.0.1.tar.gz` & `tmp/oarepo-dashboard-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-dashboard-1.0.1.tar", last modified: Thu Mar 28 15:19:45 2024, max compression
+gzip compressed data, was "oarepo-dashboard-1.0.2.tar", last modified: Tue Apr  2 08:16:58 2024, max compression
```

## Comparing `oarepo-dashboard-1.0.1.tar` & `oarepo-dashboard-1.0.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.426372 oarepo-dashboard-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-28 15:19:45.426372 oarepo-dashboard-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.418372 oarepo-dashboard-1.0.1/oarepo_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.418372 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.410372 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.418372 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/semantic-ui/translations/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/semantic-ui/translations/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.418372 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/semantic-ui/translations/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.410372 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.418372 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.410372 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.418372 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/LC_MESSAGES/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/semantic-ui/translations/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.418372 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.410372 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.418372 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.414372 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.418372 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.418372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.418372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.414372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.414372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.414372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.422372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/CommunityTypeLabel.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/ComputerTabletCommunitiesListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/MobileCommunitiesListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/RestrictedLabel.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.422372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/templates/DashboardCommunitiesPage.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.422372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.414372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.414372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.422372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/custom-components.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.422372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupValueToggler.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.422372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/custom-components.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.422372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/templates/Header.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.422372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_records/
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.414372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_records/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.414372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.414372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.422372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.422372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_records/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_records/templates/DashboardRecordsPage.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_records/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.422372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.414372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.414372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.414372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.422372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/ComputerTabletRequestsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/MobileRequestsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/RequestTypeSpecificComponents.jsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.426372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/icons/TypeIcons.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.426372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/TypeLabels.jsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.426372 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/templates/DashboardRequestsPage.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:19:45.426372 oarepo-dashboard-1.0.1/oarepo_dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-28 15:19:45.000000 oarepo-dashboard-1.0.1/oarepo_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-03-28 15:19:45.000000 oarepo-dashboard-1.0.1/oarepo_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 15:19:45.000000 oarepo-dashboard-1.0.1/oarepo_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-28 15:19:45.000000 oarepo-dashboard-1.0.1/oarepo_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-28 15:19:45.000000 oarepo-dashboard-1.0.1/oarepo_dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-28 15:19:45.000000 oarepo-dashboard-1.0.1/oarepo_dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-28 15:19:45.426372 oarepo-dashboard-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 15:16:59.000000 oarepo-dashboard-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.420006 oarepo-dashboard-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 08:16:58.420006 oarepo-dashboard-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.408006 oarepo-dashboard-1.0.2/oarepo_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.412006 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.404006 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.412006 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/semantic-ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/semantic-ui/translations/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.412006 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/semantic-ui/translations/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.404006 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.412006 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.404006 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.412006 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/LC_MESSAGES/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/semantic-ui/translations/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.412006 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.404006 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.412006 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.404006 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.412006 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.412006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.412006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.408006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.408006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.408006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/CommunityTypeLabel.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/ComputerTabletCommunitiesListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/MobileCommunitiesListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/RestrictedLabel.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/templates/DashboardCommunitiesPage.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.408006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.408006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupValueToggler.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/custom-components.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/templates/Header.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_records/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.408006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_records/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.408006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.408006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_records/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_records/templates/DashboardRecordsPage.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_records/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.408006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.408006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.408006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/ComputerTabletRequestsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/MobileRequestsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/RequestTypeSpecificComponents.jsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/icons/TypeIcons.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/TypeLabels.jsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.416006 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/templates/DashboardRequestsPage.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:16:58.420006 oarepo-dashboard-1.0.2/oarepo_dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 08:16:58.000000 oarepo-dashboard-1.0.2/oarepo_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-02 08:16:58.000000 oarepo-dashboard-1.0.2/oarepo_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:16:58.000000 oarepo-dashboard-1.0.2/oarepo_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-02 08:16:58.000000 oarepo-dashboard-1.0.2/oarepo_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 08:16:58.000000 oarepo-dashboard-1.0.2/oarepo_dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 08:16:58.000000 oarepo-dashboard-1.0.2/oarepo_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-02 08:16:58.420006 oarepo-dashboard-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 08:15:06.000000 oarepo-dashboard-1.0.2/setup.py
```

### Comparing `oarepo-dashboard-1.0.1/PKG-INFO` & `oarepo-dashboard-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-dashboard
-Version: 1.0.1
+Version: 1.0.2
 Summary: Support for user dashboard (records, communities, requests)
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
 Requires-Dist: cachetools
 Provides-Extra: dev
```

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/semantic-ui/translations/i18next.js` & `oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/semantic-ui/translations/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/translations.json` & `oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.mo` & `oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.po` & `oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.po` & `oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/i18n/translations/messages.pot` & `oarepo-dashboard-1.0.2/oarepo_dashboard/i18n/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/__init__.py` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/CommunityTypeLabel.jsx` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/CommunityTypeLabel.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/ComputerTabletCommunitiesListItem.jsx` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/ComputerTabletCommunitiesListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/MobileCommunitiesListItem.jsx` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/MobileCommunitiesListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/index.js` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/index.js`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupValueToggler.jsx` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupValueToggler.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_components/webpack.py` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_components/webpack.py`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_records/__init__.py` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_records/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from oarepo_ui.resources.config import (
     RecordsUIResourceConfig,
 )
 from oarepo_ui.resources.resource import RecordsUIResource
 from flask_menu import current_menu
+from flask_login import current_user
 from oarepo_runtime.i18n import lazy_gettext as _
 
 
 class DashboardRecordsUIResourceConfig(RecordsUIResourceConfig):
     url_prefix = "/me/records/"
     blueprint_name = "records_dashboard"
     template_folder = "templates"
@@ -36,14 +37,17 @@
     """Register blueprint for this resource."""
     app_blueprint = DashboardRecordsUIResource(
         DashboardRecordsUIResourceConfig()
     ).as_blueprint()
 
     @app_blueprint.before_app_first_request
     def init_menu():
+        if not current_user.is_authenticated:
+            return
+
         user_dashboard = current_menu.submenu("user_dashboard")
         user_dashboard.submenu("records").register(
             "records_dashboard.search",
             text=_("Records"),
             order=1,
         )
```

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/index.js` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/index.js`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/__init__.py` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/ComputerTabletRequestsListItem.jsx` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/ComputerTabletRequestsListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/MobileRequestsListItem.jsx` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/MobileRequestsListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/RequestTypeSpecificComponents.jsx` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/RequestTypeSpecificComponents.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/index.js` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/index.js`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/TypeLabels.jsx` & `oarepo-dashboard-1.0.2/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/TypeLabels.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard.egg-info/PKG-INFO` & `oarepo-dashboard-1.0.2/oarepo_dashboard.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-dashboard
-Version: 1.0.1
+Version: 1.0.2
 Summary: Support for user dashboard (records, communities, requests)
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
 Requires-Dist: cachetools
 Provides-Extra: dev
```

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard.egg-info/SOURCES.txt` & `oarepo-dashboard-1.0.2/oarepo_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/oarepo_dashboard.egg-info/entry_points.txt` & `oarepo-dashboard-1.0.2/oarepo_dashboard.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.1/setup.cfg` & `oarepo-dashboard-1.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-dashboard
-version = 1.0.1
+version = 1.0.2
 description = Support for user dashboard (records, communities, requests)
 authors = Mirek Simek <miroslav.simek@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

