# Comparing `tmp/hcs-cli-0.1.97.tar.gz` & `tmp/hcs-cli-0.1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.97.tar", last modified: Tue Sep 12 23:48:27 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.98.tar", last modified: Thu Sep 14 00:07:10 2023, max compression
```

## Comparing `hcs-cli-0.1.97.tar` & `hcs-cli-0.1.98.tar`

### file list

```diff
@@ -1,361 +1,361 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.397156 hcs-cli-0.1.97/
--rw-r--r--   0 nanw       (501) staff       (20)     2849 2023-08-25 05:19:39.000000 hcs-cli-0.1.97/.gitignore
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.183488 hcs-cli-0.1.97/.vscode/
--rw-r--r--   0 nanw       (501) staff       (20)     3304 2023-09-12 23:37:54.000000 hcs-cli-0.1.97/.vscode/launch.json
--rw-r--r--   0 nanw       (501) staff       (20)      391 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/.vscode/settings.json
--rw-r--r--   0 nanw       (501) staff       (20)       98 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/CODE_OF_CONDUCT.md
--rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/CONTRIBUTING_CLA.md
--rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/GOVERNANCE.md
--rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/LICENSE
--rw-r--r--   0 nanw       (501) staff       (20)      895 2023-08-25 05:18:47.000000 hcs-cli-0.1.97/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)      411 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/NOTICE
--rw-r--r--   0 nanw       (501) staff       (20)     4351 2023-09-12 23:48:27.396740 hcs-cli-0.1.97/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     3477 2023-08-25 17:52:56.000000 hcs-cli-0.1.97/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.189777 hcs-cli-0.1.97/doc/
--rw-r--r--   0 nanw       (501) staff       (20)      639 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/doc/az-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)     6713 2023-08-22 19:13:57.000000 hcs-cli-0.1.97/doc/dev-setup.md
--rw-r--r--   0 nanw       (501) staff       (20)      763 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/doc/get-csp-user-api-token.md
--rw-r--r--   0 nanw       (501) staff       (20)     8063 2023-08-09 18:58:55.000000 hcs-cli-0.1.97/doc/hcs-cli-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)    14052 2023-08-28 19:11:18.000000 hcs-cli-0.1.97/doc/hcs-plan.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.191880 hcs-cli-0.1.97/doc/images/
--rw-r--r--   0 nanw       (501) staff       (20)    23659 2023-08-09 17:56:41.000000 hcs-cli-0.1.97/doc/images/hcs-plan-graph.svg
--rw-r--r--   0 nanw       (501) staff       (20)   142119 2023-08-09 17:56:41.000000 hcs-cli-0.1.97/doc/images/hcs-plan.png
--rw-r--r--   0 nanw       (501) staff       (20)     1622 2023-08-25 17:35:43.000000 hcs-cli-0.1.97/doc/work-with-dev-envs.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.196692 hcs-cli-0.1.97/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     4351 2023-09-12 23:48:26.000000 hcs-cli-0.1.97/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     8672 2023-09-12 23:48:27.000000 hcs-cli-0.1.97/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-09-12 23:48:26.000000 hcs-cli-0.1.97/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-09-12 23:48:26.000000 hcs-cli-0.1.97/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      337 2023-09-12 23:48:26.000000 hcs-cli-0.1.97/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-09-12 23:48:26.000000 hcs-cli-0.1.97/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.97/mypy.ini
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.134088 hcs-cli-0.1.97/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.197549 hcs-cli-0.1.97/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.97/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      194 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/requirements-dev.txt
--rw-r--r--   0 nanw       (501) staff       (20)      336 2023-08-25 04:48:52.000000 hcs-cli-0.1.97/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-09-12 23:48:27.397297 hcs-cli-0.1.97/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)     1382 2023-08-10 22:15:28.000000 hcs-cli-0.1.97/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.200585 hcs-cli-0.1.97/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.97/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/tests/conftest.py
--rwxr-xr-x   0 nanw       (501) staff       (20)      119 2023-08-10 17:50:57.000000 hcs-cli-0.1.97/tests/test.sh
--rw-r--r--   0 nanw       (501) staff       (20)     3939 2023-08-10 22:10:49.000000 hcs-cli-0.1.97/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.201296 hcs-cli-0.1.97/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.97/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.202993 hcs-cli-0.1.97/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.97/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.205230 hcs-cli-0.1.97/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.97/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.206394 hcs-cli-0.1.97/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.97/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/tests/vhcs/cli/cmds/pki/get_root_ca.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.207475 hcs-cli-0.1.97/tests/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:43.000000 hcs-cli-0.1.97/tests/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)    16472 2023-08-28 18:50:43.000000 hcs-cli-0.1.97/tests/vhcs/cli/cmds/plan/test_plan.py
--rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      899 2023-08-10 17:52:36.000000 hcs-cli-0.1.97/tests/vhcs/cli/cmds/test_login.py
--rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/tests/vhcs/cli/cmds/test_profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     4073 2023-08-10 22:15:28.000000 hcs-cli-0.1.97/tests/vhcs/cli/test_common_args_and_return.py
--rw-r--r--   0 nanw       (501) staff       (20)     3674 2023-08-10 22:15:28.000000 hcs-cli-0.1.97/tests/vhcs/cli/test_error_handling.py
--rw-r--r--   0 nanw       (501) staff       (20)        6 2023-09-12 23:48:25.000000 hcs-cli-0.1.97/version
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.208525 hcs-cli-0.1.97/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.97/vhcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      687 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/__main__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.209590 hcs-cli-0.1.97/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.97/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.212029 hcs-cli-0.1.97/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.97/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.212592 hcs-cli-0.1.97/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.215008 hcs-cli-0.1.97/vhcs/cli/cmds/admin/ad/
--rw-r--r--   0 nanw       (501) staff       (20)      636 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/ad/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      972 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/ad/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      934 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/ad/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      845 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/ad/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.216111 hcs-cli-0.1.97/vhcs/cli/cmds/admin/azure-infra/
--rw-r--r--   0 nanw       (501) staff       (20)      640 2023-08-10 17:15:38.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/azure-infra/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      990 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/azure-infra/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.218427 hcs-cli-0.1.97/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-08-10 17:15:07.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2104 2023-08-10 22:15:28.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/edge/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      917 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      853 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.221895 hcs-cli-0.1.97/vhcs/cli/cmds/admin/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      637 2023-08-10 17:14:42.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2592 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/provider/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     1032 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)     1052 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1061 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.224207 hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-08-09 17:56:41.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      925 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1838 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.226072 hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/vm/
--rw-r--r--   0 nanw       (501) staff       (20)      622 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/vm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      994 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/vm/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      926 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/vm/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.228536 hcs-cli-0.1.97/vhcs/cli/cmds/admin/uag/
--rw-r--r--   0 nanw       (501) staff       (20)      623 2023-08-10 17:15:18.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/uag/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/uag/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/uag/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      849 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/admin/uag/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.229116 hcs-cli-0.1.97/vhcs/cli/cmds/auth/
--rw-r--r--   0 nanw       (501) staff       (20)      632 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/auth/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.230335 hcs-cli-0.1.97/vhcs/cli/cmds/auth/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/auth/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      908 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.230902 hcs-cli-0.1.97/vhcs/cli/cmds/daas/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/daas/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.232526 hcs-cli-0.1.97/vhcs/cli/cmds/daas/infra/
--rw-r--r--   0 nanw       (501) staff       (20)      648 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/daas/infra/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1037 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/daas/infra/basic.py
--rw-r--r--   0 nanw       (501) staff       (20)     7458 2023-08-29 00:42:03.000000 hcs-cli-0.1.97/vhcs/cli/cmds/daas/infra/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.234876 hcs-cli-0.1.97/vhcs/cli/cmds/daas/tenant/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/daas/tenant/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1030 2023-09-12 17:27:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/daas/tenant/consumption.py
--rw-r--r--   0 nanw       (501) staff       (20)     4607 2023-08-28 17:16:14.000000 hcs-cli-0.1.97/vhcs/cli/cmds/daas/tenant/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     4802 2023-08-28 17:16:26.000000 hcs-cli-0.1.97/vhcs/cli/cmds/daas/tenant/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.237693 hcs-cli-0.1.97/vhcs/cli/cmds/ims/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/ims/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      951 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/ims/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      900 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/ims/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      921 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/ims/list.py
--rw-r--r--   0 nanw       (501) staff       (20)      995 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/ims/list_copies.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.239962 hcs-cli-0.1.97/vhcs/cli/cmds/ims/version/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/ims/version/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1715 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/ims/version/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)     1277 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/ims/version/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1132 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/ims/version/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.241629 hcs-cli-0.1.97/vhcs/cli/cmds/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)      637 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/inventory/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      943 2023-08-09 18:31:01.000000 hcs-cli-0.1.97/vhcs/cli/cmds/inventory/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.242148 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.244383 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      801 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      792 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      964 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.247544 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1863 2023-08-10 16:48:30.000000 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     1056 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      960 2023-08-10 22:15:28.000000 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1372 2023-08-10 16:49:25.000000 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)     7610 2023-09-12 20:43:36.000000 hcs-cli-0.1.97/vhcs/cli/cmds/login.py
--rw-r--r--   0 nanw       (501) staff       (20)      740 2023-08-31 18:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/logout.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.248078 hcs-cli-0.1.97/vhcs/cli/cmds/org/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-08-10 17:12:52.000000 hcs-cli-0.1.97/vhcs/cli/cmds/org/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.249862 hcs-cli-0.1.97/vhcs/cli/cmds/org/datacenter/
--rw-r--r--   0 nanw       (501) staff       (20)      634 2023-08-10 17:13:12.000000 hcs-cli-0.1.97/vhcs/cli/cmds/org/datacenter/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      848 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/org/datacenter/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      974 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/org/datacenter/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.251723 hcs-cli-0.1.97/vhcs/cli/cmds/org/detail/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-08-10 17:13:05.000000 hcs-cli-0.1.97/vhcs/cli/cmds/org/detail/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      883 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/org/detail/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/org/detail/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.255630 hcs-cli-0.1.97/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      883 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      775 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1774 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      726 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.258105 hcs-cli-0.1.97/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      666 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2445 2023-09-12 23:44:23.000000 hcs-cli-0.1.97/vhcs/cli/cmds/plan/apply.py
--rw-r--r--   0 nanw       (501) staff       (20)     2422 2023-08-09 17:56:41.000000 hcs-cli-0.1.97/vhcs/cli/cmds/plan/destroy.py
--rw-r--r--   0 nanw       (501) staff       (20)     2191 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/plan/graph.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.258673 hcs-cli-0.1.97/vhcs/cli/cmds/portal/
--rw-r--r--   0 nanw       (501) staff       (20)      634 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.260858 hcs-cli-0.1.97/vhcs/cli/cmds/portal/entitlement/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/entitlement/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      922 2023-08-10 16:34:53.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/entitlement/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      946 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/entitlement/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      857 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/entitlement/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.263024 hcs-cli-0.1.97/vhcs/cli/cmds/portal/pool/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/pool/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      908 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/pool/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      933 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/pool/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      926 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/pool/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.266445 hcs-cli-0.1.97/vhcs/cli/cmds/portal/site/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/site/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1101 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/site/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      905 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/site/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      927 2023-08-10 21:09:35.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/site/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      830 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/site/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1015 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/portal/site/set-edge.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.267610 hcs-cli-0.1.97/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.97/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1744 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/profile/init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.268725 hcs-cli-0.1.97/vhcs/cli/cmds/tsctl/
--rw-r--r--   0 nanw       (501) staff       (20)      645 2023-08-09 17:56:41.000000 hcs-cli-0.1.97/vhcs/cli/cmds/tsctl/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1877 2023-08-10 22:15:28.000000 hcs-cli-0.1.97/vhcs/cli/cmds/tsctl/task.py
--rw-r--r--   0 nanw       (501) staff       (20)      932 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.269278 hcs-cli-0.1.97/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/vmhub/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.271437 hcs-cli-0.1.97/vhcs/cli/cmds/vmhub/otp/
--rw-r--r--   0 nanw       (501) staff       (20)      643 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/vmhub/otp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/vmhub/otp/redeem.py
--rw-r--r--   0 nanw       (501) staff       (20)     1120 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/cli/cmds/vmhub/otp/request.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2884 2023-08-31 20:18:15.000000 hcs-cli-0.1.97/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.272621 hcs-cli-0.1.97/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.97/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.303721 hcs-cli-0.1.97/vhcs/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      790 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.306227 hcs-cli-0.1.97/vhcs/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3083 2023-08-10 22:15:28.000000 hcs-cli-0.1.97/vhcs/ctxp/built_in_cmds/_ut.py
--rw-r--r--   0 nanw       (501) staff       (20)     2379 2023-08-10 17:35:16.000000 hcs-cli-0.1.97/vhcs/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     3971 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1859 2023-08-10 22:15:28.000000 hcs-cli-0.1.97/vhcs/ctxp/cli_options.py
--rw-r--r--   0 nanw       (501) staff       (20)     5466 2023-08-29 16:13:03.000000 hcs-cli-0.1.97/vhcs/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      936 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1208 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)    11497 2023-08-29 00:42:04.000000 hcs-cli-0.1.97/vhcs/ctxp/data_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2856 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     3063 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     6342 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/logger.py
--rw-r--r--   0 nanw       (501) staff       (20)     6475 2023-09-08 21:13:47.000000 hcs-cli-0.1.97/vhcs/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/profile_store.py
--rw-r--r--   0 nanw       (501) staff       (20)     1597 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     6980 2023-08-25 18:16:20.000000 hcs-cli-0.1.97/vhcs/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/ctxp/var_template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.319824 hcs-cli-0.1.97/vhcs/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      175 2023-08-09 17:56:41.000000 hcs-cli-0.1.97/vhcs/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      125 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/actions.py
--rw-r--r--   0 nanw       (501) staff       (20)     1298 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/base_provider.py
--rw-r--r--   0 nanw       (501) staff       (20)      116 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/context.py
--rw-r--r--   0 nanw       (501) staff       (20)    17626 2023-08-28 18:58:31.000000 hcs-cli-0.1.97/vhcs/plan/core.py
--rw-r--r--   0 nanw       (501) staff       (20)    10382 2023-08-28 18:58:50.000000 hcs-cli-0.1.97/vhcs/plan/dag.py
--rw-r--r--   0 nanw       (501) staff       (20)     7464 2023-08-28 18:59:16.000000 hcs-cli-0.1.97/vhcs/plan/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     5594 2023-08-23 23:10:01.000000 hcs-cli-0.1.97/vhcs/plan/kop.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.321467 hcs-cli-0.1.97/vhcs/plan/provider/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.335545 hcs-cli-0.1.97/vhcs/plan/provider/azure/
--rw-r--r--   0 nanw       (501) staff       (20)      167 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/azure/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7225 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/azure/_az_facade.py
--rw-r--r--   0 nanw       (501) staff       (20)      648 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/azure/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1574 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/azure/aad_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     2225 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/azure/aad_user.py
--rw-r--r--   0 nanw       (501) staff       (20)     1392 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/azure/nat_gateway.py
--rw-r--r--   0 nanw       (501) staff       (20)     1570 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/azure/nsg.py
--rw-r--r--   0 nanw       (501) staff       (20)     1603 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/azure/public_ip.py
--rw-r--r--   0 nanw       (501) staff       (20)     1517 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/azure/resource_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1965 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/azure/subnet.py
--rw-r--r--   0 nanw       (501) staff       (20)     1574 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/azure/virtual_network.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.339052 hcs-cli-0.1.97/vhcs/plan/provider/dev/
--rw-r--r--   0 nanw       (501) staff       (20)       30 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       34 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1694 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/dev/dummy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1114 2023-08-10 22:15:28.000000 hcs-cli-0.1.97/vhcs/plan/provider/dev/fibonacci.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.349796 hcs-cli-0.1.97/vhcs/plan/provider/hcs/
--rw-r--r--   0 nanw       (501) staff       (20)       30 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/hcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       34 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/hcs/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1494 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/hcs/ad.py
--rw-r--r--   0 nanw       (501) staff       (20)     3648 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/hcs/edge.py
--rw-r--r--   0 nanw       (501) staff       (20)     1315 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/hcs/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)     1407 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/hcs/identity_provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     3513 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/hcs/image.py
--rw-r--r--   0 nanw       (501) staff       (20)     1529 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/hcs/pool_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     2046 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/hcs/pool_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     1648 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/hcs/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     1407 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/plan/provider/hcs/site.py
--rw-r--r--   0 nanw       (501) staff       (20)     1951 2023-08-23 23:58:54.000000 hcs-cli-0.1.97/vhcs/plan/provider/hcs/uag.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.350461 hcs-cli-0.1.97/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.97/vhcs/service/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.355586 hcs-cli-0.1.97/vhcs/service/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       69 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      868 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/admin/ad.py
--rw-r--r--   0 nanw       (501) staff       (20)     1219 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/admin/azure_infra.py
--rw-r--r--   0 nanw       (501) staff       (20)     3765 2023-08-23 23:55:11.000000 hcs-cli-0.1.97/vhcs/service/admin/edge.py
--rw-r--r--   0 nanw       (501) staff       (20)     1312 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/admin/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1478 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/admin/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2014 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/admin/template.py
--rw-r--r--   0 nanw       (501) staff       (20)     3175 2023-08-24 00:03:28.000000 hcs-cli-0.1.97/vhcs/service/admin/uag.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.357344 hcs-cli-0.1.97/vhcs/service/auth/
--rw-r--r--   0 nanw       (501) staff       (20)       20 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/auth/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      897 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/auth/admin.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.360936 hcs-cli-0.1.97/vhcs/service/ims/
--rw-r--r--   0 nanw       (501) staff       (20)       72 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/ims/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2366 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/ims/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)      960 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/ims/image_copies.py
--rw-r--r--   0 nanw       (501) staff       (20)     2099 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/ims/images.py
--rw-r--r--   0 nanw       (501) staff       (20)     3356 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/ims/version.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.362053 hcs-cli-0.1.97/vhcs/service/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)       26 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1308 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/inventory/vm.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.364219 hcs-cli-0.1.97/vhcs/service/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/lcm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/lcm/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2774 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/lcm/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.366462 hcs-cli-0.1.97/vhcs/service/org_service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/org_service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1099 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/org_service/datacenter.py
--rw-r--r--   0 nanw       (501) staff       (20)     1056 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/org_service/details.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.367523 hcs-cli-0.1.97/vhcs/service/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1226 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/pki/certificate.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.369823 hcs-cli-0.1.97/vhcs/service/portal/
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/portal/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      958 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/portal/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)      944 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/portal/pool.py
--rw-r--r--   0 nanw       (501) staff       (20)     1510 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/portal/site.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.371389 hcs-cli-0.1.97/vhcs/service/tsctl/
--rw-r--r--   0 nanw       (501) staff       (20)       53 2023-08-10 22:15:28.000000 hcs-cli-0.1.97/vhcs/service/tsctl/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1097 2023-08-10 22:15:28.000000 hcs-cli-0.1.97/vhcs/service/tsctl/base.py
--rw-r--r--   0 nanw       (501) staff       (20)     1527 2023-08-10 22:15:28.000000 hcs-cli-0.1.97/vhcs/service/tsctl/task.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.372393 hcs-cli-0.1.97/vhcs/service/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       18 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1420 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/service/vmhub/otp.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.376503 hcs-cli-0.1.97/vhcs/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4414 2023-09-12 17:27:44.000000 hcs-cli-0.1.97/vhcs/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1404 2023-08-29 00:42:03.000000 hcs-cli-0.1.97/vhcs/sglib/cli_options.py
--rw-r--r--   0 nanw       (501) staff       (20)     6797 2023-08-29 23:23:49.000000 hcs-cli-0.1.97/vhcs/sglib/client_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     8043 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     5217 2023-08-10 22:15:29.000000 hcs-cli-0.1.97/vhcs/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      897 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)     9839 2023-09-11 22:31:17.000000 hcs-cli-0.1.97/vhcs/sglib/login_support.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.378128 hcs-cli-0.1.97/vhcs/support/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/support/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.383605 hcs-cli-0.1.97/vhcs/support/daas/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/support/daas/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1469 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/support/daas/cidr_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3933 2023-08-28 18:54:48.000000 hcs-cli-0.1.97/vhcs/support/daas/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1305 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/support/daas/infra.py
--rw-r--r--   0 nanw       (501) staff       (20)     4323 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/support/daas/infra_green.py
--rw-r--r--   0 nanw       (501) staff       (20)     4001 2023-08-25 20:39:40.000000 hcs-cli-0.1.97/vhcs/support/daas/infra_reuse.py
--rw-r--r--   0 nanw       (501) staff       (20)      436 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/support/daas/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.169125 hcs-cli-0.1.97/vhcs/support/daas/templates/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.390592 hcs-cli-0.1.97/vhcs/support/daas/templates/v1/
--rw-r--r--   0 nanw       (501) staff       (20)    14945 2023-08-28 18:59:38.000000 hcs-cli-0.1.97/vhcs/support/daas/templates/v1/infra-green.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      318 2023-08-28 17:18:26.000000 hcs-cli-0.1.97/vhcs/support/daas/templates/v1/infra-green.var.yml
--rw-r--r--   0 nanw       (501) staff       (20)    13100 2023-08-28 18:59:43.000000 hcs-cli-0.1.97/vhcs/support/daas/templates/v1/infra-reuse.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      502 2023-08-28 17:18:10.000000 hcs-cli-0.1.97/vhcs/support/daas/templates/v1/infra-reuse.var.yml
--rw-r--r--   0 nanw       (501) staff       (20)     3942 2023-08-28 18:59:51.000000 hcs-cli-0.1.97/vhcs/support/daas/templates/v1/tenant.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      142 2023-08-28 17:18:22.000000 hcs-cli-0.1.97/vhcs/support/daas/templates/v1/tenant.var.yml
--rw-r--r--   0 nanw       (501) staff       (20)     4869 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/support/daas/tenant_prep.py
--rw-r--r--   0 nanw       (501) staff       (20)     2040 2023-08-10 22:15:28.000000 hcs-cli-0.1.97/vhcs/support/daas/tenant_summary.py
--rw-r--r--   0 nanw       (501) staff       (20)     1470 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/support/plan_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2628 2023-08-28 18:54:45.000000 hcs-cli-0.1.97/vhcs/support/profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-12 23:48:27.396086 hcs-cli-0.1.97/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.97/vhcs/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     8145 2023-09-12 23:45:22.000000 hcs-cli-0.1.97/vhcs/util/job_view.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1909 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2958 2023-08-25 05:18:06.000000 hcs-cli-0.1.97/vhcs/util/scheduler.py
--rw-r--r--   0 nanw       (501) staff       (20)     1718 2023-08-01 22:36:44.000000 hcs-cli-0.1.97/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.581274 hcs-cli-0.1.98/
+-rw-r--r--   0 nanw       (501) staff       (20)     2849 2023-08-25 05:19:39.000000 hcs-cli-0.1.98/.gitignore
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.212889 hcs-cli-0.1.98/.vscode/
+-rw-r--r--   0 nanw       (501) staff       (20)     3304 2023-09-12 23:37:54.000000 hcs-cli-0.1.98/.vscode/launch.json
+-rw-r--r--   0 nanw       (501) staff       (20)      391 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/.vscode/settings.json
+-rw-r--r--   0 nanw       (501) staff       (20)       98 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/CONTRIBUTING_CLA.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/GOVERNANCE.md
+-rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/LICENSE
+-rw-r--r--   0 nanw       (501) staff       (20)      895 2023-08-25 05:18:47.000000 hcs-cli-0.1.98/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)      411 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/NOTICE
+-rw-r--r--   0 nanw       (501) staff       (20)     4351 2023-09-14 00:07:10.580144 hcs-cli-0.1.98/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     3477 2023-08-25 17:52:56.000000 hcs-cli-0.1.98/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.218533 hcs-cli-0.1.98/doc/
+-rw-r--r--   0 nanw       (501) staff       (20)      639 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/doc/az-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6713 2023-08-22 19:13:57.000000 hcs-cli-0.1.98/doc/dev-setup.md
+-rw-r--r--   0 nanw       (501) staff       (20)      763 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/doc/get-csp-user-api-token.md
+-rw-r--r--   0 nanw       (501) staff       (20)     8063 2023-08-09 18:58:55.000000 hcs-cli-0.1.98/doc/hcs-cli-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)    14052 2023-08-28 19:11:18.000000 hcs-cli-0.1.98/doc/hcs-plan.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.220604 hcs-cli-0.1.98/doc/images/
+-rw-r--r--   0 nanw       (501) staff       (20)    23659 2023-08-09 17:56:41.000000 hcs-cli-0.1.98/doc/images/hcs-plan-graph.svg
+-rw-r--r--   0 nanw       (501) staff       (20)   142119 2023-08-09 17:56:41.000000 hcs-cli-0.1.98/doc/images/hcs-plan.png
+-rw-r--r--   0 nanw       (501) staff       (20)     1622 2023-08-25 17:35:43.000000 hcs-cli-0.1.98/doc/work-with-dev-envs.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.225263 hcs-cli-0.1.98/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     4351 2023-09-14 00:07:09.000000 hcs-cli-0.1.98/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     8672 2023-09-14 00:07:09.000000 hcs-cli-0.1.98/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-09-14 00:07:09.000000 hcs-cli-0.1.98/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-09-14 00:07:09.000000 hcs-cli-0.1.98/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      337 2023-09-14 00:07:09.000000 hcs-cli-0.1.98/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-09-14 00:07:09.000000 hcs-cli-0.1.98/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.98/mypy.ini
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.142534 hcs-cli-0.1.98/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.226054 hcs-cli-0.1.98/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.98/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      194 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/requirements-dev.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      336 2023-08-25 04:48:52.000000 hcs-cli-0.1.98/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-09-14 00:07:10.581677 hcs-cli-0.1.98/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)     1382 2023-08-10 22:15:28.000000 hcs-cli-0.1.98/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.246761 hcs-cli-0.1.98/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.98/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/tests/conftest.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)      119 2023-08-10 17:50:57.000000 hcs-cli-0.1.98/tests/test.sh
+-rw-r--r--   0 nanw       (501) staff       (20)     3939 2023-08-10 22:10:49.000000 hcs-cli-0.1.98/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.247752 hcs-cli-0.1.98/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.98/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.250821 hcs-cli-0.1.98/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.98/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.256650 hcs-cli-0.1.98/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.98/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.258472 hcs-cli-0.1.98/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.98/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/tests/vhcs/cli/cmds/pki/get_root_ca.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.260863 hcs-cli-0.1.98/tests/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:43.000000 hcs-cli-0.1.98/tests/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)    16472 2023-08-28 18:50:43.000000 hcs-cli-0.1.98/tests/vhcs/cli/cmds/plan/test_plan.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      899 2023-08-10 17:52:36.000000 hcs-cli-0.1.98/tests/vhcs/cli/cmds/test_login.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/tests/vhcs/cli/cmds/test_profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4073 2023-08-10 22:15:28.000000 hcs-cli-0.1.98/tests/vhcs/cli/test_common_args_and_return.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3674 2023-08-10 22:15:28.000000 hcs-cli-0.1.98/tests/vhcs/cli/test_error_handling.py
+-rw-r--r--   0 nanw       (501) staff       (20)        6 2023-09-14 00:07:08.000000 hcs-cli-0.1.98/version
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.262775 hcs-cli-0.1.98/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.98/vhcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      687 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/__main__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.264613 hcs-cli-0.1.98/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.98/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.268629 hcs-cli-0.1.98/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.98/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.269738 hcs-cli-0.1.98/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.273931 hcs-cli-0.1.98/vhcs/cli/cmds/admin/ad/
+-rw-r--r--   0 nanw       (501) staff       (20)      636 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/ad/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      972 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/ad/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      934 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/ad/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      845 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/ad/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.276831 hcs-cli-0.1.98/vhcs/cli/cmds/admin/azure-infra/
+-rw-r--r--   0 nanw       (501) staff       (20)      640 2023-08-10 17:15:38.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/azure-infra/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      990 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/azure-infra/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.297961 hcs-cli-0.1.98/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-08-10 17:15:07.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2104 2023-08-10 22:15:28.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/edge/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      917 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      853 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.303782 hcs-cli-0.1.98/vhcs/cli/cmds/admin/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      637 2023-08-10 17:14:42.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2592 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/provider/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1032 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1052 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1061 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.307987 hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-08-09 17:56:41.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      925 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1838 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.311392 hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/vm/
+-rw-r--r--   0 nanw       (501) staff       (20)      622 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/vm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      994 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/vm/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      926 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/vm/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.315625 hcs-cli-0.1.98/vhcs/cli/cmds/admin/uag/
+-rw-r--r--   0 nanw       (501) staff       (20)      623 2023-08-10 17:15:18.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/uag/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/uag/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/uag/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      849 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/admin/uag/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.316293 hcs-cli-0.1.98/vhcs/cli/cmds/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)      632 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/auth/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.317750 hcs-cli-0.1.98/vhcs/cli/cmds/auth/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/auth/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      908 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.318516 hcs-cli-0.1.98/vhcs/cli/cmds/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/daas/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.320429 hcs-cli-0.1.98/vhcs/cli/cmds/daas/infra/
+-rw-r--r--   0 nanw       (501) staff       (20)      648 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/daas/infra/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1037 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/daas/infra/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7458 2023-08-29 00:42:03.000000 hcs-cli-0.1.98/vhcs/cli/cmds/daas/infra/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.346692 hcs-cli-0.1.98/vhcs/cli/cmds/daas/tenant/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/daas/tenant/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1030 2023-09-12 17:27:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/daas/tenant/consumption.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4607 2023-08-28 17:16:14.000000 hcs-cli-0.1.98/vhcs/cli/cmds/daas/tenant/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4802 2023-08-28 17:16:26.000000 hcs-cli-0.1.98/vhcs/cli/cmds/daas/tenant/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.350031 hcs-cli-0.1.98/vhcs/cli/cmds/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      951 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/ims/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      900 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/ims/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      921 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/ims/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)      995 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/ims/list_copies.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.352448 hcs-cli-0.1.98/vhcs/cli/cmds/ims/version/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/ims/version/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1715 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/ims/version/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1277 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/ims/version/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1132 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/ims/version/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.354320 hcs-cli-0.1.98/vhcs/cli/cmds/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)      637 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/inventory/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      943 2023-08-09 18:31:01.000000 hcs-cli-0.1.98/vhcs/cli/cmds/inventory/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.354898 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.357128 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      801 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      792 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      964 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.360442 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1863 2023-08-10 16:48:30.000000 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1056 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      960 2023-08-10 22:15:28.000000 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1372 2023-08-10 16:49:25.000000 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7610 2023-09-12 20:43:36.000000 hcs-cli-0.1.98/vhcs/cli/cmds/login.py
+-rw-r--r--   0 nanw       (501) staff       (20)      740 2023-08-31 18:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/logout.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.360947 hcs-cli-0.1.98/vhcs/cli/cmds/org/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-08-10 17:12:52.000000 hcs-cli-0.1.98/vhcs/cli/cmds/org/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.363006 hcs-cli-0.1.98/vhcs/cli/cmds/org/datacenter/
+-rw-r--r--   0 nanw       (501) staff       (20)      634 2023-08-10 17:13:12.000000 hcs-cli-0.1.98/vhcs/cli/cmds/org/datacenter/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      848 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/org/datacenter/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      974 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/org/datacenter/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.364438 hcs-cli-0.1.98/vhcs/cli/cmds/org/detail/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-08-10 17:13:05.000000 hcs-cli-0.1.98/vhcs/cli/cmds/org/detail/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      883 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/org/detail/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/org/detail/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.367323 hcs-cli-0.1.98/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      883 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      775 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1774 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      726 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.371364 hcs-cli-0.1.98/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      666 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2445 2023-09-12 23:44:23.000000 hcs-cli-0.1.98/vhcs/cli/cmds/plan/apply.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2422 2023-08-09 17:56:41.000000 hcs-cli-0.1.98/vhcs/cli/cmds/plan/destroy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2191 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/plan/graph.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.372101 hcs-cli-0.1.98/vhcs/cli/cmds/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)      634 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.396702 hcs-cli-0.1.98/vhcs/cli/cmds/portal/entitlement/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/entitlement/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      922 2023-08-10 16:34:53.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/entitlement/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      946 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/entitlement/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      857 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/entitlement/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.399065 hcs-cli-0.1.98/vhcs/cli/cmds/portal/pool/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/pool/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      908 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/pool/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      933 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/pool/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      926 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/pool/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.401748 hcs-cli-0.1.98/vhcs/cli/cmds/portal/site/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/site/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1101 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/site/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      905 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/site/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      927 2023-08-10 21:09:35.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/site/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      830 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/site/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1015 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/portal/site/set-edge.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.402645 hcs-cli-0.1.98/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.98/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1744 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/profile/init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.403545 hcs-cli-0.1.98/vhcs/cli/cmds/tsctl/
+-rw-r--r--   0 nanw       (501) staff       (20)      645 2023-08-09 17:56:41.000000 hcs-cli-0.1.98/vhcs/cli/cmds/tsctl/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1877 2023-08-10 22:15:28.000000 hcs-cli-0.1.98/vhcs/cli/cmds/tsctl/task.py
+-rw-r--r--   0 nanw       (501) staff       (20)      932 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.404026 hcs-cli-0.1.98/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/vmhub/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.405426 hcs-cli-0.1.98/vhcs/cli/cmds/vmhub/otp/
+-rw-r--r--   0 nanw       (501) staff       (20)      643 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/vmhub/otp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/vmhub/otp/redeem.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1120 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/cli/cmds/vmhub/otp/request.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2884 2023-08-31 20:18:15.000000 hcs-cli-0.1.98/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.406525 hcs-cli-0.1.98/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.98/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.414910 hcs-cli-0.1.98/vhcs/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.416616 hcs-cli-0.1.98/vhcs/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3083 2023-08-10 22:15:28.000000 hcs-cli-0.1.98/vhcs/ctxp/built_in_cmds/_ut.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2379 2023-08-10 17:35:16.000000 hcs-cli-0.1.98/vhcs/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3971 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1859 2023-08-10 22:15:28.000000 hcs-cli-0.1.98/vhcs/ctxp/cli_options.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5466 2023-08-29 16:13:03.000000 hcs-cli-0.1.98/vhcs/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      936 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1208 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    11497 2023-08-29 00:42:04.000000 hcs-cli-0.1.98/vhcs/ctxp/data_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2856 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3063 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6342 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/logger.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6475 2023-09-08 21:13:47.000000 hcs-cli-0.1.98/vhcs/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1597 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6980 2023-09-13 23:31:57.000000 hcs-cli-0.1.98/vhcs/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/ctxp/var_template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.420832 hcs-cli-0.1.98/vhcs/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      175 2023-08-09 17:56:41.000000 hcs-cli-0.1.98/vhcs/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      125 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/actions.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1298 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/base_provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)      116 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    17626 2023-08-28 18:58:31.000000 hcs-cli-0.1.98/vhcs/plan/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)    10382 2023-09-14 00:04:08.000000 hcs-cli-0.1.98/vhcs/plan/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7464 2023-08-28 18:59:16.000000 hcs-cli-0.1.98/vhcs/plan/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5590 2023-09-13 23:57:14.000000 hcs-cli-0.1.98/vhcs/plan/kop.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.421481 hcs-cli-0.1.98/vhcs/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.450667 hcs-cli-0.1.98/vhcs/plan/provider/azure/
+-rw-r--r--   0 nanw       (501) staff       (20)      167 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/azure/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7225 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/azure/_az_facade.py
+-rw-r--r--   0 nanw       (501) staff       (20)      648 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/azure/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1574 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/azure/aad_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2225 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/azure/aad_user.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1392 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/azure/nat_gateway.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1570 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/azure/nsg.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1603 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/azure/public_ip.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1517 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/azure/resource_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1965 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/azure/subnet.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1574 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/azure/virtual_network.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.452541 hcs-cli-0.1.98/vhcs/plan/provider/dev/
+-rw-r--r--   0 nanw       (501) staff       (20)       30 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       34 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1694 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/dev/dummy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1114 2023-08-10 22:15:28.000000 hcs-cli-0.1.98/vhcs/plan/provider/dev/fibonacci.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.458663 hcs-cli-0.1.98/vhcs/plan/provider/hcs/
+-rw-r--r--   0 nanw       (501) staff       (20)       30 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/hcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       34 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/hcs/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1494 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/hcs/ad.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3648 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/hcs/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1315 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/hcs/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1407 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/hcs/identity_provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3513 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/hcs/image.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1529 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/hcs/pool_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2046 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/hcs/pool_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1648 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/hcs/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1407 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/plan/provider/hcs/site.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1951 2023-08-23 23:58:54.000000 hcs-cli-0.1.98/vhcs/plan/provider/hcs/uag.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.459164 hcs-cli-0.1.98/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.98/vhcs/service/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.462691 hcs-cli-0.1.98/vhcs/service/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       69 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      868 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/admin/ad.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1219 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/admin/azure_infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3765 2023-08-23 23:55:11.000000 hcs-cli-0.1.98/vhcs/service/admin/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1312 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/admin/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1478 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/admin/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2014 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/admin/template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3175 2023-08-24 00:03:28.000000 hcs-cli-0.1.98/vhcs/service/admin/uag.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.463607 hcs-cli-0.1.98/vhcs/service/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)       20 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/auth/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      897 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/auth/admin.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.466423 hcs-cli-0.1.98/vhcs/service/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)       72 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2366 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/ims/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)      960 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/ims/image_copies.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2099 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/ims/images.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3356 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/ims/version.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.467508 hcs-cli-0.1.98/vhcs/service/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)       26 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1308 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/inventory/vm.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.468965 hcs-cli-0.1.98/vhcs/service/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/lcm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/lcm/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2774 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/lcm/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.470361 hcs-cli-0.1.98/vhcs/service/org_service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/org_service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1099 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/org_service/datacenter.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1056 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/org_service/details.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.471766 hcs-cli-0.1.98/vhcs/service/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1226 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/pki/certificate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.498699 hcs-cli-0.1.98/vhcs/service/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/portal/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      958 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/portal/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)      944 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/portal/pool.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1510 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/portal/site.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.501167 hcs-cli-0.1.98/vhcs/service/tsctl/
+-rw-r--r--   0 nanw       (501) staff       (20)       53 2023-08-10 22:15:28.000000 hcs-cli-0.1.98/vhcs/service/tsctl/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1097 2023-08-10 22:15:28.000000 hcs-cli-0.1.98/vhcs/service/tsctl/base.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1527 2023-08-10 22:15:28.000000 hcs-cli-0.1.98/vhcs/service/tsctl/task.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.502706 hcs-cli-0.1.98/vhcs/service/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       18 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1420 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/service/vmhub/otp.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.512167 hcs-cli-0.1.98/vhcs/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5093 2023-09-14 00:05:29.000000 hcs-cli-0.1.98/vhcs/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1404 2023-08-29 00:42:03.000000 hcs-cli-0.1.98/vhcs/sglib/cli_options.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6797 2023-08-29 23:23:49.000000 hcs-cli-0.1.98/vhcs/sglib/client_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8043 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5217 2023-08-10 22:15:29.000000 hcs-cli-0.1.98/vhcs/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      897 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)    10052 2023-09-14 00:05:29.000000 hcs-cli-0.1.98/vhcs/sglib/login_support.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.518935 hcs-cli-0.1.98/vhcs/support/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/support/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.547398 hcs-cli-0.1.98/vhcs/support/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/support/daas/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1469 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/support/daas/cidr_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3933 2023-08-28 18:54:48.000000 hcs-cli-0.1.98/vhcs/support/daas/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1305 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/support/daas/infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4323 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/support/daas/infra_green.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4001 2023-08-25 20:39:40.000000 hcs-cli-0.1.98/vhcs/support/daas/infra_reuse.py
+-rw-r--r--   0 nanw       (501) staff       (20)      436 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/support/daas/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.175498 hcs-cli-0.1.98/vhcs/support/daas/templates/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.561847 hcs-cli-0.1.98/vhcs/support/daas/templates/v1/
+-rw-r--r--   0 nanw       (501) staff       (20)    14945 2023-08-28 18:59:38.000000 hcs-cli-0.1.98/vhcs/support/daas/templates/v1/infra-green.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      318 2023-08-28 17:18:26.000000 hcs-cli-0.1.98/vhcs/support/daas/templates/v1/infra-green.var.yml
+-rw-r--r--   0 nanw       (501) staff       (20)    13100 2023-08-28 18:59:43.000000 hcs-cli-0.1.98/vhcs/support/daas/templates/v1/infra-reuse.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      502 2023-08-28 17:18:10.000000 hcs-cli-0.1.98/vhcs/support/daas/templates/v1/infra-reuse.var.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     3942 2023-08-28 18:59:51.000000 hcs-cli-0.1.98/vhcs/support/daas/templates/v1/tenant.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      142 2023-08-28 17:18:22.000000 hcs-cli-0.1.98/vhcs/support/daas/templates/v1/tenant.var.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     4917 2023-09-13 22:22:09.000000 hcs-cli-0.1.98/vhcs/support/daas/tenant_prep.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2040 2023-08-10 22:15:28.000000 hcs-cli-0.1.98/vhcs/support/daas/tenant_summary.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1470 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/support/plan_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2628 2023-08-28 18:54:45.000000 hcs-cli-0.1.98/vhcs/support/profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-09-14 00:07:10.578901 hcs-cli-0.1.98/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.98/vhcs/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8145 2023-09-12 23:45:22.000000 hcs-cli-0.1.98/vhcs/util/job_view.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1909 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2958 2023-08-25 05:18:06.000000 hcs-cli-0.1.98/vhcs/util/scheduler.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1718 2023-08-01 22:36:44.000000 hcs-cli-0.1.98/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.97/.gitignore` & `hcs-cli-0.1.98/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/.vscode/launch.json` & `hcs-cli-0.1.98/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/CODE_OF_CONDUCT.md` & `hcs-cli-0.1.98/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/CONTRIBUTING_CLA.md` & `hcs-cli-0.1.98/CONTRIBUTING_CLA.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/GOVERNANCE.md` & `hcs-cli-0.1.98/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/LICENSE` & `hcs-cli-0.1.98/LICENSE`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/Makefile` & `hcs-cli-0.1.98/Makefile`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/PKG-INFO` & `hcs-cli-0.1.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.97
+Version: 0.1.98
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.97/README.md` & `hcs-cli-0.1.98/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/doc/az-cheatsheet.md` & `hcs-cli-0.1.98/doc/az-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/doc/dev-setup.md` & `hcs-cli-0.1.98/doc/dev-setup.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/doc/get-csp-user-api-token.md` & `hcs-cli-0.1.98/doc/get-csp-user-api-token.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/doc/hcs-cli-cheatsheet.md` & `hcs-cli-0.1.98/doc/hcs-cli-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/doc/hcs-plan.md` & `hcs-cli-0.1.98/doc/hcs-plan.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/doc/images/hcs-plan-graph.svg` & `hcs-cli-0.1.98/doc/images/hcs-plan-graph.svg`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/doc/images/hcs-plan.png` & `hcs-cli-0.1.98/doc/images/hcs-plan.png`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/doc/work-with-dev-envs.md` & `hcs-cli-0.1.98/doc/work-with-dev-envs.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.98/hcs_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.97
+Version: 0.1.98
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.97/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.98/hcs_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/payload/lcm/zero.json` & `hcs-cli-0.1.98/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/pyproject.toml` & `hcs-cli-0.1.98/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/setup.py` & `hcs-cli-0.1.98/setup.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/tests/conftest.py` & `hcs-cli-0.1.98/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/tests/test_utils.py` & `hcs-cli-0.1.98/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/tests/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.98/tests/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/tests/vhcs/cli/cmds/plan/test_plan.py` & `hcs-cli-0.1.98/tests/vhcs/cli/cmds/plan/test_plan.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.98/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/tests/vhcs/cli/cmds/test_login.py` & `hcs-cli-0.1.98/tests/vhcs/cli/cmds/test_login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.98/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/tests/vhcs/cli/test_common_args_and_return.py` & `hcs-cli-0.1.98/tests/vhcs/cli/test_common_args_and_return.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/tests/vhcs/cli/test_error_handling.py` & `hcs-cli-0.1.98/tests/vhcs/cli/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/__main__.py` & `hcs-cli-0.1.98/vhcs/__main__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/ad/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/ad/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/ad/delete.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/ad/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/ad/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/ad/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/ad/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/ad/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/azure-infra/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/azure-infra/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/azure-infra/main.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/azure-infra/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/edge/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/edge/delete.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/edge/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/edge/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/edge/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/edge/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/edge/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/provider/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/provider/create.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/provider/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/provider/delete.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/provider/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/provider/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/provider/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/provider/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/delete.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/vm/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/vm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/vm/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/vm/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/template/vm/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/template/vm/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/uag/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/uag/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/uag/delete.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/uag/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/uag/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/uag/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/admin/uag/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/admin/uag/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/auth/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/auth/admin/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/auth/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/auth/admin/get_org_idp_map.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/auth/admin/get_org_idp_map.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/daas/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/daas/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/daas/infra/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/daas/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/daas/infra/basic.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/daas/infra/basic.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/daas/infra/plan.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/daas/infra/plan.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/daas/tenant/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/daas/tenant/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/daas/tenant/consumption.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/daas/tenant/consumption.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/daas/tenant/create.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/daas/tenant/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/daas/tenant/plan.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/daas/tenant/plan.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/ims/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/ims/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/ims/delete.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/ims/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/ims/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/ims/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/ims/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/ims/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/ims/list_copies.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/ims/list_copies.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/ims/version/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/ims/version/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/ims/version/delete.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/ims/version/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/ims/version/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/ims/version/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/ims/version/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/ims/version/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/inventory/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/inventory/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/inventory/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/inventory/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/inventory/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/lcm/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/lcm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/lcm/provider/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/lcm/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/lcm/provider/delete.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/lcm/provider/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/lcm/provider/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/lcm/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/lcm/provider/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/lcm/provider/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/lcm/template/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/lcm/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/lcm/template/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/lcm/template/delete.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/lcm/template/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/lcm/template/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/lcm/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/lcm/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/login.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/logout.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/logout.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/org/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/org/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/org/datacenter/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/org/datacenter/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/org/datacenter/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/org/datacenter/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/org/datacenter/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/org/datacenter/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/org/detail/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/org/detail/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/org/detail/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/org/detail/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/org/detail/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/org/detail/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/pki/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/pki/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/pki/get_org_cert.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/pki/get_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/pki/test.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/pki/test.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/plan/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/plan/apply.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/plan/apply.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/plan/destroy.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/plan/destroy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/plan/graph.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/plan/graph.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/entitlement/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/entitlement/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/entitlement/delete.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/entitlement/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/entitlement/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/entitlement/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/entitlement/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/entitlement/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/pool/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/pool/delete.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/pool/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/pool/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/pool/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/pool/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/pool/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/site/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/site/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/site/create.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/site/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/site/delete.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/site/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/site/get.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/site/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/site/list.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/site/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/portal/site/set-edge.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/portal/site/set-edge.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/profile/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/tsctl/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/tsctl/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/tsctl/task.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/tsctl/task.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/upgrade.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/upgrade.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/vmhub/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/vmhub/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/vmhub/otp/__init__.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/vmhub/otp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/vmhub/otp/redeem.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/vmhub/otp/redeem.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/cmds/vmhub/otp/request.py` & `hcs-cli-0.1.98/vhcs/cli/cmds/vmhub/otp/request.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/cli/main.py` & `hcs-cli-0.1.98/vhcs/cli/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.98/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/README.md` & `hcs-cli-0.1.98/vhcs/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/__init__.py` & `hcs-cli-0.1.98/vhcs/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/_init.py` & `hcs-cli-0.1.98/vhcs/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/built_in_cmds/_ut.py` & `hcs-cli-0.1.98/vhcs/ctxp/built_in_cmds/_ut.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.98/vhcs/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.98/vhcs/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/cli_options.py` & `hcs-cli-0.1.98/vhcs/ctxp/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/cli_processor.py` & `hcs-cli-0.1.98/vhcs/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/config.py` & `hcs-cli-0.1.98/vhcs/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/context.py` & `hcs-cli-0.1.98/vhcs/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/data_util.py` & `hcs-cli-0.1.98/vhcs/ctxp/data_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/duration.py` & `hcs-cli-0.1.98/vhcs/ctxp/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/fstore.py` & `hcs-cli-0.1.98/vhcs/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/init.py` & `hcs-cli-0.1.98/vhcs/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/jsondot.py` & `hcs-cli-0.1.98/vhcs/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/logger.py` & `hcs-cli-0.1.98/vhcs/ctxp/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/profile.py` & `hcs-cli-0.1.98/vhcs/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/profile_store.py` & `hcs-cli-0.1.98/vhcs/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/state.py` & `hcs-cli-0.1.98/vhcs/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/util.py` & `hcs-cli-0.1.98/vhcs/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/ctxp/var_template.py` & `hcs-cli-0.1.98/vhcs/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/base_provider.py` & `hcs-cli-0.1.98/vhcs/plan/base_provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/core.py` & `hcs-cli-0.1.98/vhcs/plan/core.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/dag.py` & `hcs-cli-0.1.98/vhcs/plan/dag.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/helper.py` & `hcs-cli-0.1.98/vhcs/plan/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/kop.py` & `hcs-cli-0.1.98/vhcs/plan/kop.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
     def error(self, err):
         if isinstance(err, Exception):
             if _need_stack_trace(err):
                 traceback.print_exception(type(err), err, err.__traceback__)
             details = error_details(err)
         else:
