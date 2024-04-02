# Comparing `tmp/python-gerrit-api-3.0.6.tar.gz` & `tmp/python-gerrit-api-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gerrit-api-3.0.6.tar", last modified: Tue Oct 24 07:51:16 2023, max compression
+gzip compressed data, was "python-gerrit-api-3.0.7.tar", last modified: Tue Apr  2 06:01:25 2024, max compression
```

## Comparing `python-gerrit-api-3.0.6.tar` & `python-gerrit-api-3.0.7.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 07:51:16.650528 python-gerrit-api-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12100 2023-10-24 07:51:16.650528 python-gerrit-api-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11119 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 07:51:16.642528 python-gerrit-api-3.0.6/gerrit/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 07:51:16.642528 python-gerrit-api-3.0.6/gerrit/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18261 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/accounts/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/accounts/emails.py
--rw-r--r--   0 runner    (1001) docker     (127)     5056 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/accounts/gpg_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/accounts/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 07:51:16.646528 python-gerrit-api-3.0.6/gerrit/changes/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/changes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27586 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/changes/change.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/changes/changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/changes/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/changes/drafts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/changes/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/changes/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/changes/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/changes/reviewers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12840 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/changes/revision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 07:51:16.646528 python-gerrit-api-3.0.6/gerrit/config/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/config/caches.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/config/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 07:51:16.646528 python-gerrit-api-3.0.6/gerrit/groups/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/groups/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/groups/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/groups/members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/groups/subgroups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 07:51:16.646528 python-gerrit-api-3.0.6/gerrit/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/plugins/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 07:51:16.646528 python-gerrit-api-3.0.6/gerrit/projects/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/projects/branches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/projects/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/projects/dashboards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/projects/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    14131 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/projects/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/projects/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/projects/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/projects/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 07:51:16.646528 python-gerrit-api-3.0.6/gerrit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/utils/gerritbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gerrit/utils/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 07:51:16.650528 python-gerrit-api-3.0.6/gitiles/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gitiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/gitiles/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 07:51:16.650528 python-gerrit-api-3.0.6/python_gerrit_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12100 2023-10-24 07:51:16.000000 python-gerrit-api-3.0.6/python_gerrit_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-10-24 07:51:16.000000 python-gerrit-api-3.0.6/python_gerrit_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 07:51:16.000000 python-gerrit-api-3.0.6/python_gerrit_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-24 07:51:16.000000 python-gerrit-api-3.0.6/python_gerrit_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-24 07:51:16.000000 python-gerrit-api-3.0.6/python_gerrit_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-24 07:51:16.650528 python-gerrit-api-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 07:51:16.650528 python-gerrit-api-3.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7679 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/tests/test_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/tests/test_gitiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11533 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2023-10-24 07:51:02.000000 python-gerrit-api-3.0.6/tests/test_revision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.883339 python-gerrit-api-3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-04-02 06:01:25.883339 python-gerrit-api-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11119 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.875339 python-gerrit-api-3.0.7/gerrit/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.875339 python-gerrit-api-3.0.7/gerrit/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18444 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/accounts/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/accounts/emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/accounts/gpg_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/accounts/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.875339 python-gerrit-api-3.0.7/gerrit/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27591 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/change.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/revision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.879339 python-gerrit-api-3.0.7/gerrit/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/config/caches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/config/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.879339 python-gerrit-api-3.0.7/gerrit/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/groups/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/groups/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/groups/members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/groups/subgroups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.879339 python-gerrit-api-3.0.7/gerrit/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/plugins/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.879339 python-gerrit-api-3.0.7/gerrit/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.883339 python-gerrit-api-3.0.7/gerrit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/utils/gerritbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/utils/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.883339 python-gerrit-api-3.0.7/gitiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gitiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gitiles/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.883339 python-gerrit-api-3.0.7/python_gerrit_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-04-02 06:01:25.000000 python-gerrit-api-3.0.7/python_gerrit_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-02 06:01:25.000000 python-gerrit-api-3.0.7/python_gerrit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:01:25.000000 python-gerrit-api-3.0.7/python_gerrit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 06:01:25.000000 python-gerrit-api-3.0.7/python_gerrit_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 06:01:25.000000 python-gerrit-api-3.0.7/python_gerrit_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 06:01:25.887339 python-gerrit-api-3.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.883339 python-gerrit-api-3.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/tests/test_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/tests/test_gitiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11540 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/tests/test_revision.py
```

### Comparing `python-gerrit-api-3.0.6/LICENSE` & `python-gerrit-api-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.6/PKG-INFO` & `python-gerrit-api-3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 3.0.6
+Version: 3.0.7
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 License-File: LICENSE
 Requires-Dist: requests
-Requires-Dist: six>=1.10.0
 
 Project description
 ===================
 
 .. image:: https://img.shields.io/pypi/pyversions/python-gerrit-api.svg
     :target: https://pypi.python.org/pypi/python-gerrit-api
 .. image:: https://img.shields.io/pypi/v/python-gerrit-api.svg
```

### Comparing `python-gerrit-api-3.0.6/README.rst` & `python-gerrit-api-3.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.6/gerrit/accounts/account.py` & `python-gerrit-api-3.0.7/gerrit/accounts/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,16 +50,17 @@
             result = account.set_name(input_)
 
 
         :param input_: the AccountNameInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#account-name-input
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/name",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/name", json=input_, headers=self.gerrit.default_headers
+        )
 
     def delete_name(self):
         """
         Deletes the name of an account.
         Some realms may not allow to delete the account name.
         In this case the request is rejected with '405 Method Not Allowed'.
 
@@ -83,16 +84,17 @@
         """
         Sets the status of an account.
 
         :param status: account status
         :return:
         """
         input_ = {"status": status}
-        return self.gerrit.put(self.endpoint + "/status",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/status", json=input_, headers=self.gerrit.default_headers
+        )
 
     def set_username(self, input_):
         """
         Sets the username of an account.
         Some realms may not allow to modify the account username.
         In this case the request is rejected with '405 Method Not Allowed'.
 
@@ -105,16 +107,19 @@
             account = client.accounts.get('kevin.shi')
             result = account.set_username(input_)
 
         :param input_: the UsernameInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#username-input
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/username",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/username",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def set_displayname(self, input_):
         """
         Sets the display name of an account.
         support this method since v3.2.0
 
         .. code-block:: python
@@ -126,16 +131,19 @@
             account = client.accounts.get('kevin.shi')
             result = account.set_displayname(input_)
 
         :param input_: the DisplayNameInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#display-name-input
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/displayname",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/displayname",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def get_active(self):
         """
         Checks if an account is active.
 
         :return:
         """
@@ -172,16 +180,19 @@
             account = client.accounts.get('kevin.shi')
             result = account.set_http_password(input_)
 
         :param input_: the HttpPasswordInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#http-password-input
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/password.http",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/password.http",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def delete_http_password(self):
         """
         Deletes the HTTP password of an account.
 
         :return:
         """
@@ -284,16 +295,19 @@
             account = client.accounts.get('kevin.shi')
             result = account.set_user_preferences(input_)
 
         :param input_: the PreferencesInput entity，
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#preferences-input
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/preferences",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/preferences",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def get_diff_preferences(self):
         """
         Retrieves the diff preferences of a user.
 
         :return:
         """
@@ -323,16 +337,19 @@
             account = client.accounts.get('kevin.shi')
             result = account.set_diff_preferences(input_)
 
         :param input_: the DiffPreferencesInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#diff-preferences-input
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/preferences.diff",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/preferences.diff",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def get_edit_preferences(self):
         """
         Retrieves the edit preferences of a user.
 
         :return:
         """
@@ -364,16 +381,19 @@
             account = client.accounts.get('kevin.shi')
             result = account.set_edit_preferences(input_)
 
         :param input_: the EditPreferencesInfo entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#edit-preferences-info
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/preferences.edit",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/preferences.edit",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def get_watched_projects(self):
         """
         Retrieves all projects a user is watching.
 
         :return:
         """
@@ -397,16 +417,19 @@
 
             account = client.accounts.get('kevin.shi')
             result = account.modify_watched_projects(input_)
 
         :param input_: the ProjectWatchInfo entities as list
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/watched.projects",
-                                json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/watched.projects",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def delete_watched_projects(self, input_):
         """
         Projects posted to this endpoint will no longer be watched.
 
         .. code-block:: python
 
@@ -419,16 +442,19 @@
 
             account = client.accounts.get('kevin.shi')
             result = account.delete_watched_projects(input_)
 
         :param input_: the watched projects as list
         :return:
         """
-        self.gerrit.post(self.endpoint + "/watched.projects:delete",
-                         json=input_, headers=self.gerrit.default_headers)
+        self.gerrit.post(
+            self.endpoint + "/watched.projects:delete",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def get_external_ids(self):
         """
         Retrieves the external ids of a user account.
         Only external ids belonging to the caller may be requested.
         Users that have Modify Account can request external
         ids that belong to other accounts.
@@ -451,16 +477,19 @@
 
             account = client.accounts.get('kevin.shi')
             result = account.delete_external_ids(input_)
 
         :param input_: the external ids as list
         :return:
         """
-        self.gerrit.post(self.endpoint + "/external.ids:delete",
-                         json=input_, headers=self.gerrit.default_headers)
+        self.gerrit.post(
+            self.endpoint + "/external.ids:delete",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def list_contributor_agreements(self):
         """
         Gets a list of the user’s signed contributor agreements.
 
         :return:
         """
@@ -478,16 +507,19 @@
             account = client.accounts.get('kevin.shi')
             result = account.sign_contributor_agreement(input_)
 
         :param input_: the ContributorAgreementInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#contributor-agreement-input
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/agreements",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/agreements",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def delete_draft_comments(self, input_):
         """
         Deletes some or all of a user’s draft comments.
 
         .. code-block:: python
 
@@ -497,16 +529,19 @@
             account = client.accounts.get('kevin.shi')
             result = account.delete_draft_comments(input_)
 
         :param input_: the DeleteDraftCommentsInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#delete-draft-comments-input
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/drafts:delete",
-                                json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/drafts:delete",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def index(self):
         """
         Adds or updates the account in the secondary index.
 
         :return:
         """
