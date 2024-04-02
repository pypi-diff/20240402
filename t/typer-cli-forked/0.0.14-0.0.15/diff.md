# Comparing `tmp/typer_cli_forked-0.0.14.tar.gz` & `tmp/typer_cli_forked-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "typer_cli_forked-0.0.15.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `typer_cli_forked-0.0.14.tar` & `typer_cli_forked-0.0.15.tar`

### file list

```diff
@@ -1,53 +1,55 @@
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/.coveragerc
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/mypy.ini
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/release-notes.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/requirements.txt
--rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/typer_cli_forked-0.0.14-py3-none-any.whl
--rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/typer_cli_forked-0.0.14.tar.gz
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/.github/FUNDING.yml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/.github/dependabot.yml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/.github/workflows/issue-manager.yml
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/.github/workflows/publish.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/.github/workflows/smokeshow.yml
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/.github/workflows/test.yml
--rwxr-xr-x   0        0        0      206 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/scripts/format-imports.sh
--rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/scripts/format.sh
--rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/scripts/lint.sh
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/scripts/publish.sh
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/scripts/test.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_app_other_name.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_completion_run.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_doc.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_empty_script.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_func_other_name.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_help.py
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_multi_app.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_multi_app_cli.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_multi_app_sub.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_multi_func.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_not_python.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_sub.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_sub_completion.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_sub_help.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/assets/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/assets/app_other_name.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/assets/empty_script.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/assets/func_other_name.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/assets/multi_app.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/assets/multi_app_cli.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/assets/multi_func.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/assets/multiapp-docs.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/assets/not_python.txt
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/tests/assets/sample.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/typer_cli/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/typer_cli/__main__.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/typer_cli/main.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/LICENSE
--rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/README.md
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/pyproject.toml
--rw-r--r--   0        0        0    12986 2020-02-02 00:00:00.000000 typer_cli_forked-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/.coveragerc
+-rw-r--r--   0        0        0     4554 2024-04-02 10:00:45.363140 typer_cli_forked-0.0.15/.github/DISCUSSION_TEMPLATE/questions.yml
+-rw-r--r--   0        0        0       19 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/.github/FUNDING.yml
+-rw-r--r--   0        0        0      594 2024-04-02 10:00:45.363140 typer_cli_forked-0.0.15/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      896 2024-04-02 10:00:45.363140 typer_cli_forked-0.0.15/.github/ISSUE_TEMPLATE/privileged.yml
+-rw-r--r--   0        0        0      309 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/.github/dependabot.yml
+-rw-r--r--   0        0        0      618 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/.github/workflows/issue-manager.yml
+-rw-r--r--   0        0        0      978 2024-04-02 10:00:45.363140 typer_cli_forked-0.0.15/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0      999 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      957 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/.github/workflows/smokeshow.yml
+-rw-r--r--   0        0        0     3039 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/.github/workflows/test.yml
+-rw-r--r--   0        0        0       90 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/.gitignore
+-rw-r--r--   0        0        0     1086 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/LICENSE
+-rw-r--r--   0        0        0    11003 2024-04-02 10:00:42.523082 typer_cli_forked-0.0.15/README.md
+-rw-r--r--   0        0        0     1108 2024-04-02 10:00:45.363140 typer_cli_forked-0.0.15/SECURITY.md
+-rw-r--r--   0        0        0       56 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/mypy.ini
+-rw-r--r--   0        0        0     1855 2024-04-02 10:03:45.766831 typer_cli_forked-0.0.15/pyproject.toml
+-rw-r--r--   0        0        0     6627 2024-04-02 10:00:45.363140 typer_cli_forked-0.0.15/release-notes.md
+-rw-r--r--   0        0        0      197 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/requirements.txt
+-rwxr-xr-x   0        0        0      206 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/scripts/format-imports.sh
+-rwxr-xr-x   0        0        0      190 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/scripts/format.sh
+-rwxr-xr-x   0        0        0      116 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/scripts/lint.sh
+-rwxr-xr-x   0        0        0       52 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/scripts/publish.sh
+-rwxr-xr-x   0        0        0       80 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0      273 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/scripts/test.sh
+-rw-r--r--   0        0        0        0 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/assets/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/assets/app_other_name.py
+-rw-r--r--   0        0        0        0 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/assets/empty_script.py
+-rw-r--r--   0        0        0       67 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/assets/func_other_name.py
+-rw-r--r--   0        0        0      622 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/assets/multi_app.py
+-rw-r--r--   0        0        0      265 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/assets/multi_app_cli.py
+-rw-r--r--   0        0        0      180 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/assets/multi_func.py
+-rw-r--r--   0        0        0     1334 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/assets/multiapp-docs.md
+-rw-r--r--   0        0        0       19 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/assets/not_python.txt
+-rw-r--r--   0        0        0      412 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/assets/sample.py
+-rw-r--r--   0        0        0      805 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_app_other_name.py
+-rw-r--r--   0        0        0      574 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_completion_run.py
+-rw-r--r--   0        0        0     2413 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_doc.py
+-rw-r--r--   0        0        0      380 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_empty_script.py
+-rw-r--r--   0        0        0      424 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_func_other_name.py
+-rw-r--r--   0        0        0      585 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_help.py
+-rw-r--r--   0        0        0     2477 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_multi_app.py
+-rw-r--r--   0        0        0     2044 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_multi_app_cli.py
+-rw-r--r--   0        0        0      930 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_multi_app_sub.py
+-rw-r--r--   0        0        0     2208 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_multi_func.py
+-rw-r--r--   0        0        0      316 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_not_python.py
+-rw-r--r--   0        0        0     2554 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_sub.py
+-rw-r--r--   0        0        0      590 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_sub_completion.py
+-rw-r--r--   0        0        0      500 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_sub_help.py
+-rw-r--r--   0        0        0      279 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/tests/test_version.py
+-rw-r--r--   0        0        0       23 2024-04-02 10:03:52.930978 typer_cli_forked-0.0.15/typer_cli/__init__.py
+-rw-r--r--   0        0        0       31 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/typer_cli/__main__.py
+-rw-r--r--   0        0        0     9206 2023-06-20 12:55:37.275693 typer_cli_forked-0.0.15/typer_cli/main.py
+-rw-r--r--   0        0        0    12744 1970-01-01 00:00:00.000000 typer_cli_forked-0.0.15/PKG-INFO
```