-            details = str(details)
+            details = str(err)
         self._add_log(KopAction.error, details)
         self._closed = True
         _job_view.error(self._job_id(), details)
 
     def skip(self, reason):
         self._add_log(KopAction.skip, reason)
         self._closed = True
```

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/azure/_az_facade.py` & `hcs-cli-0.1.98/vhcs/plan/provider/azure/_az_facade.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/azure/_prepare.py` & `hcs-cli-0.1.98/vhcs/plan/provider/azure/_prepare.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/azure/aad_group.py` & `hcs-cli-0.1.98/vhcs/plan/provider/azure/aad_group.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/azure/aad_user.py` & `hcs-cli-0.1.98/vhcs/plan/provider/azure/aad_user.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/azure/nat_gateway.py` & `hcs-cli-0.1.98/vhcs/plan/provider/azure/nat_gateway.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/azure/nsg.py` & `hcs-cli-0.1.98/vhcs/plan/provider/azure/nsg.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/azure/public_ip.py` & `hcs-cli-0.1.98/vhcs/plan/provider/azure/public_ip.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/azure/resource_group.py` & `hcs-cli-0.1.98/vhcs/plan/provider/azure/resource_group.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/azure/subnet.py` & `hcs-cli-0.1.98/vhcs/plan/provider/azure/subnet.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/azure/virtual_network.py` & `hcs-cli-0.1.98/vhcs/plan/provider/azure/virtual_network.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/dev/dummy.py` & `hcs-cli-0.1.98/vhcs/plan/provider/dev/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/dev/fibonacci.py` & `hcs-cli-0.1.98/vhcs/plan/provider/dev/fibonacci.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/hcs/ad.py` & `hcs-cli-0.1.98/vhcs/plan/provider/hcs/ad.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/hcs/edge.py` & `hcs-cli-0.1.98/vhcs/plan/provider/hcs/edge.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/hcs/entitlement.py` & `hcs-cli-0.1.98/vhcs/plan/provider/hcs/entitlement.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/hcs/identity_provider.py` & `hcs-cli-0.1.98/vhcs/plan/provider/hcs/identity_provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/hcs/image.py` & `hcs-cli-0.1.98/vhcs/plan/provider/hcs/image.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/hcs/pool_group.py` & `hcs-cli-0.1.98/vhcs/plan/provider/hcs/pool_group.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/hcs/pool_template.py` & `hcs-cli-0.1.98/vhcs/plan/provider/hcs/pool_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/hcs/provider.py` & `hcs-cli-0.1.98/vhcs/plan/provider/hcs/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/hcs/site.py` & `hcs-cli-0.1.98/vhcs/plan/provider/hcs/site.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/plan/provider/hcs/uag.py` & `hcs-cli-0.1.98/vhcs/plan/provider/hcs/uag.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/admin/ad.py` & `hcs-cli-0.1.98/vhcs/service/admin/ad.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/admin/azure_infra.py` & `hcs-cli-0.1.98/vhcs/service/admin/azure_infra.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/admin/edge.py` & `hcs-cli-0.1.98/vhcs/service/admin/edge.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/admin/helper.py` & `hcs-cli-0.1.98/vhcs/service/admin/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/admin/provider.py` & `hcs-cli-0.1.98/vhcs/service/admin/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/admin/template.py` & `hcs-cli-0.1.98/vhcs/service/admin/template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/admin/uag.py` & `hcs-cli-0.1.98/vhcs/service/admin/uag.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/auth/admin.py` & `hcs-cli-0.1.98/vhcs/service/auth/admin.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/ims/helper.py` & `hcs-cli-0.1.98/vhcs/service/ims/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/ims/image_copies.py` & `hcs-cli-0.1.98/vhcs/service/ims/image_copies.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/ims/images.py` & `hcs-cli-0.1.98/vhcs/service/ims/images.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/ims/version.py` & `hcs-cli-0.1.98/vhcs/service/ims/version.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/inventory/vm.py` & `hcs-cli-0.1.98/vhcs/service/inventory/vm.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/lcm/provider.py` & `hcs-cli-0.1.98/vhcs/service/lcm/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/lcm/template.py` & `hcs-cli-0.1.98/vhcs/service/lcm/template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/org_service/datacenter.py` & `hcs-cli-0.1.98/vhcs/service/org_service/datacenter.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/org_service/details.py` & `hcs-cli-0.1.98/vhcs/service/org_service/details.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/pki/certificate.py` & `hcs-cli-0.1.98/vhcs/service/pki/certificate.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/portal/entitlement.py` & `hcs-cli-0.1.98/vhcs/service/portal/entitlement.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/portal/pool.py` & `hcs-cli-0.1.98/vhcs/service/portal/pool.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/portal/site.py` & `hcs-cli-0.1.98/vhcs/service/portal/site.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/tsctl/base.py` & `hcs-cli-0.1.98/vhcs/service/tsctl/base.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/tsctl/task.py` & `hcs-cli-0.1.98/vhcs/service/tsctl/task.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/service/vmhub/otp.py` & `hcs-cli-0.1.98/vhcs/service/vmhub/otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/sglib/__init__.py` & `hcs-cli-0.1.98/vhcs/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/sglib/auth.py` & `hcs-cli-0.1.98/vhcs/sglib/auth.py`

 * *Files 24% similar despite different names*