@@ -574,9 +609,12 @@
 
 
         :param id_: change id
         :param input_: the StarsInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#stars-input
         :return:
         """
-        return self.gerrit.post(self.endpoint + f"/stars.changes/{id_}",
-                                json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + f"/stars.changes/{id_}",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
```

### Comparing `python-gerrit-api-3.0.6/gerrit/accounts/accounts.py` & `python-gerrit-api-3.0.7/gerrit/accounts/accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Author: Jialiang Shi
 import logging
 import requests
 from gerrit.accounts.account import GerritAccount
 from gerrit.utils.exceptions import (
     AccountNotFoundError,
     AccountAlreadyExistsError,
-    GerritAPIException
+    GerritAPIException,
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 class GerritAccounts:
@@ -106,9 +106,12 @@
         try:
             self.get(username)
             message = f"Account {username} already exists"
             logger.error(message)
             raise AccountAlreadyExistsError(message)
         except AccountNotFoundError:
             self.gerrit.put(
-                self.endpoint + f"/{username}", json=input_, headers=self.gerrit.default_headers)
+                self.endpoint + f"/{username}",
+                json=input_,
+                headers=self.gerrit.default_headers,
+            )
             return self.get(username)
```

### Comparing `python-gerrit-api-3.0.6/gerrit/accounts/emails.py` & `python-gerrit-api-3.0.7/gerrit/accounts/emails.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Author: Jialiang Shi
 import logging
 import requests
 from gerrit.utils.gerritbase import GerritBase
 from gerrit.utils.exceptions import (
     AccountEmailNotFoundError,
     AccountEmailAlreadyExistsError,
-    GerritAPIException
+    GerritAPIException,
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 class GerritAccountEmail(GerritBase):
@@ -78,15 +78,17 @@
 
         :return:
         """
         try:
             result = self.gerrit.get(self.endpoint + f"/{email}")
 
             email_ = result.get("email")
-            return GerritAccountEmail(email=email_, account=self.account, gerrit=self.gerrit)
+            return GerritAccountEmail(
+                email=email_, account=self.account, gerrit=self.gerrit
+            )
         except requests.exceptions.HTTPError as error:
             if error.response.status_code == 404:
                 message = f"Account Email {email} does not exist"
                 raise AccountEmailNotFoundError(message)
             raise GerritAPIException from error
 
     def set_preferred(self, email):
```

### Comparing `python-gerrit-api-3.0.6/gerrit/accounts/gpg_keys.py` & `python-gerrit-api-3.0.7/gerrit/accounts/gpg_keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 import logging
 import requests
 from gerrit.utils.gerritbase import GerritBase
-from gerrit.utils.exceptions import (
-    GPGKeyNotFoundError,
-    GerritAPIException
-)
+from gerrit.utils.exceptions import GPGKeyNotFoundError, GerritAPIException
 
 logger = logging.getLogger(__name__)
 
 
 class GerritAccountGPGKey(GerritBase):
     def __init__(self, id, account, gerrit):
         self.id = id
@@ -116,15 +113,17 @@
             account = client.accounts.get('kevin.shi')
             result = account.gpg_keys.modify(input_)
 
         :param input_: the GpgKeysInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#gpg-keys-input
         :return:
         """
-        return self.gerrit.post(self.endpoint, json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint, json=input_, headers=self.gerrit.default_headers
+        )
 
     def delete(self, id_):
         """
         Deletes a GPG key of a user.
 
         :param id_: GPG key id
         :return:
```

### Comparing `python-gerrit-api-3.0.6/gerrit/accounts/ssh_keys.py` & `python-gerrit-api-3.0.7/gerrit/accounts/ssh_keys.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 import logging
 import requests
 from gerrit.utils.gerritbase import GerritBase
-from gerrit.utils.exceptions import (
-    SSHKeyNotFoundError,
-    GerritAPIException
-)
+from gerrit.utils.exceptions import SSHKeyNotFoundError, GerritAPIException
 
 logger = logging.getLogger(__name__)
 
 
 class GerritAccountSSHKey(GerritBase):
     def __init__(self, seq, account, gerrit):
         self.seq = seq
@@ -54,31 +51,34 @@
         :param seq: SSH key id
         :return:
         """
         try:
             result = self.gerrit.get(self.endpoint + f"/{str(seq)}")
 
             seq = result.get("seq")
-            return GerritAccountSSHKey(seq=seq, account=self.account, gerrit=self.gerrit)
+            return GerritAccountSSHKey(
+                seq=seq, account=self.account, gerrit=self.gerrit
+            )
         except requests.exceptions.HTTPError as error:
             if error.response.status_code == 404:
                 message = f"SSH key {seq} does not exist"
                 raise SSHKeyNotFoundError(message)
             raise GerritAPIException from error
 
     def add(self, ssh_key):
         """
         Adds an SSH key for a user.
         The SSH public key must be provided as raw content in the request body.
 
         :param ssh_key: SSH key raw content
         :return:
         """
-        result = self.gerrit.post(self.endpoint,
-                                  data=ssh_key, headers={"Content-Type": "plain/text"})
+        result = self.gerrit.post(
+            self.endpoint, data=ssh_key, headers={"Content-Type": "plain/text"}
+        )
         return result
 
     def delete(self, seq):
         """
         Deletes an SSH key of a user.
 
         :param seq: SSH key id
```

### Comparing `python-gerrit-api-3.0.6/gerrit/base.py` & `python-gerrit-api-3.0.7/gerrit/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 import netrc
 from gerrit.utils.requester import Requester
-from gerrit.utils.common import (
-    decode_response,
-    strip_trailing_slash
-)
+from gerrit.utils.common import decode_response, strip_trailing_slash
 from gerrit.config.config import GerritConfig
 from gerrit.projects.projects import GerritProjects
 from gerrit.accounts.accounts import GerritAccounts
 from gerrit.groups.groups import GerritGroups
 from gerrit.plugins.plugins import GerritPlugins
 from gerrit.changes.changes import GerritChanges
 
@@ -29,15 +26,15 @@
         username=None,
         password=None,
         use_netrc=False,
         ssl_verify=True,
         cert=None,
         timeout=60,
         max_retries=None,
-        auth_suffix="/a"
+        auth_suffix="/a",
     ):
         self._base_url = strip_trailing_slash(base_url)
 
         if use_netrc:
             password = self.get_password_from_netrc_file()
 
         self.requester = Requester(
@@ -59,15 +56,17 @@
         Providing the password form .netrc file for getting Host name.
         :return: The related password from .netrc file as a string.
         """
 
         netrc_client = netrc.netrc()
         auth_tokens = netrc_client.authenticators(self._base_url)
         if not auth_tokens:
-            raise ValueError(f"The '{self._base_url}' host name is not found in netrc file.")
+            raise ValueError(
+                f"The '{self._base_url}' host name is not found in netrc file."
+            )
         return auth_tokens[2]
 
     def get_endpoint_url(self, endpoint):
         """
         Return the complete url including host and port for a given endpoint.
         :param endpoint: service endpoint as str
         :return: complete url (including host and port) as str
```

### Comparing `python-gerrit-api-3.0.6/gerrit/changes/change.py` & `python-gerrit-api-3.0.7/gerrit/changes/change.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,17 @@
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             result = change.update(input_)
 
         :param input_: the MergePatchSetInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#merge-patch-set-input
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/merge",
-                                json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/merge", json=input_, headers=self.gerrit.default_headers
+        )
 
     def set_commit_message(self, input_):
         """
         Creates a new patch set with a new commit message.
 
         .. code-block:: python
 
@@ -96,16 +97,17 @@
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             result = change.set_commit_message(input_)
 
         :param input_: the CommitMessageInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#commit-message-input
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/message",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/message", json=input_, headers=self.gerrit.default_headers
+        )
 
     def list_votes(self, account):
         """
         Lists the votes for a specific reviewer of the change.
 
         :param account: account id or username
         :return:
@@ -159,16 +161,17 @@
         """
         Sets the topic of a change.
 
         :param topic: The new topic
         :return:
         """
         input_ = {"topic": topic}
-        return self.gerrit.put(self.endpoint + "/topic",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/topic", json=input_, headers=self.gerrit.default_headers
+        )
 
     def delete_topic(self):
         """
         Deletes the topic of a change.
 
         :return:
         """
@@ -195,16 +198,19 @@
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             result = change.set_assignee(input_)
 
         :param input_: the AssigneeInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#assignee-input
         :return:
         """
-        result = self.gerrit.put(self.endpoint + "/assignee",
-                                 json=input_, headers=self.gerrit.default_headers)
+        result = self.gerrit.put(
+            self.endpoint + "/assignee",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
         return result
 
     def get_past_assignees(self):
         """
         Returns a list of every user ever assigned to a change, in the order in which they were
         first assigned.
 
@@ -268,16 +274,17 @@
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             result = change.rebase(input_)
 
         :param input_: the RebaseInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#rebase-input
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/rebase",
-                                json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/rebase", json=input_, headers=self.gerrit.default_headers
+        )
 
     def move(self, input_):
         """
         Move a change.
         If the change cannot be moved because the change state doesn't allow moving the change,
         the response is '409 Conflict' and the error message is contained in the response body.
 
@@ -290,17 +297,17 @@
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             result = change.move(input_)
 
         :param input_: the MoveInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#move-input
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/move",
-                                json=input_,
-                                headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/move", json=input_, headers=self.gerrit.default_headers
+        )
 
     def revert(self, input_=None):
         """
         Reverts a change.
         The request body does not need to include a RevertInput entity if no review comment is
         added.
 
@@ -324,16 +331,19 @@
             # or
             result = change.revert(input_)
 
         :param input_: the RevertInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#revert-input
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/revert",
-                                json=input_ or {}, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/revert",
+            json=input_ or {},
+            headers=self.gerrit.default_headers,
+        )
 
     def revert_submission(self):
         """
         Creates open revert changes for all of the changes of a certain submission.
 
         If the user doesn't have revert permission on the change or upload permission on the
         destination, the response is '403 Forbidden', and the error message is contained in the
@@ -368,25 +378,28 @@
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#submit-input
         :return:
         """
         endpoint = self.endpoint + "/submit"
         if input_ is None:
             result = self.gerrit.post(endpoint)
         else:
-            result = self.gerrit.post(endpoint,
-                                      json=input_, headers=self.gerrit.default_headers)
+            result = self.gerrit.post(
+                endpoint, json=input_, headers=self.gerrit.default_headers
+            )
         return result
 
     def list_submitted_together_changes(self):
         """
         Computes list of all changes which are submitted when Submit is called for this change,
         including the current change itself.
 
         """
-        return self.gerrit.get(self.endpoint + "/submitted_together?o=NON_VISIBLE_CHANGES")
+        return self.gerrit.get(
+            self.endpoint + "/submitted_together?o=NON_VISIBLE_CHANGES"
+        )
 
     def delete(self):
         """
         Deletes a change.
 
         :return:
         """
@@ -465,15 +478,17 @@
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#fix-input
         :return:
         """
         endpoint = self.endpoint + "/check"
         if input_ is None:
             result = self.gerrit.post(endpoint)
         else:
-            result = self.gerrit.post(endpoint, json=input_, headers=self.gerrit.default_headers)
+            result = self.gerrit.post(
+                endpoint, json=input_, headers=self.gerrit.default_headers
+            )
         return result
 
     def set_work_in_progress(self, input_=None):
         """
         Marks the change as not ready for review yet.
         Changes may only be marked not ready by the owner, project owners or site administrators.
         Marking a change work in progress also removes all users from the attention set.
@@ -492,17 +507,19 @@
             # or
             result = change.set_work_in_progress()
 
         :param input_: the WorkInProgressInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#work-in-progress-input
         :return:
         """
-        self.gerrit.post(self.endpoint + "/wip",
-                         json=input_ or {}, headers=self.gerrit.default_headers
-                         )
+        self.gerrit.post(
+            self.endpoint + "/wip",
+            json=input_ or {},
+            headers=self.gerrit.default_headers,
+        )
 
     def set_ready_for_review(self, input_):
         """
         Marks the change as ready for review (set WIP property to false).
         Changes may only be marked ready by the owner, project owners or site administrators.
         Marking a change ready for review also adds all of the reviewers of the change to the
         attention set.
@@ -516,15 +533,17 @@
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             change.set_ready_for_review(input_)
 
         :param input_: the WorkInProgressInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#work-in-progress-input
         :return:
         """
-        self.gerrit.post(self.endpoint + "/ready", json=input_, headers=self.gerrit.default_headers)
+        self.gerrit.post(
+            self.endpoint + "/ready", json=input_, headers=self.gerrit.default_headers
+        )
 
     def mark_private(self, input_):
         """
         Marks the change to be private. Only open changes can be marked private.
         Changes may only be marked private by the owner or site administrators.
 
         .. code-block:: python
@@ -535,17 +554,17 @@
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             change.mark_private(input_)
 
         :param input_: the PrivateInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#private-input
         :return:
         """
-        self.gerrit.post(self.endpoint + "/private",
-                         json=input_, headers=self.gerrit.default_headers
-                         )
+        self.gerrit.post(
+            self.endpoint + "/private", json=input_, headers=self.gerrit.default_headers
+        )
 
     def unmark_private(self, input_=None):
         """
         Marks the change to be non-private. Note users can only unmark own private changes.
         If the change was already not private, the response is '409 Conflict'.
 
         .. code-block:: python
@@ -561,17 +580,19 @@
         :param input_: the PrivateInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#private-input
         :return:
         """
         if input_ is None:
             self.gerrit.delete(self.endpoint + "/private")
         else:
-            self.gerrit.post(self.endpoint + "/private.delete",
-                             json=input_, headers=self.gerrit.default_headers
-                             )
+            self.gerrit.post(
+                self.endpoint + "/private.delete",
+                json=input_,
+                headers=self.gerrit.default_headers,
+            )
 
     def ignore(self):
         """
         Marks a change as ignored. The change will not be shown in the incoming reviews' dashboard,
         and email notifications will be suppressed. Ignoring a change does not cause the change’s
         "updated" timestamp to be modified, and the owner is not notified.
 
@@ -628,31 +649,37 @@
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             result = change.set_hashtags(input_)
 
         :param input_: the HashtagsInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#hashtags-input
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/hashtags",
-                                json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/hashtags",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     @property
     def messages(self):
         return GerritChangeMessages(change=self.id, gerrit=self.gerrit)
 
     def check_submit_requirement(self, input_):
         """
         Tests a submit requirement.
 
         :param input_: the SubmitRequirementInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#submit-requirement-input
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/check.submit_requirement",
-                                json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/check.submit_requirement",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def get_edit(self):
         """
         Retrieves a change edit details.
         As response an EditInfo entity is returned that describes the change edit,
         or 204 No Content when change edit doesn't exist for this change.
 
@@ -720,17 +747,15 @@
             if revision_id <= 0:
                 revision_id = self.current_revision_number + revision_id
             revision_id = self.__revision_number_to_sha(revision_id)
             if revision_id is None:
                 return None
 
         return GerritChangeRevision(
-            gerrit=self.gerrit,
-            change=self.id,
-            revision=revision_id
+            gerrit=self.gerrit, change=self.id, revision=revision_id
         )
 
     def get_attention_set(self):
         """
         Returns all users that are currently in the attention set.
         support this method since v3.3.0
 
@@ -755,16 +780,19 @@
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             result = change.add_to_attention_set(input_)
 
         :param input_: the AttentionSetInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#attention-set-input
         :return:
         """