### Comparing `typer_cli_forked-0.0.14/release-notes.md` & `typer_cli_forked-0.0.15/release-notes.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Release Notes
 
 ## Latest Changes
 
+* 👷 Update tokens for tmate and latest changes. PR [#127](https://github.com/tiangolo/typer-cli/pull/127) by [@tiangolo](https://github.com/tiangolo).
+* 👷 Update token for latest changes. PR [#126](https://github.com/tiangolo/typer-cli/pull/126) by [@tiangolo](https://github.com/tiangolo).
 * ⬆️ Update pytest-cov requirement from ^2.8.1 to ^4.0.0. PR [#76](https://github.com/tiangolo/typer-cli/pull/76) by [@dependabot[bot]](https://github.com/apps/dependabot).
 * ⬆️ Update mypy requirement from ^0.910 to ^1.0. PR [#83](https://github.com/tiangolo/typer-cli/pull/83) by [@dependabot[bot]](https://github.com/apps/dependabot).
 
+### Internal
+
+* 🔧 Add GitHub templates for discussions and issues, and security policy. PR [#133](https://github.com/tiangolo/typer-cli/pull/133) by [@alejsdev](https://github.com/alejsdev).
+* 👷 Update latest-changes GitHub Action. PR [#130](https://github.com/tiangolo/typer-cli/pull/130) by [@tiangolo](https://github.com/tiangolo).
 
 ## 0.0.13
 
 ### Upgrades
 
 * ✨ Refactor to make Typer CLI compatible with (and require) Typer `>=0.4.0` and Click `8.x.x`. Initial PRs [#67](https://github.com/tiangolo/typer-cli/pull/67) by [@cdcadman](https://github.com/cdcadman) and [#82](https://github.com/tiangolo/typer-cli/pull/82) by [@omBratteng](https://github.com/omBratteng).
```

### Comparing `typer_cli_forked-0.0.14/.github/workflows/issue-manager.yml` & `typer_cli_forked-0.0.15/.github/workflows/issue-manager.yml`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/.github/workflows/latest-changes.yml` & `typer_cli_forked-0.0.15/.github/workflows/latest-changes.yml`

 * *Files 13% similar despite different names*

```diff
@@ -10,31 +10,26 @@
     inputs:
       number:
         description: PR number
         required: true
       debug_enabled:
         description: 'Run the build with tmate debugging enabled (https://github.com/marketplace/actions/debugging-with-tmate)'
         required: false
-        default: ''
+        default: 'false'
 
 jobs:
   latest-changes:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           # To allow latest-changes to commit to master
-          token: ${{ secrets.ACTIONS_TOKEN }}
-      # Allow debugging with tmate
-      - name: Setup tmate session
-        uses: mxschmitt/action-tmate@v3
-        if: ${{ github.event_name == 'workflow_dispatch' && github.event.inputs.debug_enabled == 'true' }}
-        with:
-          limit-access-to-actor: true
-          token: ${{ secrets.ACTIONS_TOKEN }}
-          standard_token: ${{ secrets.GITHUB_TOKEN }}
-      - uses: docker://tiangolo/latest-changes:0.0.3
+          token: ${{ secrets.TYPER_CLI_LATEST_CHANGES }}
+      - uses: docker://tiangolo/latest-changes:0.2.0
+      # - uses: tiangolo/latest-changes@main
         with:
           token: ${{ secrets.GITHUB_TOKEN }}
           latest_changes_file: release-notes.md
-          latest_changes_header: '## Latest Changes\n\n'
+          latest_changes_header: '## Latest Changes'
           debug_logs: true
+          end_regex: '^## '
+          label_header_prefix: '### '
```

### Comparing `typer_cli_forked-0.0.14/.github/workflows/publish.yml` & `typer_cli_forked-0.0.15/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/.github/workflows/smokeshow.yml` & `typer_cli_forked-0.0.15/.github/workflows/smokeshow.yml`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/.github/workflows/test.yml` & `typer_cli_forked-0.0.15/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/tests/test_app_other_name.py` & `typer_cli_forked-0.0.15/tests/test_app_other_name.py`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/tests/test_completion_run.py` & `typer_cli_forked-0.0.15/tests/test_completion_run.py`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/tests/test_doc.py` & `typer_cli_forked-0.0.15/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/tests/test_help.py` & `typer_cli_forked-0.0.15/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/tests/test_multi_app.py` & `typer_cli_forked-0.0.15/tests/test_multi_app.py`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/tests/test_multi_app_cli.py` & `typer_cli_forked-0.0.15/tests/test_multi_app_cli.py`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/tests/test_multi_app_sub.py` & `typer_cli_forked-0.0.15/tests/test_multi_app_sub.py`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/tests/test_multi_func.py` & `typer_cli_forked-0.0.15/tests/test_multi_func.py`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/tests/test_sub.py` & `typer_cli_forked-0.0.15/tests/test_sub.py`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/tests/test_sub_completion.py` & `typer_cli_forked-0.0.15/tests/test_sub_completion.py`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/tests/assets/multi_app.py` & `typer_cli_forked-0.0.15/tests/assets/multi_app.py`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/tests/assets/multiapp-docs.md` & `typer_cli_forked-0.0.15/tests/assets/multiapp-docs.md`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/typer_cli/main.py` & `typer_cli_forked-0.0.15/typer_cli/main.py`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/LICENSE` & `typer_cli_forked-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_cli_forked-0.0.14/README.md` & `typer_cli_forked-0.0.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,14 @@
 <a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/tiangolo/typer-cli" target="_blank">
     <img src="https://coverage-badge.samuelcolvin.workers.dev/tiangolo/typer-cli.svg" alt="Coverage">
 <a href="https://pypi.org/project/typer-cli" target="_blank">
     <img src="https://badge.fury.io/py/typer-cli.svg" alt="Package version">
 </a>
 </p>
 
-# Note on the fork
-
-This is a temporary fork of [https://pypi.org/project/typer-cli/] while [this PR](https://github.com/tiangolo/typer-cli/pull/120) has not been merged and released.
-
-For general uses, use the main typer-cli library.
-
-# Description
-
 There is an optional utility tool called **Typer CLI**, additional to **Typer** itself.
 
 It's main feature is to provide ✨ completion ✨ in the Terminal for your own small programs built with **Typer**.
 
 ...without you having to create a complete installable Python package.
 
 It's probably most useful if you have a small custom Python script using **Typer** (maybe as part of some project), for some small tasks, and it's not complex/important enough to create a whole installable Python package for it (something to be installed with `pip`).
```

### Comparing `typer_cli_forked-0.0.14/pyproject.toml` & `typer_cli_forked-0.0.15/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
 [project]
 name = "typer-cli-forked"
 description = "Run Typer scripts with completion, without having to create a package, using Typer CLI."
 readme = "README.md"
 requires-python = ">=3.7"
-license = "MIT"
+license = {file = "LICENSE"}
 authors = [
     {name = "Sebastián Ramírez", email = "tiangolo@gmail.com"},
 ]
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
@@ -36,24 +32,31 @@
     "Typing :: Typed",
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License"
 ]
 
 dynamic = ["version"]
 dependencies = [
-"typer >=0.4.0,<=0.9.0",
+"typer ~= 0.12",
 "colorama >=0.4.3,<=0.5.0",
-"shellingham >=1.3.2,<=1.5.0",
+"shellingham >= 1.3",
 ]
 
+[project.optional-dependencies]
+build = ["flit ~= 3.9"]
+
 [project.urls]
 Homepage = "https://github.com/tiangolo/typer-cli"
 Documentation = "https://typer.tiangolo.com/typer-cli/"
 
 [project.scripts]
 typer = "typer_cli.main:main"
 
-[tool.hatch.version]
-path = "typer_cli/__init__.py"
+[build-system]
+requires = ["flit_core ~= 3.8,<4"]
+build-backend = "flit_core.buildapi"
+
+[tool.flit.module]
+name = "typer_cli"
 
 [tool.isort]
 profile = "black"
```

### Comparing `typer_cli_forked-0.0.14/PKG-INFO` & `typer_cli_forked-0.0.15/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: typer-cli-forked
-Version: 0.0.14
+Version: 0.0.15
 Summary: Run Typer scripts with completion, without having to create a package, using Typer CLI.
-Project-URL: Homepage, https://github.com/tiangolo/typer-cli
-Project-URL: Documentation, https://typer.tiangolo.com/typer-cli/
 Author-email: Sebastián Ramírez <tiangolo@gmail.com>
-License-Expression: MIT
-License-File: LICENSE
-Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Requires-Dist: colorama<=0.5.0,>=0.4.3
-Requires-Dist: shellingham<=1.5.0,>=1.3.2
-Requires-Dist: typer<=0.9.0,>=0.4.0
-Description-Content-Type: text/markdown
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Requires-Dist: typer ~= 0.12
+Requires-Dist: colorama >=0.4.3,<=0.5.0
+Requires-Dist: shellingham >= 1.3
+Requires-Dist: flit ~= 3.9 ; extra == "build"
+Project-URL: Documentation, https://typer.tiangolo.com/typer-cli/
+Project-URL: Homepage, https://github.com/tiangolo/typer-cli
+Provides-Extra: build
 
 # Typer CLI
 
 <p align="center">
     <em>Run <strong>Typer</strong> scripts with completion, without having to create a package, using <strong>Typer CLI</strong>.</em>
 </p>
 <p align="center">
@@ -49,22 +49,14 @@
 <a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/tiangolo/typer-cli" target="_blank">
     <img src="https://coverage-badge.samuelcolvin.workers.dev/tiangolo/typer-cli.svg" alt="Coverage">
 <a href="https://pypi.org/project/typer-cli" target="_blank">
     <img src="https://badge.fury.io/py/typer-cli.svg" alt="Package version">
 </a>
 </p>
 
-# Note on the fork
-
-This is a temporary fork of [https://pypi.org/project/typer-cli/] while [this PR](https://github.com/tiangolo/typer-cli/pull/120) has not been merged and released.
-
-For general uses, use the main typer-cli library.
-
-# Description
-
 There is an optional utility tool called **Typer CLI**, additional to **Typer** itself.
 
 It's main feature is to provide ✨ completion ✨ in the Terminal for your own small programs built with **Typer**.
 
 ...without you having to create a complete installable Python package.
 
 It's probably most useful if you have a small custom Python script using **Typer** (maybe as part of some project), for some small tasks, and it's not complex/important enough to create a whole installable Python package for it (something to be installed with `pip`).
@@ -534,7 +526,8 @@
 * `--help`: Show this message and exit.
 
 ---
 
 ## License
 
 **Typer CLI**, the same as **Typer**, is licensed under the terms of the MIT license.
+
```