```diff
@@ -69,23 +69,47 @@
         oauth_token = csp_client.login_with_client_id_and_secret(
             csp_config.clientId, csp_config.clientSecret, csp_config.orgId
         )
     else:
         # This should be a config from interactive login.
         # Use existing oauth_token to refresh.
         if old_oauth_token:
-            oauth_token = refresh_oauth_token(old_oauth_token, csp_config.url)
+            try:
+                oauth_token = refresh_oauth_token(old_oauth_token, csp_config.url)
+            except Exception as e:
+                oauth_token = None
+                log.warning(e)
         else:
             oauth_token = None
     return oauth_token
 
 
+_oauth_client_instance = None
+import threading
+
+_lock = threading.RLock()
+
+
 def oauth_client():
-    login(False)
-    oauth_token = profile.auth.get().token
+    global _oauth_client_instance, _lock
+    if not _oauth_client_instance:
+        with _lock:
+            if not _oauth_client_instance:
+                _oauth_client_instance = _oauth_client_impl()
+    return _oauth_client_instance
+
+
+def _oauth_client_impl():
+    oauth_token = login(False)
+
+    if not oauth_token:
+        panic(
+            "Login failed. If this is configured API key or client credential, refresh the credential from CSP and update profile config. If this is browser based interactive login, login again."
+        )
+
     csp_url = profile.current().csp.url
 
     def fn_on_new_oauth_token(token, refresh_token=None, access_token=None):
         use_oauth_token(token)
 
     if profile.current().csp.apiToken:
         # for api-token login, due to no client ID, it will fail with 400 during refresh.
```