-        result = self.gerrit.post(self.endpoint + "/attention",
-                                  json=input_, headers=self.gerrit.default_headers)
+        result = self.gerrit.post(
+            self.endpoint + "/attention",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
         return result
 
     def remove_from_attention_set(self, id_, input_=None):
         """
         Deletes a single user from the attention set of a change.
         support this method since v3.3.0
```

### Comparing `python-gerrit-api-3.0.6/gerrit/changes/changes.py` & `python-gerrit-api-3.0.7/gerrit/changes/changes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 import logging
 import requests
 from gerrit.changes.change import GerritChange
-from gerrit.utils.exceptions import (
-    ChangeNotFoundError,
-    GerritAPIException
-)
+from gerrit.utils.exceptions import ChangeNotFoundError, GerritAPIException
 
 
 logger = logging.getLogger(__name__)
 
 
 class GerritChanges:
     def __init__(self, gerrit):
@@ -90,15 +87,17 @@
         :return:
         """
         project_name = input_.get("project")
         branch_name = input_.get("branch")
         project = self.gerrit.projects.get(project_name)
         project.branches.get(branch_name)
 
-        result = self.gerrit.post(self.endpoint + '/', json=input_, headers=self.gerrit.default_headers)
+        result = self.gerrit.post(
+            self.endpoint + "/", json=input_, headers=self.gerrit.default_headers
+        )
         return result
 
     def delete(self, id_):
         """
         Deletes a change.
 
         :param id_: change id
```

### Comparing `python-gerrit-api-3.0.6/gerrit/changes/comments.py` & `python-gerrit-api-3.0.7/gerrit/changes/comments.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 class GerritChangeRevisionComment(GerritBase):
     def __init__(self, id: str, change: str, revision: str, gerrit):
         self.id = id
         self.change = change
         self.revision = revision
         self.gerrit = gerrit
-        self.endpoint = f"/changes/{self.change}/revisions/{self.revision}/comments/{self.id}"
+        self.endpoint = (
+            f"/changes/{self.change}/revisions/{self.revision}/comments/{self.id}"
+        )
         super().__init__(self)
 
     def __str__(self):
         return self.id
 
     def delete(self, input_=None):
         """
@@ -38,16 +40,19 @@
         :param input_: the DeleteCommentInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-comment-input
         :return:
         """
         if input_ is None:
             return self.gerrit.delete(self.endpoint)
         else:
-            return self.gerrit.post(self.endpoint + "/delete",
-                                    json=input_, headers=self.gerrit.default_headers)
+            return self.gerrit.post(
+                self.endpoint + "/delete",
+                json=input_,
+                headers=self.gerrit.default_headers,
+            )
 
 
 class GerritChangeRevisionComments:
     def __init__(self, change, revision, gerrit):
         self.change = change
         self.revision = revision
         self.gerrit = gerrit
```

### Comparing `python-gerrit-api-3.0.6/gerrit/changes/drafts.py` & `python-gerrit-api-3.0.7/gerrit/changes/drafts.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 class GerritChangeRevisionDraft(GerritBase):
     def __init__(self, id: str, change: str, revision: str, gerrit):
         self.id = id
         self.change = change
         self.revision = revision
         self.gerrit = gerrit
-        self.endpoint = f"/changes/{self.change}/revisions/{self.revision}/drafts/{self.id}"
+        self.endpoint = (
+            f"/changes/{self.change}/revisions/{self.revision}/drafts/{self.id}"
+        )
         super().__init__(self)
 
     def __str__(self):
         return self.id
 
     def update(self, input_):
         """
@@ -32,15 +34,17 @@
             draft = revision.drafts.get('89f04e8c_9b7fd51d')
             result = draft.update(input_)
 
         :param input_: the CommentInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#comment-input
         :return:
         """
-        return self.gerrit.put(self.endpoint, json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint, json=input_, headers=self.gerrit.default_headers
+        )
 
     def delete(self):
         """
         Deletes a draft comment from a revision.
 
         :return:
         """
@@ -99,15 +103,17 @@
             revision = change.get_revision('3848807f587dbd3a7e61723bbfbf1ad13ad5a00a')
             new_draft = revision.drafts.create(input_)
 
         :param input_: the CommentInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#comment-input
         :return:
         """
-        result = self.gerrit.put(self.endpoint, json=input_, headers=self.gerrit.default_headers)
+        result = self.gerrit.put(
+            self.endpoint, json=input_, headers=self.gerrit.default_headers
+        )
         return result
 
     def delete(self, id_):
         """
         Deletes a draft comment from a revision.
 
         :param id_: the draft comment id
```

### Comparing `python-gerrit-api-3.0.6/gerrit/changes/edit.py` & `python-gerrit-api-3.0.7/gerrit/changes/edit.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,37 +39,44 @@
         """
         Put content of a file to a change edit.
 
         :param file: the file path
         :param file_content: the content of the file need to change
         :return:
         """
-        self.gerrit.put(self.endpoint + f"/{quote_plus(file)}",
-                        data=file_content, headers={"Content-Type": "plain/text"})
+        self.gerrit.put(
+            self.endpoint + f"/{quote_plus(file)}",
+            data=file_content,
+            headers={"Content-Type": "plain/text"},
+        )
 
     def restore_file_content(self, file):
         """
         restores file content
 
         :param file: Path to file to restore.
         :return:
         """
         input_ = {"restore_path": file}
-        self.gerrit.post(self.endpoint, json=input_, headers=self.gerrit.default_headers)
+        self.gerrit.post(
+            self.endpoint, json=input_, headers=self.gerrit.default_headers
+        )
 
     def rename_file(self, old_path, new_path):
         """
         rename file
 
         :param old_path: Old path to file to rename.
         :param new_path: New path to file to rename.
         :return:
         """
         input_ = {"old_path": old_path, "new_path": new_path}
-        self.gerrit.post(self.endpoint, json=input_, headers=self.gerrit.default_headers)
+        self.gerrit.post(
+            self.endpoint, json=input_, headers=self.gerrit.default_headers
+        )
 
     def delete_file(self, file):
         """
         Deletes a file from a change edit.
 
         :param file: Path to file to delete.
         :return:
@@ -91,16 +98,17 @@
             edit = change.get_edit()
             edit.change_commit_message(input_)
 
         :param input_: the ChangeEditMessageInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#change-edit-message-input
         :return:
         """
-        self.gerrit.put(self.endpoint + ":message",
-                        json=input_, headers=self.gerrit.default_headers)
+        self.gerrit.put(
+            self.endpoint + ":message", json=input_, headers=self.gerrit.default_headers
+        )
 
     def get_commit_message(self):
         """
         Retrieves commit message from change edit.
         The commit message is returned as base64 encoded string.
 
         :return:
@@ -121,16 +129,17 @@
             edit = change.get_edit()
             edit.publish(input_)
 
         :param input_: the PublishChangeEditInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#publish-change-edit-input
         :return:
         """
-        self.gerrit.post(self.endpoint + ":publish",
-                         json=input_, headers=self.gerrit.default_headers)
+        self.gerrit.post(
+            self.endpoint + ":publish", json=input_, headers=self.gerrit.default_headers
+        )
 
     def rebase(self):
         """
         Rebase change edit on top of the latest patch set.
         When change was rebased on top of the latest patch set, response '204 No Content'
         is returned.
         When change edit is already based on top of the latest patch set,
```

### Comparing `python-gerrit-api-3.0.6/gerrit/changes/files.py` & `python-gerrit-api-3.0.7/gerrit/changes/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 from typing import Optional
 from base64 import b64decode
 from urllib.parse import quote_plus
 import requests
 from gerrit.utils.exceptions import (
     UnknownFile,
     FileContentNotFoundError,
-    GerritAPIException
+    GerritAPIException,
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 class GerritChangeRevisionFile:
     def __init__(self, path: str, json: dict, change: str, revision: str, gerrit):
         self.path = path
         self.json = json
         self.change = change
         self.revision = revision
         self.gerrit = gerrit
-        self.endpoint = f"/changes/{self.change}/revisions/{self.revision}" \
-                        f"/files/{quote_plus(self.path)}"
+        self.endpoint = (
+            f"/changes/{self.change}/revisions/{self.revision}"
+            f"/files/{quote_plus(self.path)}"
+        )
 
     def __repr__(self):
         return f"<{self.__class__.__module__}.{self.__class__.__name__} {str(self)}>"
 
     def __str__(self):
         return self.path
 
@@ -112,16 +114,21 @@
     def __init__(self, change, revision, gerrit):
         self.change = change
         self.revision = revision
         self.gerrit = gerrit
         self._data = []
         self.endpoint = f"/changes/{self.change}/revisions/{self.revision}/files"
 
-    def search(self, reviewed: Optional[bool] = None, base: Optional[int] = None,
-               q: Optional[str] = None, parent: Optional[int] = None):
+    def search(
+        self,
+        reviewed: Optional[bool] = None,
+        base: Optional[int] = None,
+        q: Optional[str] = None,
+        parent: Optional[int] = None,
+    ):
         """
         Lists the files that were modified, added or deleted in a revision.
         The reviewed, base, q, and parent are mutually exclusive. That is, only one of them may be used at a time.
 
         :param reviewed: return a list of the paths the caller has marked as reviewed
         :param base: return a map of the files which are different in this commit compared to the given revision.
           The revision must correspond to a patch set in the change.
@@ -197,15 +204,19 @@
         :return:
         """
         if not self._data:
             self._data = self.poll()
 
         for file in self._data:
             yield GerritChangeRevisionFile(
-                path=file["path"], json=file, change=self.change, revision=self.revision, gerrit=self.gerrit
+                path=file["path"],
+                json=file,
+                change=self.change,
+                revision=self.revision,
+                gerrit=self.gerrit,
             )
 
     def __getitem__(self, path):
         """
         get a file by path
 
         :param path: file path
```

### Comparing `python-gerrit-api-3.0.6/gerrit/changes/messages.py` & `python-gerrit-api-3.0.7/gerrit/changes/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,19 @@
         :param input_: the DeleteChangeMessageInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-change-message-input
         :return:
         """
         if input_ is None:
             self.gerrit.delete(self.endpoint)
         else:
-            self.gerrit.post(self.endpoint + "/delete",
-                             json=input_, headers=self.gerrit.default_headers)
+            self.gerrit.post(
+                self.endpoint + "/delete",
+                json=input_,
+                headers=self.gerrit.default_headers,
+            )
 
 
 class GerritChangeMessages:
     def __init__(self, change, gerrit):
         self.change = change
         self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/messages"
```

### Comparing `python-gerrit-api-3.0.6/gerrit/changes/reviewers.py` & `python-gerrit-api-3.0.7/gerrit/changes/reviewers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Author: Jialiang Shi
 import logging
 import requests
 from gerrit.utils.gerritbase import GerritBase
 from gerrit.utils.exceptions import (
     ReviewerNotFoundError,
     ReviewerAlreadyExistsError,
-    GerritAPIException
+    GerritAPIException,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class GerritChangeReviewer(GerritBase):
     def __init__(self, account: str, change: str, gerrit):
@@ -44,16 +44,19 @@
         :param input_: the DeleteReviewerInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-reviewer-input
         :return:
         """
         if input_ is None:
             self.gerrit.delete(self.endpoint)
         else:
-            self.gerrit.post(self.endpoint + "/delete",
-                             json=input_, headers=self.gerrit.default_headers)
+            self.gerrit.post(
+                self.endpoint + "/delete",
+                json=input_,
+                headers=self.gerrit.default_headers,
+            )
 
     def list_votes(self):
         """
         Lists the votes for a specific reviewer of the change.
 
         :return:
         """
@@ -82,15 +85,17 @@
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-vote-input
         :return:
         """
         endpoint = self.endpoint + f"/votes/{label}"
         if input_ is None:
             self.gerrit.delete(endpoint)
         else:
-            self.gerrit.post(endpoint + "/delete", json=input_, headers=self.gerrit.default_headers)
+            self.gerrit.post(
+                endpoint + "/delete", json=input_, headers=self.gerrit.default_headers
+            )
 
 
 class GerritChangeReviewers:
     def __init__(self, change, gerrit):
         self.change = change
         self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/reviewers"
@@ -111,15 +116,17 @@
         :param account: _account_id, name, username or email
         :return:
         """
         try:
             result = self.gerrit.get(self.endpoint + f"/{account}")
 
             account = result[0].get("_account_id")
-            return GerritChangeReviewer(account=account, change=self.change, gerrit=self.gerrit)
+            return GerritChangeReviewer(
+                account=account, change=self.change, gerrit=self.gerrit
+            )
         except requests.exceptions.HTTPError as error:
             if error.response.status_code == 404:
                 message = f"Reviewer {account} does not exist"
                 raise ReviewerNotFoundError(message)
             raise GerritAPIException from error
 
     def add(self, input_):
@@ -150,9 +157,11 @@
         reviewer = input_.get("reviewer")
         try:
             self.get(reviewer)
             message = f"Reviewer {reviewer} already exists"
             logger.error(message)
             raise ReviewerAlreadyExistsError(message)
         except ReviewerNotFoundError:
-            self.gerrit.post(self.endpoint, json=input_, headers=self.gerrit.default_headers)
+            self.gerrit.post(
+                self.endpoint, json=input_, headers=self.gerrit.default_headers
+            )
             return self.get(reviewer)
```

### Comparing `python-gerrit-api-3.0.6/gerrit/changes/revision.py` & `python-gerrit-api-3.0.7/gerrit/changes/revision.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,16 +53,19 @@
             revision = change.get_revision('3848807f587dbd3a7e61723bbfbf1ad13ad5a00a')
             result = revision.set_description(input_)
 
         :param input_: the DescriptionInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#description-input
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/description",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/description",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def get_merge_list(self):
         """
         Returns the list of commits that are being integrated into a target branch by a merge
         commit. By default, the first parent is assumed to be uninteresting. By using the parent
         option another parent can be set as uninteresting (parents are 1-based).
 
@@ -138,16 +141,17 @@
             revision = change.get_revision('3848807f587dbd3a7e61723bbfbf1ad13ad5a00a')
             result = revision.set_review(input_)
 
         :param input_: the ReviewInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#review-input
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/review",
-                                json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/review", json=input_, headers=self.gerrit.default_headers
+        )
 
     def rebase(self, input_):
         """
         Rebases a revision.
         Optionally, the parent revision can be changed to another patch set through the RebaseInput
         entity.
 
@@ -161,16 +165,17 @@
             revision = change.get_revision('3848807f587dbd3a7e61723bbfbf1ad13ad5a00a')
             result = revision.rebase(input_)
 
         :param input_: the RebaseInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#rebase-input
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/rebase",
-                                json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/rebase", json=input_, headers=self.gerrit.default_headers
+        )
 
     def submit(self):
         """
         Submits a revision.
         If the revision cannot be submitted, e.g. because the submit rule doesn’t allow submitting
         the revision or the revision is not the current revision, the response is 409 Conflict and
         the error message is contained in the response body.
@@ -246,27 +251,33 @@
         """
         Tests the submit_type Prolog rule in the project, or the one given.
 
         :param input_: the Prolog code
         :type: str
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/test.submit_type",
-                                data=input_, headers={"Content-Type": "plain/text"})
+        return self.gerrit.post(
+            self.endpoint + "/test.submit_type",
+            data=input_,
+            headers={"Content-Type": "plain/text"},
+        )
 
     def test_submit_rule(self, input_):
         """
         Tests the submit_rule Prolog rule in the project, or the one given.
 
         :param input_: the Prolog code
         :type: str
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/test.submit_rule",
-                                data=input_, headers={"Content-Type": "plain/text"})
+        return self.gerrit.post(
+            self.endpoint + "/test.submit_rule",
+            data=input_,
+            headers={"Content-Type": "plain/text"},
+        )
 
     @property
     def drafts(self):
         return GerritChangeRevisionDrafts(
             change=self.change, revision=self.revision, gerrit=self.gerrit
         )
 
@@ -314,16 +325,19 @@
             revision = change.get_revision('3848807f587dbd3a7e61723bbfbf1ad13ad5a00a')
             result = revision.cherry_pick(input_)
 
         :param input_: the CherryPickInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#cherry-pick-commit
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/cherrypick",
-                                json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/cherrypick",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def list_reviewers(self):
         """
         Lists the reviewers of a revision.
 
         :return:
         """
```

### Comparing `python-gerrit-api-3.0.6/gerrit/config/caches.py` & `python-gerrit-api-3.0.7/gerrit/config/caches.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,10 @@
             }
             gerrit.config.caches.operation(input_)
 
         :param input_: the CacheOperationInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-config.html#cache-operation-input
         :return:
         """
-        self.gerrit.post(self.endpoint, json=input_, headers=self.gerrit.default_headers)
+        self.gerrit.post(
+            self.endpoint, json=input_, headers=self.gerrit.default_headers
+        )
```

### Comparing `python-gerrit-api-3.0.6/gerrit/config/config.py` & `python-gerrit-api-3.0.7/gerrit/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,18 @@
             result = client.config.check_consistency(input_)
 
         :param input_: the ConsistencyCheckInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-config.html#consistency-check-input
         :return:
         """
         return self.gerrit.post(
-            self.endpoint + "/check.consistency", json=input_, headers=self.gerrit.default_headers)
+            self.endpoint + "/check.consistency",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def reload_config(self):
         """
         Reloads the gerrit.config configuration.
 
         :return:
         """