### Comparing `hcs-cli-0.1.97/vhcs/sglib/cli_options.py` & `hcs-cli-0.1.98/vhcs/sglib/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/sglib/client_util.py` & `hcs-cli-0.1.98/vhcs/sglib/client_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/sglib/csp.py` & `hcs-cli-0.1.98/vhcs/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/sglib/ez_client.py` & `hcs-cli-0.1.98/vhcs/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/sglib/hcs_client.py` & `hcs-cli-0.1.98/vhcs/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/sglib/login_support.py` & `hcs-cli-0.1.98/vhcs/sglib/login_support.py`

 * *Files 6% similar despite different names*

```diff
@@ -261,17 +261,21 @@
         _scheduler.submit(refresh_impl, delay)
 
     delay = get_refresh_delay(oauth_token)
     _scheduler.submit(refresh_impl, delay)
 
 
 def refresh_oauth_token(old_oauth_token: dict, csp_url: str):
-    client = create_oauth_client(old_oauth_token, csp_url)
-    token_endpoint = csp_url + "/csp/gateway/am/api/auth/token"
-    new_token = client.refresh_token(token_endpoint)
+    with create_oauth_client(old_oauth_token, csp_url) as client:
+        token_endpoint = csp_url + "/csp/gateway/am/api/auth/token"
+        new_token = client.refresh_token(token_endpoint)
+        if not new_token:
+            raise Exception("CSP auth refresh failed.")
+        if "cspErrorCode" in new_token:
+            raise Exception(f"CSP auth failed: {new_token.get('message')}")
     return new_token
 
 
 # def _test():
 #     import jwt
 #     import json
 #     csp_url = 'https://console-stg.cloud.vmware.com'
```