@@ -67,15 +70,17 @@
             result = client.config.confirm_email(input_)
 
         :param input_: the EmailConfirmationInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-config.html#email-confirmation-input
         :return:
         """
         self.gerrit.put(
-            self.endpoint + "/email.confirm", json=input_, headers=self.gerrit.default_headers
+            self.endpoint + "/email.confirm",
+            json=input_,
+            headers=self.gerrit.default_headers,
         )
 
     @property
     def caches(self):
         return Caches(gerrit=self.gerrit)
 
     def get_summary(self, option=None):
@@ -131,15 +136,17 @@
             result = client.config.set_default_user_preferences(input_)
 
         :param input_: the PreferencesInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#preferences-input
         :return:
         """
         return self.gerrit.put(
-            self.endpoint + "/preferences", json=input_, headers=self.gerrit.default_headers
+            self.endpoint + "/preferences",
+            json=input_,
+            headers=self.gerrit.default_headers,
         )
 
     def get_default_diff_preferences(self):
         """
         Returns the default diff preferences for the server.
 
         :return:
@@ -169,15 +176,17 @@
             result = client.config.set_default_diff_preferences(input_)
 
         :param input_: the DiffPreferencesInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#diff-preferences-input
         :return:
         """
         return self.gerrit.put(
-            self.endpoint + "/preferences.diff", json=input_, headers=self.gerrit.default_headers
+            self.endpoint + "/preferences.diff",
+            json=input_,
+            headers=self.gerrit.default_headers,
         )
 
     def get_default_edit_preferences(self):
         """
         Returns the default edit preferences for the server.
 
         :return:
@@ -205,15 +214,17 @@
             result = client.config.set_default_edit_preferences(input_)
 
         :param input_: the EditPreferencesInfo entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#edit-preferences-input
         :return:
         """
         return self.gerrit.put(
-            self.endpoint + "/preferences.edit", json=input_, headers=self.gerrit.default_headers
+            self.endpoint + "/preferences.edit",
+            json=input_,
+            headers=self.gerrit.default_headers,
         )
 
     def index_changes(self, input_):
         """
         Index a set of changes
 
         .. code-block:: python
@@ -222,9 +233,11 @@
             gerrit.config.index_changes(input_)
 
         :param input_: the IndexChangesInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-config.html#index-changes-input
         :return:
         """
         self.gerrit.post(
-            self.endpoint + "/index.changes", json=input_, headers=self.gerrit.default_headers
+            self.endpoint + "/index.changes",
+            json=input_,
+            headers=self.gerrit.default_headers,
         )
```

### Comparing `python-gerrit-api-3.0.6/gerrit/config/tasks.py` & `python-gerrit-api-3.0.7/gerrit/config/tasks.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.6/gerrit/groups/group.py` & `python-gerrit-api-3.0.7/gerrit/groups/group.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,16 @@
             group = client.groups.get('0017af503a22f7b3fa6ce2cd3b551734d90701b4')
             result = group.set_name(input_)
 
         :param input_:
         :return:
         """
         return self.gerrit.put(
-            self.endpoint + "/name", json=input_, headers=self.gerrit.default_headers)
+            self.endpoint + "/name", json=input_, headers=self.gerrit.default_headers
+        )
 
     def get_description(self):
         """
         Retrieves the description of a group.
 
         :return:
         """
@@ -75,15 +76,18 @@
             group = client.groups.get('0017af503a22f7b3fa6ce2cd3b551734d90701b4')
             result = group.set_description(input_)
 
         :param input_:
         :return:
         """
         return self.gerrit.put(
-            self.endpoint + "/description", json=input_, headers=self.gerrit.default_headers)
+            self.endpoint + "/description",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def delete_description(self):
         """
         Deletes the description of a Gerrit internal group.
         This endpoint is only allowed for Gerrit internal groups;
         attempting to call on a non-internal group will return 405 Method Not Allowed.
 
@@ -115,15 +119,16 @@
 
 
         :param input_: the GroupOptionsInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-groups.html#group-options-input
         :return:
         """
         return self.gerrit.put(
-            self.endpoint + "/options", json=input_, headers=self.gerrit.default_headers)
+            self.endpoint + "/options", json=input_, headers=self.gerrit.default_headers
+        )
 
     def get_owner(self):
         """
         Retrieves the owner group of a Gerrit internal group.
 
         :return: As response a GroupInfo entity is returned that describes the owner group.
         """
@@ -144,15 +149,16 @@
             result = group.set_owner(input_)
 
         :param input_: As response a GroupInfo entity is returned that describes the new owner
         group.
         :return:
         """
         return self.gerrit.put(
-            self.endpoint + "/owner", json=input_, headers=self.gerrit.default_headers)
+            self.endpoint + "/owner", json=input_, headers=self.gerrit.default_headers
+        )
 
     def get_audit_log(self):
         """
         Gets the audit log of a Gerrit internal group.
         This endpoint is only allowed for Gerrit internal groups;
         attempting to call on a non-internal group will return 405 Method Not Allowed.