### Comparing `hcs-cli-0.1.97/vhcs/support/daas/cidr_util.py` & `hcs-cli-0.1.98/vhcs/support/daas/cidr_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/support/daas/helper.py` & `hcs-cli-0.1.98/vhcs/support/daas/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/support/daas/infra.py` & `hcs-cli-0.1.98/vhcs/support/daas/infra.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/support/daas/infra_green.py` & `hcs-cli-0.1.98/vhcs/support/daas/infra_green.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/support/daas/infra_reuse.py` & `hcs-cli-0.1.98/vhcs/support/daas/infra_reuse.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/support/daas/templates/v1/infra-green.blueprint.yml` & `hcs-cli-0.1.98/vhcs/support/daas/templates/v1/infra-green.blueprint.yml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/support/daas/templates/v1/infra-reuse.blueprint.yml` & `hcs-cli-0.1.98/vhcs/support/daas/templates/v1/infra-reuse.blueprint.yml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/support/daas/templates/v1/tenant.blueprint.yml` & `hcs-cli-0.1.98/vhcs/support/daas/templates/v1/tenant.blueprint.yml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/support/daas/tenant_prep.py` & `hcs-cli-0.1.98/vhcs/support/daas/tenant_prep.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,19 +18,18 @@
 from vhcs.plan import PluginException
 from .cidr_util import find_available_cidr_24
 
 log = logging.getLogger(__name__)
 
 
 def process(data: dict, state: dict) -> dict:
-    import time
-
-    time.sleep(10)
     org_id = data["orgId"]
     edge = admin.edge.get(data["edgeId"], org_id)
+    if not edge:
+        raise PluginException("Edge not found: " + data["edgeId"])
     provider_id = edge["providerInstanceId"]
     # log.info('Provider: %s', provider_id)
     provider = admin.provider.get("azure", provider_id, org_id)
     if not provider:
         raise PluginException("Provider not found: " + provider_id)
     providerData = provider["providerDetails"]["data"]
     subscription_id = providerData["subscriptionId"]
```

### Comparing `hcs-cli-0.1.97/vhcs/support/daas/tenant_summary.py` & `hcs-cli-0.1.98/vhcs/support/daas/tenant_summary.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/support/plan_util.py` & `hcs-cli-0.1.98/vhcs/support/plan_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/support/profile.py` & `hcs-cli-0.1.98/vhcs/support/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/util/check_license.py` & `hcs-cli-0.1.98/vhcs/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/util/duration.py` & `hcs-cli-0.1.98/vhcs/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/util/job_view.py` & `hcs-cli-0.1.98/vhcs/util/job_view.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/util/pki_util.py` & `hcs-cli-0.1.98/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/util/query_util.py` & `hcs-cli-0.1.98/vhcs/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/util/scheduler.py` & `hcs-cli-0.1.98/vhcs/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.97/vhcs/util/versions.py` & `hcs-cli-0.1.98/vhcs/util/versions.py`

 * *Files identical despite different names*