```

### Comparing `python-gerrit-api-3.0.6/gerrit/groups/groups.py` & `python-gerrit-api-3.0.7/gerrit/groups/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 import logging
 import requests
 from gerrit.groups.group import GerritGroup
 from gerrit.utils.common import params_creator
 from gerrit.utils.exceptions import (
     GroupNotFoundError,
     GroupAlreadyExistsError,
-    GerritAPIException
+    GerritAPIException,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class GerritGroups:
     def __init__(self, gerrit):
         self.gerrit = gerrit
-        self.endpoint = "/groups"
+        self.endpoint = "/groups/"
 
-    def list(self, pattern_dispatcher=None, options=None, limit: int = 25, skip: int = 0):
+    def list(
+        self, pattern_dispatcher=None, options=None, limit: int = 25, skip: int = 0
+    ):
         """
         Lists the groups accessible by the caller.
 
         :param pattern_dispatcher: Dict of pattern type with respective
                      pattern value: {('match'|'regex') : value}
         :param options: Additional fields can be obtained by adding o parameters,
                         each option requires more lookups and slows down the query response time to
@@ -32,16 +34,19 @@
                           MEMBERS: include list of direct group members.
         :param limit: Int value that allows to limit the number of groups
                       to be included in the output results
         :param skip: Int value that allows to skip the given
                      number of groups from the beginning of the list
         :return:
         """
-        params = params_creator((("o", options), ("n", limit), ("S", skip)),
-                                {"match": "m", "regex": "r"}, pattern_dispatcher)
+        params = params_creator(
+            (("o", options), ("n", limit), ("S", skip)),
+            {"match": "m", "regex": "r"},
+            pattern_dispatcher,
+        )
 
         return self.gerrit.get(self.endpoint, params=params)
 
     def search(self, query, options=None, limit: int = 25, skip: int = 0):
         """
         Query Groups
 
@@ -109,9 +114,12 @@
         try:
             self.get(name)
             message = f"Group {name} already exists"
             logger.error(message)
             raise GroupAlreadyExistsError(message)
         except GroupNotFoundError:
             self.gerrit.put(
-                self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers)
+                self.endpoint + f"/{name}",
+                json=input_,
+                headers=self.gerrit.default_headers,
+            )
             return self.get(name)
```

### Comparing `python-gerrit-api-3.0.6/gerrit/groups/members.py` & `python-gerrit-api-3.0.7/gerrit/groups/members.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Author: Jialiang Shi
 import logging
 import requests
 
 from gerrit.utils.exceptions import (
     GroupMemberNotFoundError,
     GroupMemberAlreadyExistsError,
-    GerritAPIException
+    GerritAPIException,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class GerritGroupMembers:
     def __init__(self, group_id, gerrit):
```

### Comparing `python-gerrit-api-3.0.6/gerrit/groups/subgroups.py` & `python-gerrit-api-3.0.7/gerrit/groups/subgroups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.6/gerrit/plugins/plugins.py` & `python-gerrit-api-3.0.7/gerrit/plugins/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,31 +44,34 @@
         self.endpoint = "/plugins"
 
     def list(
         self,
         is_all: bool = False,
         limit: int = 25,
         skip: int = 0,
-        pattern_dispatcher=None
+        pattern_dispatcher=None,
     ):
         """
         Lists the plugins installed on the Gerrit server.
 
         :param is_all: boolean value, if True then all plugins (including
                        hidden ones) will be added to the results
         :param limit: Int value that allows to limit the number of plugins
                       to be included in the output results
         :param skip: Int value that allows to skip the given
                      number of plugins from the beginning of the list
         :param pattern_dispatcher: Dict of pattern type with respective
                      pattern value: {('prefix'|'match'|'regex') : value}
         :return:
         """
-        params = params_creator((("n", limit), ("S", skip)),
-                                {"prefix": "p", "match": "m", "regex": "r"}, pattern_dispatcher)
+        params = params_creator(
+            (("n", limit), ("S", skip)),
+            {"prefix": "p", "match": "m", "regex": "r"},
+            pattern_dispatcher,
+        )
         params["all"] = int(is_all)
 
         return self.gerrit.get(self.endpoint + "/", params=params)
 
     def get(self, id_):
         """
 
@@ -94,10 +97,12 @@
 
         :param id_: plugin id
         :param input_: the PluginInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-plugins.html#plugin-input
         :return:
         """
         result = self.gerrit.put(
-            self.endpoint + f"/{id_}.jar", json=input_, headers=self.gerrit.default_headers
+            self.endpoint + f"/{id_}.jar",
+            json=input_,
+            headers=self.gerrit.default_headers,
         )
         return result
```

### Comparing `python-gerrit-api-3.0.6/gerrit/projects/branches.py` & `python-gerrit-api-3.0.7/gerrit/projects/branches.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from urllib.parse import quote_plus, unquote_plus
 import requests
 from gerrit.utils.common import params_creator
 from gerrit.utils.gerritbase import GerritBase
 from gerrit.utils.exceptions import (
     BranchNotFoundError,
     BranchAlreadyExistsError,
-    GerritAPIException
+    GerritAPIException,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class GerritProjectBranch(GerritBase):
     def __init__(self, name: str, project: str, gerrit):
@@ -100,16 +100,19 @@
 
         :param pattern_dispatcher: Dict of pattern type with respective
                pattern value: {('match'|'regex') : value}
         :param limit: Limit the number of branches to be included in the results.
         :param skip: Skip the given number of branches from the beginning of the list.
         :return:
         """
-        params = params_creator((("n", limit), ("s", skip)),
-                                {"match": "m", "regex": "r"}, pattern_dispatcher)
+        params = params_creator(
+            (("n", limit), ("s", skip)),
+            {"match": "m", "regex": "r"},
+            pattern_dispatcher,
+        )
 
         return self.gerrit.get(self.endpoint + "/", params=params)
 
     def get(self, name):
         """
         get a branch by ref
 
@@ -117,15 +120,17 @@
         :return:
         """
         try:
             result = self.gerrit.get(self.endpoint + f"/{quote_plus(name)}")
 
             ref = result.get("ref")
             name = ref.replace(self.branch_prefix, "")
-            return GerritProjectBranch(name=name, project=self.project, gerrit=self.gerrit)
+            return GerritProjectBranch(
+                name=name, project=self.project, gerrit=self.gerrit
+            )
         except requests.exceptions.HTTPError as error:
             if error.response.status_code == 404:
                 message = f"Branch {name} does not exist"
                 raise BranchNotFoundError(message)
             raise GerritAPIException from error
 
     def create(self, name, input_):
@@ -149,15 +154,18 @@
         try:
             self.get(name)
             message = f"Branch {name} already exists"
             logger.error(message)
             raise BranchAlreadyExistsError(message)
         except BranchNotFoundError:
             self.gerrit.put(
-                self.endpoint + f"/{quote_plus(name)}", json=input_, headers=self.gerrit.default_headers)
+                self.endpoint + f"/{quote_plus(name)}",
+                json=input_,
+                headers=self.gerrit.default_headers,
+            )
 
             return self.get(name)
 
     def delete(self, name):
         """
         Delete a branch.
```

### Comparing `python-gerrit-api-3.0.6/gerrit/projects/commit.py` & `python-gerrit-api-3.0.7/gerrit/projects/commit.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,18 @@
             result = commit.cherry_pick(input_)
 
         :param input_: the CherryPickInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#cherrypick-input
         :return:  the resulting cherry-picked change
         """
         result = self.gerrit.post(
-            self.endpoint + "/cherrypick", json=input_, headers=self.gerrit.default_headers)
+            self.endpoint + "/cherrypick",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
         return result
 
     def list_change_files(self):
         """
         Lists the files that were modified, added or deleted in a commit.
 
         :return:
```

### Comparing `python-gerrit-api-3.0.6/gerrit/projects/dashboards.py` & `python-gerrit-api-3.0.7/gerrit/projects/dashboards.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,29 +55,32 @@
 
         :param id_: the dashboard id
         :param input_: the DashboardInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#dashboard-input
         :return:
         """
         result = self.gerrit.put(
-            self.endpoint + f"/{id_}", json=input_, headers=self.gerrit.default_headers)
+            self.endpoint + f"/{id_}", json=input_, headers=self.gerrit.default_headers
+        )
         return result
 
     def get(self, id_):
         """
         Retrieves a project dashboard. The dashboard can be defined on that project or be inherited
         from a parent project.
 
         :param id_: the dashboard id
         :return:
         """
         result = self.gerrit.get(self.endpoint + f"/{id_}")
 
         dashboard_id = result.get("id")
-        return GerritProjectDashboard(id=dashboard_id, project=self.project, gerrit=self.gerrit)
+        return GerritProjectDashboard(
+            id=dashboard_id, project=self.project, gerrit=self.gerrit
+        )
 
     def delete(self, id_):
         """
         Deletes a project dashboard.
 
         :param id_: the dashboard id
         :return:
```

### Comparing `python-gerrit-api-3.0.6/gerrit/projects/labels.py` & `python-gerrit-api-3.0.7/gerrit/projects/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,17 @@
             label = project.labels.get("foo")
             result = label.set(input_)
 
         :param input_: the LabelDefinitionInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#label-definition-input
         :return:
         """
-        result = self.gerrit.put(self.endpoint, json=input_, headers=self.gerrit.default_headers)
+        result = self.gerrit.put(
+            self.endpoint, json=input_, headers=self.gerrit.default_headers
+        )
         return result
 
     def delete(self):
         """
         Deletes the definition of a label that is defined in this project.
         The calling user must have write access to the refs/meta/config branch of the project.
 
@@ -100,15 +102,16 @@
 
         :param name: label name
         :param input_: the LabelDefinitionInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#label-definition-input
         :return:
         """
         result = self.gerrit.put(
-            self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers)
+            self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers
+        )
         return result
 
     def delete(self, name):
         """
         Deletes the definition of a label that is defined in this project.
         The calling user must have write access to the refs/meta/config branch of the project.
```

### Comparing `python-gerrit-api-3.0.6/gerrit/projects/project.py` & `python-gerrit-api-3.0.7/gerrit/projects/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 from gerrit.utils.gerritbase import GerritBase
 from gerrit.projects.commit import GerritProjectCommit
 from gerrit.projects.branches import GerritProjectBranches
 from gerrit.projects.tags import GerritProjectTags
 from gerrit.projects.dashboards import GerritProjectDashboards
 from gerrit.projects.labels import GerritProjectLabels
 from gerrit.projects.webhooks import GerritProjectWebHooks
-from gerrit.utils.exceptions import (
-    CommitNotFoundError,
-    GerritAPIException
-)
+from gerrit.utils.exceptions import CommitNotFoundError, GerritAPIException
 
 logger = logging.getLogger(__name__)
 
 
 class GerritProject(GerritBase):
     def __init__(self, project_id: str, gerrit):
         self.id = project_id
@@ -49,16 +46,19 @@
             project = client.projects.get('myproject')
             result = project.set_description(input_)
 
         :param input_: the ProjectDescriptionInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#project-description-input
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/description",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/description",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
 
     def delete_description(self):
         """
         Deletes the description of a project.
 
         :return:
         """
@@ -94,16 +94,17 @@
             project = client.projects.get('myproject')
             result = project.set_parent(input_)
 
         :param input_: The ProjectParentInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#project-parent-input
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/parent",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/parent", json=input_, headers=self.gerrit.default_headers
+        )
 
     def get_head(self):
         """
         Retrieves for a project the name of the branch to which HEAD points.
 
         :return:
         """
@@ -121,16 +122,17 @@
             project = client.projects.get('myproject')
             result = project.set_HEAD(input_)
 
         :param input_: The HeadInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#head-input
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/HEAD",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/HEAD", json=input_, headers=self.gerrit.default_headers
+        )
 
     def get_config(self):
         """
         Gets some configuration information about a project.
         Note that this config info is not simply the contents of project.config; it generally
         contains fields that may
         have been inherited from parent projects.
@@ -162,16 +164,17 @@
             project = client.projects.get('myproject')
             result = project.set_config(input_)
 
         :param input_: the ConfigInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#config-info
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/config",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/config", json=input_, headers=self.gerrit.default_headers
+        )
 
     def get_statistics(self):
         """
         Return statistics for the repository of a project.
 
         :return:
         """
@@ -189,16 +192,17 @@
             project = client.projects.get('myproject')
             result = project.run_garbage_collection(input_)
 
         :param input_: the GCInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#gc-input
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/gc",
-                                json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/gc", json=input_, headers=self.gerrit.default_headers
+        )
 
     def ban_commits(self, input_):
         """
         Marks commits as banned for the project.
 
         .. code-block:: python
 
@@ -212,16 +216,17 @@
             project = client.projects.get('myproject')
             result = project.ban_commits(input_)
 
         :param input_: the BanInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#ban-input
         :return:
         """
-        return self.gerrit.put(self.endpoint + "/ban",
-                               json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.put(
+            self.endpoint + "/ban", json=input_, headers=self.gerrit.default_headers
+        )
 
     def get_access_rights(self):
         """
         Lists the access rights for a single project.
 
         :return:
         """
@@ -232,16 +237,17 @@
         Sets access rights for the project using the diff schema provided by ProjectAccessInput.
         https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#set-access
 
         :param input_: the ProjectAccessInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#project-access-input
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/access",
-                                json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/access", json=input_, headers=self.gerrit.default_headers
+        )
 
     def create_change(self, input_):
         """
         Create Change for review. This endpoint is functionally equivalent to create change in the
         change API, but it has the project name in the URL, which is easier to route in sharded
         deployments.
         support this method since v3.3.0
@@ -257,31 +263,37 @@
 
             project = client.projects.get('myproject')
             result = project.create_change(input_)
 
         :param input_:
         :return:
         """
-        result = self.gerrit.post(self.endpoint + "/create.change",
-                                  json=input_, headers=self.gerrit.default_headers)
+        result = self.gerrit.post(
+            self.endpoint + "/create.change",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
         return result
 
     def create_access_rights_change(self, input_):
         """
         Sets access rights for the project using the diff schema provided by ProjectAccessInput
         This takes the same input as Update Access Rights, but creates a pending change for review.
         Like Create Change, it returns a ChangeInfo entity describing the resulting change.
         https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#create-access-change
 
         :param input_: the ProjectAccessInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#project-access-input
         :return:
         """
-        result = self.gerrit.put(self.endpoint + "/access:review",
-                                 json=input_, headers=self.gerrit.default_headers)
+        result = self.gerrit.put(
+            self.endpoint + "/access:review",
+            json=input_,
+            headers=self.gerrit.default_headers,
+        )
         return result
 
     def check_access(self, options):
         """
         runs access checks for other users.
 
         :param options:
@@ -311,16 +323,17 @@
             project = client.projects.get('myproject')
             result = project.index(input_)
 
         :param input_: the IndexProjectInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#index-project-input
         :return:
         """
-        self.gerrit.post(self.endpoint + "/index",
-                         json=input_, headers=self.gerrit.default_headers)
+        self.gerrit.post(
+            self.endpoint + "/index", json=input_, headers=self.gerrit.default_headers
+        )
 
     def index_all_changes(self):
         """
         Adds or updates the current project (and children, if specified) in the secondary index.
         The indexing task is executed asynchronously in background and this command returns
         immediately if async is specified in the input.
 
@@ -345,16 +358,17 @@
             project = client.projects.get('myproject')
             result = project.check_consistency(input_)
 
         :param input_: the CheckProjectInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#check-project-input
         :return:
         """
-        return self.gerrit.post(self.endpoint + "/check",
-                                json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(
+            self.endpoint + "/check", json=input_, headers=self.gerrit.default_headers
+        )
 
     @property
     def branches(self):
         """
         List the branches of a project. except the refs/meta/config
 
         :return:
@@ -385,15 +399,17 @@
 
         :return:
         """
         try:
             result = self.gerrit.get(self.endpoint + f"/commits/{commit}")
 
             commit = result.get("commit")
-            return GerritProjectCommit(commit=commit, project=self.id, gerrit=self.gerrit)
+            return GerritProjectCommit(
+                commit=commit, project=self.id, gerrit=self.gerrit
+            )
         except requests.exceptions.HTTPError as error:
             if error.response.status_code == 404:
                 message = f"Commit {commit} does not exist"
                 logger.error(message)
                 raise CommitNotFoundError(message)
             raise GerritAPIException from error
```

### Comparing `python-gerrit-api-3.0.6/gerrit/projects/projects.py` & `python-gerrit-api-3.0.7/gerrit/projects/projects.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from urllib.parse import quote_plus
 import requests
 from gerrit.projects.project import GerritProject
 from gerrit.utils.common import params_creator
 from gerrit.utils.exceptions import (
     ProjectNotFoundError,
     ProjectAlreadyExistsError,
-    GerritAPIException
+    GerritAPIException,
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 class GerritProjects:
@@ -56,15 +56,21 @@
 
         :return:
         """
         if is_all and state:
             raise ValueError("is_all can not be used together with the state option.")
 
         pattern_types = {"prefix": "p", "match": "m", "regex": "r"}
-        tuples = (("n", limit), ("S", skip), ("type", project_type), ("b", branch), ("state", state))
+        tuples = (
+            ("n", limit),
+            ("S", skip),
+            ("type", project_type),
+            ("b", branch),
+            ("state", state),
+        )
         params = params_creator(tuples, pattern_types, pattern_dispatcher)
         if is_all:
             params.clear()
             params["all"] = int(is_all)
         params["d"] = int(description)
 
         return self.gerrit.get(self.endpoint + "/", params=params)
@@ -135,20 +141,25 @@
         """
         try:
             self.get(project_name)
             message = f"Project {project_name} already exists"
             logger.error(message)
             raise ProjectAlreadyExistsError(message)
         except ProjectNotFoundError:
-            self.gerrit.put(self.endpoint + f"/{quote_plus(project_name)}",
-                            json=input_, headers=self.gerrit.default_headers)
+            self.gerrit.put(
+                self.endpoint + f"/{quote_plus(project_name)}",
+                json=input_,
+                headers=self.gerrit.default_headers,
+            )
             return self.get(project_name)
 
     def delete(self, project_name: str):
         """
         Delete the project, requires delete-project plugin
 
         :param project_name: project name
         :return:
         """
         self.get(project_name)
-        self.gerrit.post(self.endpoint + f"/{quote_plus(project_name)}/delete-project~delete")
+        self.gerrit.post(
+            self.endpoint + f"/{quote_plus(project_name)}/delete-project~delete"
+        )
```

### Comparing `python-gerrit-api-3.0.6/gerrit/projects/tags.py` & `python-gerrit-api-3.0.7/gerrit/projects/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from urllib.parse import quote_plus
 import requests
 from gerrit.utils.common import params_creator
 from gerrit.utils.gerritbase import GerritBase
 from gerrit.utils.exceptions import (
     TagNotFoundError,
     TagAlreadyExistsError,
-    GerritAPIException
+    GerritAPIException,
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 class GerritProjectTag(GerritBase):
@@ -50,16 +50,19 @@
 
         :param pattern_dispatcher: Dict of pattern type with respective
                pattern value: {('match'|'regex') : value}
         :param limit: Limit the number of tags to be included in the results.
         :param skip: Skip the given number of tags from the beginning of the list.
         :return:
         """
-        params = params_creator((("n", limit), ("s", skip)),
-                                {"match": "m", "regex": "r"}, pattern_dispatcher)
+        params = params_creator(
+            (("n", limit), ("s", skip)),
+            {"match": "m", "regex": "r"},
+            pattern_dispatcher,
+        )
         return self.gerrit.get(self.endpoint + "/", params=params)
 
     def get(self, name):
         """
         get a tag by ref
 
         :param name: the tag ref
@@ -99,15 +102,18 @@
         try:
             self.get(name)
             message = f"Tag {name} already exists"
             logger.error(message)
             raise TagAlreadyExistsError(message)
         except TagNotFoundError:
             self.gerrit.put(
-                self.endpoint + f"/{quote_plus(name)}", json=input_, headers=self.gerrit.default_headers)
+                self.endpoint + f"/{quote_plus(name)}",
+                json=input_,
+                headers=self.gerrit.default_headers,
+            )
 
             return self.get(name)
 
     def delete(self, name):
         """
         Delete a tag.
```

### Comparing `python-gerrit-api-3.0.6/gerrit/projects/webhooks.py` & `python-gerrit-api-3.0.7/gerrit/projects/webhooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 
 class GerritProjectWebHook(GerritBase):
     def __init__(self, name: str, project: str, gerrit):
         self.name = name
         self.project = project
         self.gerrit = gerrit
-        self.endpoint = f"/config/server/webhooks~projects/{self.project}/remotes/{self.name}"
+        self.endpoint = (
+            f"/config/server/webhooks~projects/{self.project}/remotes/{self.name}"
+        )
         super().__init__(self)
 
     def __str__(self):
         return self.name
 
     def delete(self):
         """
@@ -56,15 +58,16 @@
             new_webhook = project.webhooks.create('test', input_)
 
         :param name: the webhook name
         :param input_: the RemoteInfo entity
         :return:
         """
         result = self.gerrit.put(
-            self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers)
+            self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers
+        )
         return result
 
     def get(self, name):
         """
         Get information about one webhook.
 
         :param name: the webhook name
```

### Comparing `python-gerrit-api-3.0.6/gerrit/utils/common.py` & `python-gerrit-api-3.0.7/gerrit/utils/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,16 +47,14 @@
     if pattern_dispatcher is not None and pattern_dispatcher:
         for item in pattern_types:
             if item in pattern_dispatcher:
                 p, v = pattern_types[item], pattern_dispatcher[item]
                 break
         else:
             k = list(pattern_types.keys())
-            raise ValueError("Pattern types can be either " + ", ".join(k[:-1]) + " or " + k[-1])
+            raise ValueError(
+                "Pattern types can be either " + ", ".join(k[:-1]) + " or " + k[-1]
+            )
 
-    params = {
-        k: v
-        for k, v in tuples + ((p, v),)
-        if v is not None
-    }
+    params = {k: v for k, v in tuples + ((p, v),) if v is not None}
 
     return params
```

### Comparing `python-gerrit-api-3.0.6/gerrit/utils/exceptions.py` & `python-gerrit-api-3.0.7/gerrit/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.6/gerrit/utils/gerritbase.py` & `python-gerrit-api-3.0.7/gerrit/utils/gerritbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 class GerritBase:
     """
     This appears to be the base object that all other gerrit objects are
     inherited from
     """
+
     def __init__(self, pull=True):
         """
         Initialize a gerrit connection
         """
         self._data = None
         if pull:
             self.poll()
@@ -28,15 +29,15 @@
     def poll(self):
         data = self._poll()
         self._data = data
 
         if isinstance(self._data, dict):
             for key, value in self._data.items():
                 try:
-                    if key[0] == '_':
+                    if key[0] == "_":
                         key = key[1:]
                     setattr(self, key, value)
                 except AttributeError:
                     pass
 
     def _poll(self):
         res = self.gerrit.get(self.endpoint)  # pylint: disable=no-member
```

### Comparing `python-gerrit-api-3.0.6/gerrit/utils/requester.py` & `python-gerrit-api-3.0.7/gerrit/utils/requester.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-import six.moves.urllib.parse as urlparse
+import urllib.parse as urlparse
 from requests import Session
 from requests.adapters import HTTPAdapter
 from gerrit.utils.exceptions import (
     NotAllowedError,
     ValidationError,
     AuthError,
     UnauthorizedError,
@@ -30,15 +30,15 @@
     AUTH_COOKIE = None
 
     def __init__(self, **kwargs):
         """
         :param kwargs:
         """
         timeout = 10
-        base_url = kwargs.get('base_url')
+        base_url = kwargs.get("base_url")
         self.base_scheme = urlparse.urlsplit(base_url).scheme if base_url else None
         self.username = kwargs.get("username")
         self.password = kwargs.get("password")
         self.ssl_verify = kwargs.get("ssl_verify")
         self.cert = kwargs.get("cert")
         self.timeout = kwargs.get("timeout", timeout)
         self.session = Session()
@@ -57,15 +57,15 @@
             url_split = urlparse.urlsplit(url)
             url = urlparse.urlunsplit(
                 [
                     self.base_scheme,
                     url_split.netloc,
                     url_split.path,
                     url_split.query,
-                    url_split.fragment
+                    url_split.fragment,
                 ]
             )
         return url
 
     def get_request_dict(
         self, params=None, data=None, json=None, headers=None, **kwargs
     ):
@@ -118,15 +118,15 @@
         self,
         url,
         params=None,
         headers=None,
         allow_redirects=True,
         stream=False,
         raise_for_status: bool = True,
-        **kwargs
+        **kwargs,
     ):
         """
         :param url:
         :param params:
         :param headers:
         :param allow_redirects:
         :param stream:
@@ -135,15 +135,15 @@
         :return:
         """
         request_kwargs = self.get_request_dict(
             params=params,
             headers=headers,
             allow_redirects=allow_redirects,
             stream=stream,
-            **kwargs
+            **kwargs,
         )
         response = self.session.get(self._update_url_scheme(url), **request_kwargs)
         if raise_for_status:
             self.confirm_status(response)
         return response
 
     def post(
@@ -152,15 +152,15 @@
         params=None,
         data=None,
         json=None,
         files=None,
         headers=None,
         allow_redirects=True,
         raise_for_status: bool = True,
-        **kwargs
+        **kwargs,
     ):
         """
         :param url:
         :param params:
         :param data:
         :param json:
         :param files:
@@ -173,15 +173,15 @@
         request_kwargs = self.get_request_dict(
             params=params,
             data=data,
             json=json,
             files=files,
             headers=headers,
             allow_redirects=allow_redirects,
-            **kwargs
+            **kwargs,
         )
         response = self.session.post(self._update_url_scheme(url), **request_kwargs)
         if raise_for_status:
             self.confirm_status(response)
         return response
 
     def put(
@@ -190,15 +190,15 @@
         params=None,
         data=None,
         json=None,
         files=None,
         headers=None,
         allow_redirects=True,
         raise_for_status: bool = True,
-        **kwargs
+        **kwargs,
     ):
         """
         :param url:
         :param params:
         :param data:
         :param json:
         :param files:
@@ -211,22 +211,29 @@
         request_kwargs = self.get_request_dict(
             params=params,
             data=data,
             json=json,
             files=files,
             headers=headers,
             allow_redirects=allow_redirects,
-            **kwargs
+            **kwargs,
         )
         response = self.session.put(self._update_url_scheme(url), **request_kwargs)
         if raise_for_status:
             self.confirm_status(response)
         return response
 
-    def delete(self, url, headers=None, allow_redirects=True, raise_for_status: bool = True, **kwargs):
+    def delete(
+        self,
+        url,
+        headers=None,
+        allow_redirects=True,
+        raise_for_status: bool = True,
+        **kwargs,
+    ):
         """
         :param url:
         :param headers:
         :param allow_redirects:
         :param raise_for_status:
         :param kwargs:
         :return:
@@ -256,18 +263,22 @@
                 reason = res.reason.decode("utf-8")
             except UnicodeDecodeError:
                 reason = res.reason.decode("iso-8859-1")
         else:
             reason = res.reason
 
         if 400 <= res.status_code < 500:
-            http_error_msg = f"{res.status_code} Client Error: {reason} for url: {res.url}"
+            http_error_msg = (
+                f"{res.status_code} Client Error: {reason} for url: {res.url}"
+            )
 
         elif 500 <= res.status_code < 600:
-            http_error_msg = f"{res.status_code} Server Error: {reason} for url: {res.url}"
+            http_error_msg = (
+                f"{res.status_code} Server Error: {reason} for url: {res.url}"
+            )
 
         if not http_error_msg:
             return
 
         if res.status_code == 400:
             # Validation error
             raise ValidationError(http_error_msg)
```

### Comparing `python-gerrit-api-3.0.6/gitiles/base.py` & `python-gerrit-api-3.0.7/gitiles/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from typing import Optional
 from base64 import b64decode
 from gerrit.utils.requester import Requester
-from gerrit.utils.common import (
-    decode_response,
-    strip_trailing_slash
-)
+from gerrit.utils.common import decode_response, strip_trailing_slash
 
 
 class GitilesClient:
     def __init__(
         self,
         base_url,
         username=None,
@@ -59,15 +56,17 @@
             params.update({"s": start})
 
         response = self.requester.get(self.get_endpoint_url(endpoint), params=params)
         result = decode_response(response)
 
         return result
 
-    def download_file(self, repo: str, ref: str, path: str, format: str = "TEXT", decode: bool = False):
+    def download_file(
+        self, repo: str, ref: str, path: str, format: str = "TEXT", decode: bool = False
+    ):
         """Downloads raw file content from a Gitiles repository."""
         endpoint = f"/{repo}/+/{ref}/{path}"
         params = {"format": format}
 
         response = self.requester.get(self.get_endpoint_url(endpoint), params=params)
         result = decode_response(response)
```

### Comparing `python-gerrit-api-3.0.6/python_gerrit_api.egg-info/PKG-INFO` & `python-gerrit-api-3.0.7/python_gerrit_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 3.0.6
+Version: 3.0.7
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 License-File: LICENSE
 Requires-Dist: requests
-Requires-Dist: six>=1.10.0
 
 Project description
 ===================
 
 .. image:: https://img.shields.io/pypi/pyversions/python-gerrit-api.svg
     :target: https://pypi.python.org/pypi/python-gerrit-api
 .. image:: https://img.shields.io/pypi/v/python-gerrit-api.svg
```

### Comparing `python-gerrit-api-3.0.6/python_gerrit_api.egg-info/SOURCES.txt` & `python-gerrit-api-3.0.7/python_gerrit_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.6/setup.py` & `python-gerrit-api-3.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.6/tests/test_accounts.py` & `python-gerrit-api-3.0.7/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.6/tests/test_changes.py` & `python-gerrit-api-3.0.7/tests/test_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
 def test_get_change_reviewer(gerrit_client):
     change_id = "LineageOS%2Fandroid~lineage-20.0~I0bcf3ba13177947a2c018d9dcebdb94b561573d3"
     change = gerrit_client.changes.get(id_=change_id)
 
     from gerrit.utils.exceptions import ReviewerNotFoundError
     with pytest.raises(ReviewerNotFoundError):
-        change.reviewers.get(account="shijl900925")
+        change.reviewers.get(account="shijl0925")
 
     reviewer = change.reviewers.get(account="javelinanddart")
     assert "_account_id" in reviewer.to_dict()
 
     votes = reviewer.list_votes()
     assert votes.get("Code-Review") == 2
 
@@ -170,8 +170,8 @@
     change_id = "LineageOS%2Fandroid~lineage-20.0~I0bcf3ba13177947a2c018d9dcebdb94b561573d3"
     change = gerrit_client.changes.get(id_=change_id)
 
     from gerrit.utils.exceptions import ReviewerAlreadyExistsError
     with pytest.raises(ReviewerAlreadyExistsError):
         change.reviewers.add(input_={"reviewer": "javelinanddart"})
 
-    change.reviewers.add(input_={"reviewer": "shijl0925"})
+    change.reviewers.add(input_={"reviewer": "jialiang.shi"})
```

### Comparing `python-gerrit-api-3.0.6/tests/test_gitiles.py` & `python-gerrit-api-3.0.7/tests/test_gitiles.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.6/tests/test_groups.py` & `python-gerrit-api-3.0.7/tests/test_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     group = gerrit_client.groups.get(group_id)
 
     account_id = 16
     from gerrit.utils.exceptions import GroupMemberAlreadyExistsError
     with pytest.raises(GroupMemberAlreadyExistsError):
         group.members.add(account_id)
 
-    user = gerrit_client.accounts.get(account="shijl0925")
+    user = gerrit_client.accounts.get(account="jialiang.shi")
     account_id = user.account_id
     logger.debug(f"account id: {account_id}")
     group.members.add(account_id)
 
 
 def test_group_member(gerrit_client):
     group_id = 613
```

### Comparing `python-gerrit-api-3.0.6/tests/test_projects.py` & `python-gerrit-api-3.0.7/tests/test_projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,28 +88,28 @@
     project_info = project.to_dict()
     assert project_info.get("name") == project_name
     assert project_info.get("id") == quote_plus(project_name)
 
     assert project.name == project_name
 
     assert project != gerrit_client.projects.get(name="LineageOS/android_art")
-    assert project != gerrit_client.accounts.get(account="shijl0925")
+    assert project != gerrit_client.accounts.get(account="jialiang.shi")
 
 
 @pytest.mark.parametrize('gerrit_object', data, indirect=True)
 def test_get_project_access_rights(gerrit_client, gerrit_object):
     project_name = gerrit_object["project_name"]
     project = gerrit_client.projects.get(name=project_name)
     access_rights = project.get_access_rights()
     assert "inherits_from" in access_rights.keys()
 
 
 @pytest.mark.parametrize('project_name, expected',
                          [("LineageOS/android", "Head-Developers"),
-                          ("LineageOS/android_device_google_tangorpro", "PROJECT-Google-gs201")
+                          ("LineageOS/android_device_google_tangorpro", "PROJECT-Google-tangorpro")
                           ])
 def test_get_project_parent(gerrit_client, project_name, expected):
     project = gerrit_client.projects.get(name=project_name)
     HEAD = project.get_parent()
     assert HEAD == expected
```

### Comparing `python-gerrit-api-3.0.6/tests/test_revision.py` & `python-gerrit-api-3.0.7/tests/test_revision.py`

 * *Files identical despite different names*

