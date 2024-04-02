# Comparing `tmp/codemodder-0.86.2.tar.gz` & `tmp/codemodder-0.87.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codemodder-0.86.2.tar", last modified: Wed Mar 27 16:59:47 2024, max compression
+gzip compressed data, was "codemodder-0.87.0.tar", last modified: Tue Apr  2 14:47:54 2024, max compression
```

## Comparing `codemodder-0.86.2.tar` & `codemodder-0.87.0.tar`

### file list

```diff
@@ -1,459 +1,463 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.245838 codemodder-0.86.2/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-27 16:59:36.000000 codemodder-0.86.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.181838 codemodder-0.86.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-27 16:59:36.000000 codemodder-0.86.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-27 16:59:36.000000 codemodder-0.86.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-27 16:59:36.000000 codemodder-0.86.2/.github/pixeebot.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-27 16:59:36.000000 codemodder-0.86.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.181838 codemodder-0.86.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-27 16:59:36.000000 codemodder-0.86.2/.github/workflows/autoformat-pixeebot-prs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-27 16:59:36.000000 codemodder-0.86.2/.github/workflows/codemod_pygoat.yml
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-27 16:59:36.000000 codemodder-0.86.2/.github/workflows/deploy_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-27 16:59:36.000000 codemodder-0.86.2/.github/workflows/integration_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-27 16:59:36.000000 codemodder-0.86.2/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-27 16:59:36.000000 codemodder-0.86.2/.github/workflows/pre-commit-autoupdate.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-27 16:59:36.000000 codemodder-0.86.2/.github/workflows/sonar_pixee.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-27 16:59:36.000000 codemodder-0.86.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-27 16:59:36.000000 codemodder-0.86.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-27 16:59:36.000000 codemodder-0.86.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-27 16:59:36.000000 codemodder-0.86.2/.semgrepignore
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-27 16:59:36.000000 codemodder-0.86.2/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-03-27 16:59:36.000000 codemodder-0.86.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-27 16:59:36.000000 codemodder-0.86.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-27 16:59:36.000000 codemodder-0.86.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-27 16:59:36.000000 codemodder-0.86.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-27 16:59:36.000000 codemodder-0.86.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-27 16:59:36.000000 codemodder-0.86.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    44620 2024-03-27 16:59:47.245838 codemodder-0.86.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-27 16:59:36.000000 codemodder-0.86.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.181838 codemodder-0.86.2/ci_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-27 16:59:36.000000 codemodder-0.86.2/ci_tests/test_pygoat_findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-27 16:59:36.000000 codemodder-0.86.2/codecov.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.181838 codemodder-0.86.2/img/
--rw-r--r--   0 runner    (1001) docker     (127)    41511 2024-03-27 16:59:36.000000 codemodder-0.86.2/img/base-codemod.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-03-27 16:59:36.000000 codemodder-0.86.2/img/codemodder-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-03-27 16:59:36.000000 codemodder-0.86.2/img/codemodder-light.png
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-03-27 16:59:36.000000 codemodder-0.86.2/img/codemodder.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.193838 codemodder-0.86.2/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_add_requests_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_combine_startswith_endswith.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_django_session_cookie_secure_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_fix_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_lxml_safe_parser_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_multiple_codemods.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_process_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_request_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_str_concat_in_seq_literals.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_use_defusedxml.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_use_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-27 16:59:36.000000 codemodder-0.86.2/integration_tests/test_with_threading_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-03-27 16:59:36.000000 codemodder-0.86.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-27 16:59:36.000000 codemodder-0.86.2/renovate.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 16:59:47.245838 codemodder-0.86.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.177838 codemodder-0.86.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.197838 codemodder-0.86.2/src/codemodder/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-27 16:59:47.000000 codemodder-0.86.2/src/codemodder/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/code_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemodder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.197838 codemodder-0.86.2/src/codemodder/codemods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/base_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/base_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/base_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/check_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/import_modifier_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/imported_call_modifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/libcst_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/semgrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/sonar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.201838 codemodder-0.86.2/src/codemodder/codemods/test/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/test/integration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/test/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.201838 codemodder-0.86.2/src/codemodder/codemods/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/transformations/clean_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/transformations/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23555 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codemods/utils_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/codetf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.201838 codemodder-0.86.2/src/codemodder/dependency_management/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/dependency_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/dependency_management/base_dependency_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/dependency_management/codemod_dependencies.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/dependency_management/dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/dependency_management/pyproject_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/dependency_management/requirements_txt_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/dependency_management/setup_py_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/dependency_management/setupcfg_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/file_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.201838 codemodder-0.86.2/src/codemodder/project_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/project_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.201838 codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/package_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/project_analysis/python_repo_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/sarifs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.205838 codemodder-0.86.2/src/codemodder/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19714 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/scripts/generate_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/scripts/get_hashes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/semgrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/sonar_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.205838 codemodder-0.86.2/src/codemodder/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/utils/abc_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/utils/clean_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/utils/format_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/utils/linearize_string_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/codemodder/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.245838 codemodder-0.86.2/src/codemodder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44620 2024-03-27 16:59:47.000000 codemodder-0.86.2/src/codemodder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19244 2024-03-27 16:59:47.000000 codemodder-0.86.2/src/codemodder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 16:59:47.000000 codemodder-0.86.2/src/codemodder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-27 16:59:47.000000 codemodder-0.86.2/src/codemodder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-27 16:59:47.000000 codemodder-0.86.2/src/codemodder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-27 16:59:47.000000 codemodder-0.86.2/src/codemodder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.213838 codemodder-0.86.2/src/core_codemods/
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/add_requests_timeouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.213838 codemodder-0.86.2/src/core_codemods/api/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/api/core_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/combine_startswith_endswith.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/django_session_cookie_secure_off.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.221838 codemodder-0.86.2/src/core_codemods/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_add-requests-timeouts.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_django-debug-flag-on.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_django-json-response-type.md
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_django-receiver-on-top.md
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_django-session-cookie-secure-off.md
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_exception-without-raise.md
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-assert-tuple.md
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-async-task-instantiation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-hasattr-call.md
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-missing-self-or-cls.md
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-mutable-params.md
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_flask-json-response-type.md
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_harden-pickle-load.md
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_harden-pyyaml.md
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_harden-ruamel.md
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_https-connection.md
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_jwt-decode-verify.md
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_lazy-logging.md
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_limit-readline.md
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_literal-or-new-object-identity.md
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_numpy-nan-equality.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_remove-debug-breakpoint.md
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_remove-future-imports.md
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_remove-module-global.md
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_remove-unnecessary-f-str.md
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_replace-flask-send-file.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_requests-verify.md
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_sandbox-process-creation.md
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_secure-flask-cookie.md
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_secure-random.md
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_secure-tempfile.md
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_sql-parameterization.md
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_str-concat-in-sequence-literals.md
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_subprocess-shell-false.md
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_unused-imports.md
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_url-sandbox.md
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_use-defusedxml.md
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_use-generator.md
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_use-set-literal.md
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/docs/pixee_python_use-walrus-if.md
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/fix_async_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/lxml_safe_parser_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/process_creation_sandbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.221838 codemodder-0.86.2/src/core_codemods/refactor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/refactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/refactor/refactor_new_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/remove_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/requests_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/secure_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.225838 codemodder-0.86.2/src/core_codemods/sonar/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/sonar/sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/sonar/sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/sonar/sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/sonar/sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/sonar/sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/sonar/sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/sonar/sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/sonar/sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/sonar/sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/sonar/sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)    22977 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/str_concat_in_seq_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/use_defused_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/use_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-03-27 16:59:36.000000 codemodder-0.86.2/src/core_codemods/with_threading_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.225838 codemodder-0.86.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.237838 codemodder-0.86.2/tests/codemods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_add_requests_timeouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_async_fix_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_base_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_base_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_combine_startswith_endswith.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_django_session_cookie_secure_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_include_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)    23091 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_lxml_safe_parameter_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_process_creation_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_remove_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_request_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_str_concat_in_seq_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_use_defused_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/codemods/test_with_threading_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.237838 codemodder-0.86.2/tests/dependency_management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/dependency_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/dependency_management/test_base_dependency_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/dependency_management/test_dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/dependency_management/test_pyproject_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/dependency_management/test_requirements_txt_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/dependency_management/test_setup_py_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/dependency_management/test_setupcfgt_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.237838 codemodder-0.86.2/tests/project_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/project_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.241838 codemodder-0.86.2/tests/project_analysis/file_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/project_analysis/file_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/project_analysis/file_parsers/test_setup_py_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/project_analysis/test_python_repo_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.241838 codemodder-0.86.2/tests/samples/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/make_request.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/multiple_codemods.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/semgrep.sarif
--rw-r--r--   0 runner    (1001) docker     (127)    59825 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/sonar_issues.json
--rw-r--r--   0 runner    (1001) docker     (127)   451117 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/samples/webgoat_v8.2.0_codeql.sarif
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_ancestorpatterns_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_basetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_code_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_codemod_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_codemodder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_codetf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_file_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_format_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_linearize_string_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_nameresolution_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_sarif_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:47.241838 codemodder-0.86.2/tests/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/transformations/test_clean_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/transformations/test_remove_empty_string_concatenation.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-27 16:59:36.000000 codemodder-0.86.2/tests/transformations/test_remove_unused_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.246827 codemodder-0.87.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-02 14:47:41.000000 codemodder-0.87.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.174824 codemodder-0.87.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/pixeebot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.178824 codemodder-0.87.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/autoformat-pixeebot-prs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/codemod_pygoat.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/deploy_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/integration_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/pre-commit-autoupdate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/sonar_pixee.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-02 14:47:41.000000 codemodder-0.87.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-02 14:47:41.000000 codemodder-0.87.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-02 14:47:41.000000 codemodder-0.87.0/.semgrepignore
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 14:47:41.000000 codemodder-0.87.0/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-02 14:47:41.000000 codemodder-0.87.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-02 14:47:41.000000 codemodder-0.87.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 14:47:41.000000 codemodder-0.87.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-02 14:47:41.000000 codemodder-0.87.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-02 14:47:41.000000 codemodder-0.87.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-02 14:47:41.000000 codemodder-0.87.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    44628 2024-04-02 14:47:54.246827 codemodder-0.87.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-02 14:47:41.000000 codemodder-0.87.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.178824 codemodder-0.87.0/ci_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-02 14:47:41.000000 codemodder-0.87.0/ci_tests/test_pygoat_findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 14:47:41.000000 codemodder-0.87.0/codecov.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.178824 codemodder-0.87.0/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    41511 2024-04-02 14:47:41.000000 codemodder-0.87.0/img/base-codemod.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-02 14:47:41.000000 codemodder-0.87.0/img/codemodder-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-02 14:47:41.000000 codemodder-0.87.0/img/codemodder-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-02 14:47:41.000000 codemodder-0.87.0/img/codemodder.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.190825 codemodder-0.87.0/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_add_requests_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_combine_startswith_endswith.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_django_session_cookie_secure_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_lxml_safe_parser_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_multiple_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_process_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_request_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_str_concat_in_seq_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_use_defusedxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_use_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_with_threading_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-02 14:47:41.000000 codemodder-0.87.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 14:47:41.000000 codemodder-0.87.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:47:54.246827 codemodder-0.87.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.170824 codemodder-0.87.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.194825 codemodder-0.87.0/src/codemodder/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/code_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemodder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.194825 codemodder-0.87.0/src/codemodder/codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/base_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/base_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/base_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/check_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/import_modifier_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/imported_call_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/libcst_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/sonar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.198825 codemodder-0.87.0/src/codemodder/codemods/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/test/integration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/test/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.198825 codemodder-0.87.0/src/codemodder/codemods/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/transformations/clean_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/transformations/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23555 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/utils_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.198825 codemodder-0.87.0/src/codemodder/dependency_management/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/base_dependency_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/codemod_dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/pyproject_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/requirements_txt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/setup_py_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/setupcfg_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/file_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.198825 codemodder-0.87.0/src/codemodder/project_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.202825 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/package_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/python_repo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/sarifs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.202825 codemodder-0.87.0/src/codemodder/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/scripts/generate_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/scripts/get_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/sonar_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.202825 codemodder-0.87.0/src/codemodder/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/utils/abc_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/utils/clean_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/utils/format_string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/utils/linearize_string_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.246827 codemodder-0.87.0/src/codemodder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44628 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19419 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.210826 codemodder-0.87.0/src/core_codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/add_requests_timeouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.214826 codemodder-0.87.0/src/core_codemods/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/api/core_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/combine_startswith_endswith.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/django_session_cookie_secure_off.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.222826 codemodder-0.87.0/src/core_codemods/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-debug-flag-on.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-json-response-type.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-session-cookie-secure-off.md
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_exception-without-raise.md
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-assert-tuple.md
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-async-task-instantiation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-hasattr-call.md
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-missing-self-or-cls.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_harden-ruamel.md
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_https-connection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_lazy-logging.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_limit-readline.md
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_literal-or-new-object-identity.md
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_numpy-nan-equality.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-debug-breakpoint.md
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-future-imports.md
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-module-global.md
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-unnecessary-f-str.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_requests-verify.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-random.md
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-tempfile.md
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_sql-parameterization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_str-concat-in-sequence-literals.md
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_unused-imports.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_url-sandbox.md
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-defusedxml.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-generator.md
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-set-literal.md
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-walrus-if.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_async_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/lxml_safe_parser_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/process_creation_sandbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.222826 codemodder-0.87.0/src/core_codemods/refactor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/refactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/refactor/refactor_new_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/remove_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/requests_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/secure_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.222826 codemodder-0.87.0/src/core_codemods/sonar/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22977 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/str_concat_in_seq_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/use_defused_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/use_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/with_threading_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.226826 codemodder-0.87.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.238826 codemodder-0.87.0/tests/codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_add_requests_timeouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_async_fix_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_base_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_base_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_combine_startswith_endswith.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_django_session_cookie_secure_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_include_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23091 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_lxml_safe_parameter_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_process_creation_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_remove_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_request_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_str_concat_in_seq_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_use_defused_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_with_threading_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.238826 codemodder-0.87.0/tests/dependency_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/test_base_dependency_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/test_dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/test_pyproject_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/test_requirements_txt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/test_setup_py_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/test_setupcfgt_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.238826 codemodder-0.87.0/tests/project_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.242827 codemodder-0.87.0/tests/project_analysis/file_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/file_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/test_python_repo_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.242827 codemodder-0.87.0/tests/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/make_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/multiple_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/semgrep.sarif
+-rw-r--r--   0 runner    (1001) docker     (127)    77614 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/sonar_issues.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   451117 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/webgoat_v8.2.0_codeql.sarif
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_ancestorpatterns_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_basetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_code_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_codemod_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_codemodder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_codetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_file_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_format_string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_linearize_string_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_nameresolution_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_sarif_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.246827 codemodder-0.87.0/tests/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/transformations/test_clean_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/transformations/test_remove_empty_string_concatenation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/transformations/test_remove_unused_imports.py
```

### Comparing `codemodder-0.86.2/.github/workflows/autoformat-pixeebot-prs.yaml` & `codemodder-0.87.0/.github/workflows/autoformat-pixeebot-prs.yaml`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/.github/workflows/codemod_pygoat.yml` & `codemodder-0.87.0/.github/workflows/codemod_pygoat.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/.github/workflows/deploy_to_pypi.yml` & `codemodder-0.87.0/.github/workflows/deploy_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/.github/workflows/integration_test.yml` & `codemodder-0.87.0/.github/workflows/integration_test.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/.github/workflows/lint.yml` & `codemodder-0.87.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/.github/workflows/pre-commit-autoupdate.yml` & `codemodder-0.87.0/.github/workflows/pre-commit-autoupdate.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/.github/workflows/sonar_pixee.yml` & `codemodder-0.87.0/.github/workflows/sonar_pixee.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/.github/workflows/test.yml` & `codemodder-0.87.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/.gitignore` & `codemodder-0.87.0/.gitignore`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/.pre-commit-config.yaml` & `codemodder-0.87.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
          "types-jsonschema~=4.21.0",
          "types-mock==5.0.*",
          "types-PyYAML==6.0",
          "types-toml~=0.10",
          "types-requests~=2.13",
     ]
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.3.4
+  rev: v0.3.5
   hooks:
     - id: ruff
       exclude: tests/samples/
     # todo: replace black with this?
     # Run the formatter.
     # - id: ruff-format
 - repo: https://github.com/pycqa/isort
```

### Comparing `codemodder-0.86.2/CHANGELOG.md` & `codemodder-0.87.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/CONTRIBUTING.md` & `codemodder-0.87.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/LICENSE` & `codemodder-0.87.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/Makefile` & `codemodder-0.87.0/Makefile`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/PKG-INFO` & `codemodder-0.87.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codemodder
-Version: 0.86.2
+Version: 0.87.0
 Summary: A pluggable framework for building codemods in Python
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -708,15 +708,15 @@
 Requires-Dist: pytest-xdist==3.*; extra == "test"
 Requires-Dist: requests~=2.31.0; extra == "test"
 Requires-Dist: security~=1.2.0; extra == "test"
 Requires-Dist: types-mock==5.1.*; extra == "test"
 Requires-Dist: django<6,>=4; extra == "test"
 Requires-Dist: numpy~=1.26.0; extra == "test"
 Requires-Dist: flask_wtf~=1.2.0; extra == "test"
-Requires-Dist: fickling~=0.1.0; extra == "test"
+Requires-Dist: fickling>=0.1.3,~=0.1.0; extra == "test"
 Provides-Extra: complexity
 Requires-Dist: radon==6.0.*; extra == "complexity"
 Requires-Dist: xenon==0.9.*; extra == "complexity"
 Provides-Extra: all
 Requires-Dist: codemodder[test]; extra == "all"
 Requires-Dist: codemodder[complexity]; extra == "all"
```

### Comparing `codemodder-0.86.2/README.md` & `codemodder-0.87.0/README.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/ci_tests/test_pygoat_findings.py` & `codemodder-0.87.0/ci_tests/test_pygoat_findings.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/img/base-codemod.jpg` & `codemodder-0.87.0/img/base-codemod.jpg`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/img/codemodder-dark.png` & `codemodder-0.87.0/img/codemodder-dark.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/img/codemodder-light.png` & `codemodder-0.87.0/img/codemodder-light.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/img/codemodder.png` & `codemodder-0.87.0/img/codemodder.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_add_requests_timeout.py` & `codemodder-0.87.0/integration_tests/test_add_requests_timeout.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_combine_startswith_endswith.py` & `codemodder-0.87.0/integration_tests/test_combine_startswith_endswith.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_dependency_manager.py` & `codemodder-0.87.0/integration_tests/test_dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_django_debug_flag_on.py` & `codemodder-0.87.0/integration_tests/test_django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_django_json_response_type.py` & `codemodder-0.87.0/integration_tests/test_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_django_model_without_dunder_str.py` & `codemodder-0.87.0/integration_tests/test_django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_django_receiver_on_top.py` & `codemodder-0.87.0/integration_tests/test_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_django_session_cookie_secure_off.py` & `codemodder-0.87.0/integration_tests/test_django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_exception_without_raise.py` & `codemodder-0.87.0/integration_tests/test_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_file_resource_leak.py` & `codemodder-0.87.0/integration_tests/test_file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_fix_assert_tuple.py` & `codemodder-0.87.0/integration_tests/test_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_fix_dataclass_defaults.py` & `codemodder-0.87.0/integration_tests/test_fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_fix_deprecated_abstractproperty.py` & `codemodder-0.87.0/integration_tests/test_fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_fix_deprecated_logging_warn.py` & `codemodder-0.87.0/integration_tests/test_fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_fix_empty_sequence_comparison.py` & `codemodder-0.87.0/integration_tests/test_fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_fix_hasattr_call.py` & `codemodder-0.87.0/integration_tests/test_fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_fix_missing_self_or_cls.py` & `codemodder-0.87.0/integration_tests/test_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_fix_mutable_params.py` & `codemodder-0.87.0/integration_tests/test_fix_mutable_params.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_fix_task_instantiation.py` & `codemodder-0.87.0/integration_tests/test_fix_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_flask_enable_csrf_protection.py` & `codemodder-0.87.0/integration_tests/test_flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_flask_json_response_type.py` & `codemodder-0.87.0/integration_tests/test_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_harden_pickle_load.py` & `codemodder-0.87.0/integration_tests/test_harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_harden_pyyaml.py` & `codemodder-0.87.0/integration_tests/test_harden_pyyaml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_harden_ruamel.py` & `codemodder-0.87.0/integration_tests/test_harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_https_connection.py` & `codemodder-0.87.0/integration_tests/test_https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_jinja2_autoescape.py` & `codemodder-0.87.0/integration_tests/test_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_jwt_decode_verify.py` & `codemodder-0.87.0/integration_tests/test_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_lazy_logging.py` & `codemodder-0.87.0/integration_tests/test_lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_limit_readline.py` & `codemodder-0.87.0/integration_tests/test_limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_literal_or_new_object_identity.py` & `codemodder-0.87.0/integration_tests/test_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_lxml_safe_parser_defaults.py` & `codemodder-0.87.0/integration_tests/test_lxml_safe_parser_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_lxml_safe_parsing.py` & `codemodder-0.87.0/integration_tests/test_lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_multiple_codemods.py` & `codemodder-0.87.0/integration_tests/test_multiple_codemods.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_numpy_nan_equality.py` & `codemodder-0.87.0/integration_tests/test_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_order_imports.py` & `codemodder-0.87.0/integration_tests/test_order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_process_sandbox.py` & `codemodder-0.87.0/integration_tests/test_process_sandbox.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,33 +4,37 @@
 
 
 class TestProcessSandbox(BaseIntegrationTest):
     codemod = ProcessSandbox
     original_code = """
     import subprocess
 
-    subprocess.run("echo 'hi'", shell=True)
-    subprocess.run(["ls", "-l"])
+    cmd = " ".join(["ls"])
+
+    subprocess.run(cmd, shell=True)
+    subprocess.run([cmd, "-l"])
     
-    subprocess.call("echo 'hi'", shell=True)
-    subprocess.call(["ls", "-l"])
+    subprocess.call(cmd, shell=True)
+    subprocess.call([cmd, "-l"])
     
-    subprocess.check_output(["ls", "-l"])
+    subprocess.check_output([cmd, "-l"])
     
+    subprocess.run("ls -l", shell=True)
+
     var = "hello"
     """
     replacement_lines = [
         (2, """from security import safe_command\n\n"""),
-        (3, """safe_command.run(subprocess.run, "echo 'hi'", shell=True)\n"""),
-        (4, """safe_command.run(subprocess.run, ["ls", "-l"])\n"""),
-        (6, """safe_command.run(subprocess.call, "echo 'hi'", shell=True)\n"""),
-        (7, """safe_command.run(subprocess.call, ["ls", "-l"])\n"""),
+        (5, """safe_command.run(subprocess.run, cmd, shell=True)\n"""),
+        (6, """safe_command.run(subprocess.run, [cmd, "-l"])\n"""),
+        (8, """safe_command.run(subprocess.call, cmd, shell=True)\n"""),
+        (9, """safe_command.run(subprocess.call, [cmd, "-l"])\n"""),
     ]
-    expected_diff = '--- \n+++ \n@@ -1,10 +1,11 @@\n import subprocess\n+from security import safe_command\n \n-subprocess.run("echo \'hi\'", shell=True)\n-subprocess.run(["ls", "-l"])\n+safe_command.run(subprocess.run, "echo \'hi\'", shell=True)\n+safe_command.run(subprocess.run, ["ls", "-l"])\n \n-subprocess.call("echo \'hi\'", shell=True)\n-subprocess.call(["ls", "-l"])\n+safe_command.run(subprocess.call, "echo \'hi\'", shell=True)\n+safe_command.run(subprocess.call, ["ls", "-l"])\n \n subprocess.check_output(["ls", "-l"])\n \n'
-    expected_line_change = "3"
+    expected_diff = '--- \n+++ \n@@ -1,12 +1,13 @@\n import subprocess\n+from security import safe_command\n \n cmd = " ".join(["ls"])\n \n-subprocess.run(cmd, shell=True)\n-subprocess.run([cmd, "-l"])\n+safe_command.run(subprocess.run, cmd, shell=True)\n+safe_command.run(subprocess.run, [cmd, "-l"])\n \n-subprocess.call(cmd, shell=True)\n-subprocess.call([cmd, "-l"])\n+safe_command.run(subprocess.call, cmd, shell=True)\n+safe_command.run(subprocess.call, [cmd, "-l"])\n \n subprocess.check_output([cmd, "-l"])\n \n'
+    expected_line_change = "5"
     num_changes = 4
     num_changed_files = 2
     change_description = ProcessSandbox.change_description
 
     requirements_file_name = "requirements.txt"
     original_requirements = (
         "# file used to test dependency management\n"
```

### Comparing `codemodder-0.86.2/integration_tests/test_program.py` & `codemodder-0.87.0/integration_tests/test_program.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_remove_assertion_in_pytest_raises.py` & `codemodder-0.87.0/integration_tests/test_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_remove_debug_breakpoint.py` & `codemodder-0.87.0/integration_tests/test_remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_remove_future_imports.py` & `codemodder-0.87.0/integration_tests/test_remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_remove_module_global.py` & `codemodder-0.87.0/integration_tests/test_remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_remove_unused_imports.py` & `codemodder-0.87.0/integration_tests/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_replace_flask_send_file.py` & `codemodder-0.87.0/integration_tests/test_replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_request_verify.py` & `codemodder-0.87.0/integration_tests/test_request_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_secure_flask_cookie.py` & `codemodder-0.87.0/integration_tests/test_secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_secure_flask_session_config.py` & `codemodder-0.87.0/integration_tests/test_secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_secure_random.py` & `codemodder-0.87.0/integration_tests/test_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_sonar_django_json_response_type.py` & `codemodder-0.87.0/integration_tests/test_sonar_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_sonar_django_receiver_on_top.py` & `codemodder-0.87.0/integration_tests/test_sonar_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_sonar_exception_without_raise.py` & `codemodder-0.87.0/integration_tests/test_sonar_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_sonar_fix_assert_tuple.py` & `codemodder-0.87.0/integration_tests/test_sonar_fix_assert_tuple.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,11 +4,10 @@
 
 
 class TestFixAssertTuple(SonarIntegrationTest):
     codemod = SonarFixAssertTuple
     code_path = "tests/samples/fix_assert_tuple.py"
     replacement_lines = [(1, "assert 1 == 1\n"), (2, "assert 2 == 2\n")]
     expected_diff = "--- \n+++ \n@@ -1 +1,2 @@\n-assert (1 == 1, 2 == 2)\n+assert 1 == 1\n+assert 2 == 2\n"
-    sonar_issues_json = "tests/samples/sonar_issues.json"
     expected_line_change = "1"
     change_description = FixAssertTupleTransform.change_description
     num_changes = 2
```

### Comparing `codemodder-0.86.2/integration_tests/test_sonar_fix_missing_self_or_cls.py` & `codemodder-0.87.0/integration_tests/test_sonar_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_sonar_flask_json_response_type.py` & `codemodder-0.87.0/integration_tests/test_sonar_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_sonar_jwt_decode_verify.py` & `codemodder-0.87.0/integration_tests/test_sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_sonar_literal_or_new_object_identity.py` & `codemodder-0.87.0/integration_tests/test_sonar_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_sonar_numpy_nan_equality.py` & `codemodder-0.87.0/integration_tests/test_sonar_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_sonar_remove_assertion_in_pytest_raises.py` & `codemodder-0.87.0/integration_tests/test_sonar_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_sql_parameterization.py` & `codemodder-0.87.0/integration_tests/test_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_str_concat_in_seq_literals.py` & `codemodder-0.87.0/integration_tests/test_str_concat_in_seq_literals.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_subprocess_shell_false.py` & `codemodder-0.87.0/integration_tests/test_subprocess_shell_false.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_tempfile_mktemp.py` & `codemodder-0.87.0/integration_tests/test_tempfile_mktemp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from codemodder.codemods.test import BaseIntegrationTest
-from core_codemods.tempfile_mktemp import TempfileMktemp
+from core_codemods.tempfile_mktemp import TempfileMktemp, TempfileMktempTransformer
 
 
 class TestTempfileMktemp(BaseIntegrationTest):
     codemod = TempfileMktemp
     original_code = """
     import tempfile
 
     tempfile.mktemp()
     var = "hello"
     """
     replacement_lines = [(3, "tempfile.mkstemp()\n")]
     expected_diff = '--- \n+++ \n@@ -1,4 +1,4 @@\n import tempfile\n \n-tempfile.mktemp()\n+tempfile.mkstemp()\n var = "hello"\n'
     expected_line_change = "3"
-    change_description = TempfileMktemp.change_description
+    change_description = TempfileMktempTransformer.change_description
```

### Comparing `codemodder-0.86.2/integration_tests/test_unnecessary_f_str.py` & `codemodder-0.87.0/integration_tests/test_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_upgrade_sslcontext_minimum_version.py` & `codemodder-0.87.0/integration_tests/test_upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_upgrade_sslcontext_tls.py` & `codemodder-0.87.0/integration_tests/test_upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_url_sandbox.py` & `codemodder-0.87.0/integration_tests/test_url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_use_defusedxml.py` & `codemodder-0.87.0/integration_tests/test_use_defusedxml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_use_generator.py` & `codemodder-0.87.0/integration_tests/test_use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_use_set_literal.py` & `codemodder-0.87.0/integration_tests/test_use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_use_walrus_if.py` & `codemodder-0.87.0/integration_tests/test_use_walrus_if.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/integration_tests/test_with_threading_lock.py` & `codemodder-0.87.0/integration_tests/test_with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/pyproject.toml` & `codemodder-0.87.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     "pytest-xdist==3.*",
     "requests~=2.31.0",
     "security~=1.2.0",
     "types-mock==5.1.*",
     "django>=4,<6",
     "numpy~=1.26.0",
     "flask_wtf~=1.2.0",
-    "fickling~=0.1.0",
+    "fickling~=0.1.0,>=0.1.3",
 ]
 complexity = [
     "radon==6.0.*",
     "xenon==0.9.*",
 ]
 all = [
     "codemodder[test]",
```

### Comparing `codemodder-0.86.2/src/codemodder/cli.py` & `codemodder-0.87.0/src/codemodder/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,8 +170,13 @@
         help="Comma-separated set of path(s) to Sonar issues JSON file(s) to feed to the codemods",
     )
     parser.add_argument(
         "--sonar-hotspots-json",
         action=CsvListAction,
         help="Comma-separated set of path(s) to Sonar hotspots JSON file(s) to feed to the codemods",
     )
+    parser.add_argument(
+        "--defectdojo-findings-json",
+        action=CsvListAction,
+        help="Comma-separated set of path(s) to DefectDojo's v2 Findings JSON file(s) to feed to the codemods",
+    )
     return parser.parse_args(argv)
```

### Comparing `codemodder-0.86.2/src/codemodder/code_directory.py` & `codemodder-0.87.0/src/codemodder/code_directory.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemodder.py` & `codemodder-0.87.0/src/codemodder/codemodder.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemods/api.py` & `codemodder-0.87.0/src/codemodder/codemods/api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemods/base_codemod.py` & `codemodder-0.87.0/src/codemodder/codemods/base_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemods/base_transformer.py` & `codemodder-0.87.0/src/codemodder/codemods/base_transformer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemods/base_visitor.py` & `codemodder-0.87.0/src/codemodder/codemods/base_visitor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import ClassVar, Collection
 
+import libcst as cst
 from libcst import MetadataDependent
+from libcst._position import CodePosition, CodeRange
 from libcst.codemod import ContextAwareVisitor, VisitorBasedCodemodCommand
 from libcst.metadata import PositionProvider, ProviderT
 
 from codemodder.result import Result
 
 
 # TODO: this should just be part of BaseTransformer and BaseVisitor?
@@ -44,15 +46,26 @@
         pos_to_match = self.node_position(node)
         return self.filter_by_result(node) and self.filter_by_path_includes_or_excludes(
             pos_to_match
         )
 
     def node_position(self, node):
         # See https://github.com/Instagram/LibCST/blob/main/libcst/_metadata_dependent.py#L112
-        return self.get_metadata(PositionProvider, node)
+        match node:
+            case cst.FunctionDef():
+                # By default a function's position includes the entire
+                # function definition. Instead, we will only use the first line
+                # of the function definition.
+                params_end = self.get_metadata(PositionProvider, node.params).end
+                return CodeRange(
+                    start=self.get_metadata(PositionProvider, node).start,
+                    end=CodePosition(params_end.line, params_end.column + 1),
+                )
+            case _:
+                return self.get_metadata(PositionProvider, node)
 
     def lineno_for_node(self, node):
         return self.node_position(node).start.line
 
 
 class BaseTransformer(VisitorBasedCodemodCommand, UtilsMixin):
     def __init__(
```

### Comparing `codemodder-0.86.2/src/codemodder/codemods/check_annotations.py` & `codemodder-0.87.0/src/codemodder/codemods/check_annotations.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemods/import_modifier_codemod.py` & `codemodder-0.87.0/src/codemodder/codemods/import_modifier_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemods/imported_call_modifier.py` & `codemodder-0.87.0/src/codemodder/codemods/imported_call_modifier.py`

 * *Files 21% similar despite different names*

```diff
@@ -88,26 +88,7 @@
 
                 # it is a simple name, e.g. call() -> module.new_call()
                 return self.update_simple_name(
                     true_name, original_node, updated_node, new_args
                 )
 
         return updated_node
-
-    def filter_by_path_includes_or_excludes(self, pos_to_match):
-        """
-        Returns False if the node, whose position in the file is pos_to_match, matches any of the lines specified in the path-includes or path-excludes flags.
-        """
-        # excludes takes precedence if defined
-        if self.line_exclude:
-            return not any(match_line(pos_to_match, line) for line in self.line_exclude)
-        if self.line_include:
-            return any(match_line(pos_to_match, line) for line in self.line_include)
-        return True
-
-    def node_position(self, node):
-        # See https://github.com/Instagram/LibCST/blob/main/libcst/_metadata_dependent.py#L112
-        return self.get_metadata(PositionProvider, node)
-
-
-def match_line(pos, line):
-    return pos.start.line == line and pos.end.line == line
```

### Comparing `codemodder-0.86.2/src/codemodder/codemods/libcst_transformer.py` & `codemodder-0.87.0/src/codemodder/codemods/libcst_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from collections import namedtuple
 
 import libcst as cst
 from libcst import matchers
 from libcst._position import CodeRange
 from libcst.codemod import CodemodContext
 from libcst.codemod.visitors import AddImportsVisitor, RemoveImportsVisitor
-from libcst.metadata import PositionProvider
 
 from codemodder.codemods.base_transformer import BaseTransformerPipeline
 from codemodder.codemods.base_visitor import BaseTransformer
 from codemodder.codemods.utils import get_call_name
 from codemodder.codetf import Change, ChangeSet
 from codemodder.context import CodemodExecutionContext
 from codemodder.dependency import Dependency
@@ -94,18 +93,14 @@
         return self._new_or_updated_node(original_node, updated_node)
 
     def leave_ClassDef(
         self, original_node: cst.ClassDef, updated_node: cst.ClassDef
     ) -> cst.ClassDef:
         return self._new_or_updated_node(original_node, updated_node)
 
-    def node_position(self, node):
-        # See https://github.com/Instagram/LibCST/blob/main/libcst/_metadata_dependent.py#L112
-        return self.get_metadata(PositionProvider, node)
-
     def add_change(self, node, description: str, start: bool = True):
         position = self.node_position(node)
         self.add_change_from_position(position, description, start)
 
     def add_change_from_position(
         self, position: CodeRange, description: str, start: bool = True
     ):
```

### Comparing `codemodder-0.86.2/src/codemodder/codemods/semgrep.py` & `codemodder-0.87.0/src/codemodder/codemods/semgrep.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemods/sonar.py` & `codemodder-0.87.0/src/codemodder/codemods/sonar.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 
 
 class SonarCodemod(SASTCodemod):
     @property
     def origin(self):
         return "sonar"
 
+    @property
+    def rule_id(self):
+        return self._metadata.tool.rule_id
+
     @classmethod
     def from_core_codemod(
         cls,
         name: str,
         other: CoreCodemod,
         rule_id: str,
         rule_name: str,
```

### Comparing `codemodder-0.86.2/src/codemodder/codemods/test/integration_utils.py` & `codemodder-0.87.0/src/codemodder/codemods/test/integration_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 from textwrap import dedent
 from types import ModuleType
 
 import jsonschema
 
 from codemodder import __version__, registry
+from codemodder.sonar_results import SonarResultSet
 
 from .validations import execute_code
 
 
 class DependencyTestMixin:
     # Only for codemods that modify requirements should these be overridden
     requirements_file_name = ""
@@ -111,27 +112,14 @@
             f" --sonar-issues-json={self.sonar_issues_json}"
             if self.sonar_issues_json
             else ""
         )
         assert run["directory"] == os.path.abspath(self.code_dir)
         assert run["sarifs"] == []
 
-    def _assert_sonar_fields(self, result):
-        assert result["detectionTool"]["name"] == "Sonar"
-        assert (
-            result["detectionTool"]["rule"]["id"]
-            == self.codemod_instance._metadata.tool.rule_id
-        )
-        assert (
-            result["detectionTool"]["rule"]["name"]
-            == self.codemod_instance._metadata.tool.rule_name
-        )
-        # TODO: empty array until we add findings metadata
-        assert result["detectionTool"]["findings"] == []
-
     def _assert_results_fields(self, results, output_path):
         assert len(results) == 1
         result = results[0]
         assert result["codemod"] == self.codemod_instance.id
         assert result["references"] == [
             ref.model_dump(exclude_none=True)
             for ref in self.codemod_instance.references
@@ -142,21 +130,15 @@
         # TODO: if/when we add description for each url
         for reference in result["references"][
             # Last reference for Sonar has a different description
             : (-1 if self.sonar_issues_json else None)
         ]:
             assert reference["url"] == reference["description"]
 
-        if self.sonar_issues_json:
-            assert self.codemod_instance._metadata.tool is not None
-            assert (
-                result["references"][-1]["description"]
-                == self.codemod_instance._metadata.tool.rule_name
-            )
-            self._assert_sonar_fields(result)
+        self._assert_sonar_fields(result)
 
         assert len(result["changeset"]) == self.num_changed_files
 
         # A codemod may change multiple files. For now we will
         # assert the resulting data for one file only.
         change = [
             result for result in result["changeset"] if result["path"] == output_path
@@ -165,14 +147,17 @@
         assert change["diff"] == self.expected_diff
 
         assert len(change["changes"]) == self.num_changes
         line_change = change["changes"][0]
         assert line_change["lineNumber"] == int(self.expected_line_change)
         assert line_change["description"] == self.change_description
 
+    def _assert_sonar_fields(self, result):
+        del result
+
     def _assert_codetf_output(self, codetf_schema):
         with open(self.output_path, "r", encoding="utf-8") as f:
             codetf = json.load(f)
 
         jsonschema.validate(codetf, codetf_schema)
 
         assert sorted(codetf.keys()) == ["results", "run"]
@@ -273,23 +258,55 @@
         cls.output_path = tempfile.mkstemp()[1]
 
         # TODO: support sonar integration tests that add a dependency to
         # `requirements_file_name`. These tests would not be able to run
         # in parallel at this time since they would all override the same
         # tests/samples/requirements.txt file, unless we change that to
         # a temporary file.
+        cls.check_sonar_issues()
 
     @classmethod
     def teardown_class(cls):
         """Ensure any re-written file is undone after integration test class"""
         pathlib.Path(cls.output_path).unlink(missing_ok=True)
         # Revert code file
         with open(cls.code_path, mode="w", encoding="utf-8") as f:
             f.write(cls.original_code)
 
+    @classmethod
+    def check_sonar_issues(cls):
+        sonar_results = SonarResultSet.from_json(cls.sonar_issues_json)
+
+        assert (
+            cls.codemod.rule_id in sonar_results
+        ), f"Make sure to add a sonar issue for {cls.codemod.rule_id} in {cls.sonar_issues_json}"
+        results_for_codemod = sonar_results[cls.codemod.rule_id]
+        file_path = pathlib.Path(cls.code_filename)
+        assert (
+            file_path in results_for_codemod
+        ), f"Make sure to add a sonar issue for file `{cls.code_filename}` under rule `{cls.codemod.rule_id}` in {cls.sonar_issues_json}"
+
+    def _assert_sonar_fields(self, result):
+        assert self.codemod_instance._metadata.tool is not None
+        assert (
+            result["references"][-1]["description"]
+            == self.codemod_instance._metadata.tool.rule_name
+        )
+        assert result["detectionTool"]["name"] == "Sonar"
+        assert (
+            result["detectionTool"]["rule"]["id"]
+            == self.codemod_instance._metadata.tool.rule_id
+        )
+        assert (
+            result["detectionTool"]["rule"]["name"]
+            == self.codemod_instance._metadata.tool.rule_name
+        )
+        # TODO: empty array until we add findings metadata
+        assert result["detectionTool"]["findings"] == []
+
 
 def original_and_expected_from_code_path(code_path, replacements):
     """
     Returns a pair (original_code, expected) where original_code contains the contents of the code_path file and expected contains the code_path file where, for each (i,replacement) in replacements, the lines numbered i in original_code are replaced with replacement.
     """
     lines = _lines_from_codepath(code_path)
     original_raw_code = "".join(lines)
```

### Comparing `codemodder-0.86.2/src/codemodder/codemods/test/utils.py` & `codemodder-0.87.0/src/codemodder/codemods/test/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemods/test/validations.py` & `codemodder-0.87.0/src/codemodder/codemods/test/validations.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemods/transformations/clean_imports.py` & `codemodder-0.87.0/src/codemodder/codemods/transformations/clean_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py` & `codemodder-0.87.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemods/transformations/remove_unused_imports.py` & `codemodder-0.87.0/src/codemodder/codemods/transformations/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemods/utils.py` & `codemodder-0.87.0/src/codemodder/codemods/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codemods/utils_mixin.py` & `codemodder-0.87.0/src/codemodder/codemods/utils_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/codetf.py` & `codemodder-0.87.0/src/codemodder/codetf.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/context.py` & `codemodder-0.87.0/src/codemodder/context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/dependency.py` & `codemodder-0.87.0/src/codemodder/dependency.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,18 +88,18 @@
         "https://opensource.org/license/MIT/",
     ),
     oss_link="https://github.com/pixee/python-security",
     package_link="https://pypi.org/project/security/",
 )
 
 Fickling = Dependency(
-    Requirement("fickling~=0.1.0"),
+    Requirement("fickling~=0.1.0,>=0.1.3"),
     hashes=[
-        "a5bb5982e2c0e86d41fceaf9576929f0e7bfeef53998248f69c885224cf45739",
-        "1d74a9ef84e56ecd3114563907166bfa65e17e3a00190157c1514fff08e086b4",
+        "c7ad5885cd97f8c693cf7824fdbcf9d103dbacbce36546e5a031805a7261bb74",
+        "606b3153ad4b2c0338930d08a739f7f10a560f996e0bd3a4b46544417254b0d0",
     ],
     description="""This package provides analysis of pickled data to help identify potential security vulnerabilities.""",
     _license=License(
         "LGPL-3.0",
         "https://opensource.org/license/LGPL-3.0/",
     ),
     oss_link="https://github.com/trailofbits/fickling",
```

### Comparing `codemodder-0.86.2/src/codemodder/dependency_management/base_dependency_writer.py` & `codemodder-0.87.0/src/codemodder/dependency_management/base_dependency_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/dependency_management/dependency_manager.py` & `codemodder-0.87.0/src/codemodder/dependency_management/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/dependency_management/pyproject_writer.py` & `codemodder-0.87.0/src/codemodder/dependency_management/pyproject_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/dependency_management/requirements_txt_writer.py` & `codemodder-0.87.0/src/codemodder/dependency_management/requirements_txt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/dependency_management/setup_py_writer.py` & `codemodder-0.87.0/src/codemodder/dependency_management/setup_py_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/dependency_management/setupcfg_writer.py` & `codemodder-0.87.0/src/codemodder/dependency_management/setupcfg_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/diff.py` & `codemodder-0.87.0/src/codemodder/diff.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/file_context.py` & `codemodder-0.87.0/src/codemodder/file_context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/logging.py` & `codemodder-0.87.0/src/codemodder/logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/base_parser.py` & `codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/package_store.py` & `codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/package_store.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py` & `codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py` & `codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py` & `codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py` & `codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/project_analysis/python_repo_manager.py` & `codemodder-0.87.0/src/codemodder/project_analysis/python_repo_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/registry.py` & `codemodder-0.87.0/src/codemodder/registry.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/result.py` & `codemodder-0.87.0/src/codemodder/result.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/sarifs.py` & `codemodder-0.87.0/src/codemodder/sarifs.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/scripts/generate_docs.py` & `codemodder-0.87.0/src/codemodder/scripts/generate_docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,14 +310,19 @@
         need_sarif="Yes (Sonar)",
     ),
     "fix-missing-self-or-cls-S5719": DocMetadata(
         importance=CORE_METADATA["fix-missing-self-or-cls"].importance,
         guidance_explained=CORE_METADATA["fix-missing-self-or-cls"].guidance_explained,
         need_sarif="Yes (Sonar)",
     ),
+    "secure-tempfile-S5445": DocMetadata(
+        importance=CORE_METADATA["secure-tempfile"].importance,
+        guidance_explained=CORE_METADATA["secure-tempfile"].guidance_explained,
+        need_sarif="Yes (Sonar)",
+    ),
 }
 
 
 def generate_docs(codemod):
     try:
         codemod_data = METADATA[codemod.name]
     except KeyError as exc:
```

### Comparing `codemodder-0.86.2/src/codemodder/scripts/get_hashes.py` & `codemodder-0.87.0/src/codemodder/scripts/get_hashes.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/semgrep.py` & `codemodder-0.87.0/src/codemodder/semgrep.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/sonar_results.py` & `codemodder-0.87.0/src/codemodder/sonar_results.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/utils/clean_code.py` & `codemodder-0.87.0/src/codemodder/utils/clean_code.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/utils/format_string_parser.py` & `codemodder-0.87.0/src/codemodder/utils/format_string_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/utils/linearize_string_expression.py` & `codemodder-0.87.0/src/codemodder/utils/linearize_string_expression.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/utils/timer.py` & `codemodder-0.87.0/src/codemodder/utils/timer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder/utils/utils.py` & `codemodder-0.87.0/src/codemodder/utils/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/codemodder.egg-info/PKG-INFO` & `codemodder-0.87.0/src/codemodder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codemodder
-Version: 0.86.2
+Version: 0.87.0
 Summary: A pluggable framework for building codemods in Python
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -708,15 +708,15 @@
 Requires-Dist: pytest-xdist==3.*; extra == "test"
 Requires-Dist: requests~=2.31.0; extra == "test"
 Requires-Dist: security~=1.2.0; extra == "test"
 Requires-Dist: types-mock==5.1.*; extra == "test"
 Requires-Dist: django<6,>=4; extra == "test"
 Requires-Dist: numpy~=1.26.0; extra == "test"
 Requires-Dist: flask_wtf~=1.2.0; extra == "test"
-Requires-Dist: fickling~=0.1.0; extra == "test"
+Requires-Dist: fickling>=0.1.3,~=0.1.0; extra == "test"
 Provides-Extra: complexity
 Requires-Dist: radon==6.0.*; extra == "complexity"
 Requires-Dist: xenon==0.9.*; extra == "complexity"
 Provides-Extra: all
 Requires-Dist: codemodder[test]; extra == "all"
 Requires-Dist: codemodder[complexity]; extra == "all"
```

### Comparing `codemodder-0.86.2/src/codemodder.egg-info/SOURCES.txt` & `codemodder-0.87.0/src/codemodder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 integration_tests/test_sonar_fix_assert_tuple.py
 integration_tests/test_sonar_fix_missing_self_or_cls.py
 integration_tests/test_sonar_flask_json_response_type.py
 integration_tests/test_sonar_jwt_decode_verify.py
 integration_tests/test_sonar_literal_or_new_object_identity.py
 integration_tests/test_sonar_numpy_nan_equality.py
 integration_tests/test_sonar_remove_assertion_in_pytest_raises.py
+integration_tests/test_sonar_tempfile_mktemp.py
 integration_tests/test_sql_parameterization.py
 integration_tests/test_str_concat_in_seq_literals.py
 integration_tests/test_subprocess_shell_false.py
 integration_tests/test_tempfile_mktemp.py
 integration_tests/test_unnecessary_f_str.py
 integration_tests/test_upgrade_sslcontext_minimum_version.py
 integration_tests/test_upgrade_sslcontext_tls.py
@@ -299,14 +300,15 @@
 src/core_codemods/sonar/sonar_fix_assert_tuple.py
 src/core_codemods/sonar/sonar_fix_missing_self_or_cls.py
 src/core_codemods/sonar/sonar_flask_json_response_type.py
 src/core_codemods/sonar/sonar_jwt_decode_verify.py
 src/core_codemods/sonar/sonar_literal_or_new_object_identity.py
 src/core_codemods/sonar/sonar_numpy_nan_equality.py
 src/core_codemods/sonar/sonar_remove_assertion_in_pytest_raises.py
+src/core_codemods/sonar/sonar_tempfile_mktemp.py
 tests/__init__.py
 tests/conftest.py
 tests/test_ancestorpatterns_mixin.py
 tests/test_basetype.py
 tests/test_cli.py
 tests/test_code_directory.py
 tests/test_codemod_docs.py
@@ -377,14 +379,15 @@
 tests/codemods/test_sonar_fix_assert_tuple.py
 tests/codemods/test_sonar_fix_missing_self_or_cls.py
 tests/codemods/test_sonar_flask_json_response_type.py
 tests/codemods/test_sonar_jwt_decode_verify.py
 tests/codemods/test_sonar_literal_or_new_object_identity.py
 tests/codemods/test_sonar_numpy_nan_equality.py
 tests/codemods/test_sonar_remove_assertion_in_pytest_raises.py
+tests/codemods/test_sonar_tempfile_mktemp.py
 tests/codemods/test_sql_parameterization.py
 tests/codemods/test_str_concat_in_seq_literal.py
 tests/codemods/test_subprocess_shell_false.py
 tests/codemods/test_tempfile_mktemp.py
 tests/codemods/test_upgrade_sslcontext_minimum_version.py
 tests/codemods/test_upgrade_sslcontext_tls.py
 tests/codemods/test_url_sandbox.py
@@ -417,12 +420,13 @@
 tests/samples/literal_or_new_object_identity.py
 tests/samples/make_request.py
 tests/samples/multiple_codemods.py
 tests/samples/numpy_nan_equality.py
 tests/samples/remove_assertion_in_pytest_raises.py
 tests/samples/semgrep.sarif
 tests/samples/sonar_issues.json
+tests/samples/tempfile_mktemp.py
 tests/samples/webgoat_v8.2.0_codeql.sarif
 tests/transformations/__init__.py
 tests/transformations/test_clean_code.py
 tests/transformations/test_remove_empty_string_concatenation.py
 tests/transformations/test_remove_unused_imports.py
```

### Comparing `codemodder-0.86.2/src/codemodder.egg-info/requires.txt` & `codemodder-0.87.0/src/codemodder.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 pytest-xdist==3.*
 requests~=2.31.0
 security~=1.2.0
 types-mock==5.1.*
 django<6,>=4
 numpy~=1.26.0
 flask_wtf~=1.2.0
-fickling~=0.1.0
+fickling>=0.1.3,~=0.1.0
```

### Comparing `codemodder-0.86.2/src/core_codemods/__init__.py` & `codemodder-0.87.0/src/core_codemods/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 from .sonar.sonar_flask_json_response_type import SonarFlaskJsonResponseType
 from .sonar.sonar_jwt_decode_verify import SonarJwtDecodeVerify
 from .sonar.sonar_literal_or_new_object_identity import SonarLiteralOrNewObjectIdentity
 from .sonar.sonar_numpy_nan_equality import SonarNumpyNanEquality
 from .sonar.sonar_remove_assertion_in_pytest_raises import (
     SonarRemoveAssertionInPytestRaises,
 )
+from .sonar.sonar_tempfile_mktemp import SonarTempfileMktemp
 from .sql_parameterization import SQLQueryParameterization
 from .str_concat_in_seq_literal import StrConcatInSeqLiteral
 from .subprocess_shell_false import SubprocessShellFalse
 from .tempfile_mktemp import TempfileMktemp
 from .upgrade_sslcontext_minimum_version import UpgradeSSLContextMinimumVersion
 from .upgrade_sslcontext_tls import UpgradeSSLContextTLS
 from .url_sandbox import UrlSandbox
@@ -142,9 +143,10 @@
         SonarExceptionWithoutRaise,
         SonarFixAssertTuple,
         SonarRemoveAssertionInPytestRaises,
         SonarFlaskJsonResponseType,
         SonarDjangoJsonResponseType,
         SonarJwtDecodeVerify,
         SonarFixMissingSelfOrCls,
+        SonarTempfileMktemp,
     ],
 )
```

### Comparing `codemodder-0.86.2/src/core_codemods/add_requests_timeouts.py` & `codemodder-0.87.0/src/core_codemods/add_requests_timeouts.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/api/core_codemod.py` & `codemodder-0.87.0/src/core_codemods/api/core_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/combine_startswith_endswith.py` & `codemodder-0.87.0/src/core_codemods/combine_startswith_endswith.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/django_debug_flag_on.py` & `codemodder-0.87.0/src/core_codemods/django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/django_json_response_type.py` & `codemodder-0.87.0/src/core_codemods/django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/django_model_without_dunder_str.py` & `codemodder-0.87.0/src/core_codemods/django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/django_receiver_on_top.py` & `codemodder-0.87.0/src/core_codemods/django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/django_session_cookie_secure_off.py` & `codemodder-0.87.0/src/core_codemods/django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_add-requests-timeouts.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_django-json-response-type.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-json-response-type.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_django-receiver-on-top.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_fix-mutable-params.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_flask-json-response-type.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_harden-pickle-load.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_harden-pyyaml.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_harden-ruamel.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_harden-ruamel.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_jwt-decode-verify.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_lazy-logging.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_lazy-logging.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_limit-readline.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_limit-readline.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_remove-future-imports.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-future-imports.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_replace-flask-send-file.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_requests-verify.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_requests-verify.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_sandbox-process-creation.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_secure-flask-cookie.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_secure-random.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-random.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_sql-parameterization.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_sql-parameterization.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_subprocess-shell-false.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_url-sandbox.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_url-sandbox.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_use-defusedxml.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-defusedxml.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_use-generator.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-generator.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/docs/pixee_python_use-walrus-if.md` & `codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-walrus-if.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/enable_jinja2_autoescape.py` & `codemodder-0.87.0/src/core_codemods/enable_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/exception_without_raise.py` & `codemodder-0.87.0/src/core_codemods/exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/file_resource_leak.py` & `codemodder-0.87.0/src/core_codemods/file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/fix_assert_tuple.py` & `codemodder-0.87.0/src/core_codemods/fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/fix_async_task_instantiation.py` & `codemodder-0.87.0/src/core_codemods/fix_async_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/fix_dataclass_defaults.py` & `codemodder-0.87.0/src/core_codemods/fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/fix_deprecated_abstractproperty.py` & `codemodder-0.87.0/src/core_codemods/fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/fix_deprecated_logging_warn.py` & `codemodder-0.87.0/src/core_codemods/fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/fix_empty_sequence_comparison.py` & `codemodder-0.87.0/src/core_codemods/fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/fix_hasattr_call.py` & `codemodder-0.87.0/src/core_codemods/fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/fix_missing_self_or_cls.py` & `codemodder-0.87.0/src/core_codemods/fix_missing_self_or_cls.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     LibcstResultTransformer, NameAndAncestorResolutionMixin
 ):
     change_description = "Add `self` or `cls` parameter to instance or class method."
 
     def leave_FunctionDef(
         self, original_node: cst.FunctionDef, updated_node: cst.FunctionDef
     ) -> cst.FunctionDef:
-        # TODO: add filter by include or exclude that works for nodes
-        # that that have different start/end numbers.
+        if not self.node_is_selected(original_node):
+            return original_node
 
         if not self.find_immediate_class_def(original_node):
             # If `original_node` is not inside a class, nothing to do.
             return original_node
 
         if self.find_immediate_function_def(original_node):
             # If `original_node` is inside a class but also nested within a function/method
```

### Comparing `codemodder-0.86.2/src/core_codemods/fix_mutable_params.py` & `codemodder-0.87.0/src/core_codemods/fix_mutable_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,16 +163,16 @@
 
     def leave_FunctionDef(
         self,
         original_node: cst.FunctionDef,
         updated_node: cst.FunctionDef,
     ):
         """Transforms function definitions with mutable default parameters"""
-        # TODO: add filter by include or exclude that works for nodes
-        # that that have different start/end numbers.
+        if not self.node_is_selected(original_node):
+            return updated_node
 
         (
             updated_params,
             new_var_decls,
             add_annotation,
         ) = self._gather_and_update_params(original_node, updated_node)
```

### Comparing `codemodder-0.86.2/src/core_codemods/flask_enable_csrf_protection.py` & `codemodder-0.87.0/src/core_codemods/flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/flask_json_response_type.py` & `codemodder-0.87.0/src/core_codemods/flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/harden_pickle_load.py` & `codemodder-0.87.0/src/core_codemods/harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/harden_pyyaml.py` & `codemodder-0.87.0/src/core_codemods/harden_pyyaml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/harden_ruamel.py` & `codemodder-0.87.0/src/core_codemods/harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/https_connection.py` & `codemodder-0.87.0/src/core_codemods/https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/jwt_decode_verify.py` & `codemodder-0.87.0/src/core_codemods/jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/lazy_logging.py` & `codemodder-0.87.0/src/core_codemods/lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/limit_readline.py` & `codemodder-0.87.0/src/core_codemods/limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/literal_or_new_object_identity.py` & `codemodder-0.87.0/src/core_codemods/literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/lxml_safe_parser_defaults.py` & `codemodder-0.87.0/src/core_codemods/lxml_safe_parser_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/lxml_safe_parsing.py` & `codemodder-0.87.0/src/core_codemods/lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/numpy_nan_equality.py` & `codemodder-0.87.0/src/core_codemods/numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/order_imports.py` & `codemodder-0.87.0/src/core_codemods/order_imports.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import libcst as cst
 from libcst.metadata import PositionProvider
 
+from codemodder.codemods.base_visitor import UtilsMixin
 from codemodder.codemods.transformations.clean_imports import (
     GatherTopLevelImportBlocks,
     OrderImportsBlocksTransform,
 )
 from core_codemods.api import Metadata, ReviewGuidance, SimpleCodemod
 
 
-class OrderImports(SimpleCodemod):
+class OrderImports(SimpleCodemod, UtilsMixin):
     metadata = Metadata(
         name="order-imports",
         summary="Order Imports",
         review_guidance=ReviewGuidance.MERGE_WITHOUT_REVIEW,
         description="",
     )
     change_description = "Ordered and formatted import block below this line"
@@ -42,26 +43,7 @@
                 if changed:
                     self.add_change(
                         top_imports_visitor.top_imports_blocks[i][0],
                         self.change_description,
                     )
             return result_tree
         return tree
-
-    def filter_by_path_includes_or_excludes(self, pos_to_match):
-        """
-        Returns False if the node, whose position in the file is pos_to_match, matches any of the lines specified in the path-includes or path-excludes flags.
-        """
-        # excludes takes precedence if defined
-        if self.line_exclude:
-            return not any(match_line(pos_to_match, line) for line in self.line_exclude)
-        if self.line_include:
-            return any(match_line(pos_to_match, line) for line in self.line_include)
-        return True
-
-    def node_position(self, node):
-        # See https://github.com/Instagram/LibCST/blob/main/libcst/_metadata_dependent.py#L112
-        return self.get_metadata(PositionProvider, node)
-
-
-def match_line(pos, line):
-    return pos.start.line == line and pos.end.line == line
```

### Comparing `codemodder-0.86.2/src/core_codemods/process_creation_sandbox.py` & `codemodder-0.87.0/src/core_codemods/process_creation_sandbox.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,29 +23,28 @@
     )
 
     adds_dependency = True
     detector_pattern = """
         rules:
             - pattern-either:
               - patterns:
-                - pattern: subprocess.run(...)
+                - pattern: subprocess.$FUNC(...)
+                - pattern-not: subprocess.$FUNC("...", ...)
+                - pattern-not: subprocess.$FUNC(["...", ...], ...)
+                - metavariable-pattern:
+                    metavariable: $FUNC
+                    patterns:
+                    - pattern-either:
+                      - pattern: run
+                      - pattern: call
+                      - pattern: Popen
                 - pattern-inside: |
                     import subprocess
                     ...
-              - patterns:
-                - pattern: subprocess.call(...)
-                - pattern-inside: |
-                    import subprocess
-                    ...
-              - patterns:
-                - pattern: subprocess.Popen(...)
-                - pattern-inside: |
-                    import subprocess
-                    ...
-        """
+    """
 
     def on_result_found(self, original_node, updated_node):
         self.add_needed_import("security", "safe_command")
         self.add_dependency(Security)
         return self.update_call_target(
             updated_node,
             "safe_command",
```

### Comparing `codemodder-0.86.2/src/core_codemods/refactor/refactor_new_api.py` & `codemodder-0.87.0/src/core_codemods/refactor/refactor_new_api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/remove_assertion_in_pytest_raises.py` & `codemodder-0.87.0/src/core_codemods/remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/remove_debug_breakpoint.py` & `codemodder-0.87.0/src/core_codemods/remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/remove_future_imports.py` & `codemodder-0.87.0/src/core_codemods/remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/remove_module_global.py` & `codemodder-0.87.0/src/core_codemods/remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/remove_unnecessary_f_str.py` & `codemodder-0.87.0/src/core_codemods/remove_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/remove_unused_imports.py` & `codemodder-0.87.0/src/core_codemods/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/replace_flask_send_file.py` & `codemodder-0.87.0/src/core_codemods/replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/requests_verify.py` & `codemodder-0.87.0/src/core_codemods/requests_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/secure_flask_cookie.py` & `codemodder-0.87.0/src/core_codemods/secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/secure_flask_session_config.py` & `codemodder-0.87.0/src/core_codemods/secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/secure_random.py` & `codemodder-0.87.0/src/core_codemods/secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/sonar/sonar_jwt_decode_verify.py` & `codemodder-0.87.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/sql_parameterization.py` & `codemodder-0.87.0/src/core_codemods/sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/str_concat_in_seq_literal.py` & `codemodder-0.87.0/src/core_codemods/str_concat_in_seq_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/subprocess_shell_false.py` & `codemodder-0.87.0/src/core_codemods/subprocess_shell_false.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/tempfile_mktemp.py` & `codemodder-0.87.0/src/core_codemods/tempfile_mktemp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,44 @@
+from codemodder.codemods.libcst_transformer import (
+    LibcstResultTransformer,
+    LibcstTransformerPipeline,
+)
+from codemodder.codemods.semgrep import SemgrepRuleDetector
 from codemodder.codemods.utils_mixin import NameResolutionMixin
-from core_codemods.api import Metadata, Reference, ReviewGuidance, SimpleCodemod
+from core_codemods.api import CoreCodemod, Metadata, Reference, ReviewGuidance
 
 
-class TempfileMktemp(SimpleCodemod, NameResolutionMixin):
-    metadata = Metadata(
+class TempfileMktempTransformer(LibcstResultTransformer, NameResolutionMixin):
+    change_description = "Replaces `tempfile.mktemp` with `tempfile.mkstemp`."
+    _module_name = "tempfile"
+
+    def on_result_found(self, original_node, updated_node):
+        maybe_name = self.get_aliased_prefix_name(original_node, self._module_name)
+        if (maybe_name := maybe_name or self._module_name) == self._module_name:
+            self.add_needed_import(self._module_name)
+        self.remove_unused_import(original_node)
+        return self.update_call_target(updated_node, maybe_name, "mkstemp")
+
+
+TempfileMktemp = CoreCodemod(
+    metadata=Metadata(
         name="secure-tempfile",
         summary="Upgrade and Secure Temp File Creation",
         review_guidance=ReviewGuidance.MERGE_WITHOUT_REVIEW,
         references=[
             Reference(
                 url="https://docs.python.org/3/library/tempfile.html#tempfile.mktemp"
             ),
         ],
-    )
-    change_description = "Replaces `tempfile.mktemp` with `tempfile.mkstemp`."
-
-    _module_name = "tempfile"
-    detector_pattern = """
+    ),
+    detector=SemgrepRuleDetector(
+        """
         rules:
           - patterns:
             - pattern: tempfile.mktemp(...)
             - pattern-inside: |
                 import tempfile
                 ...
         """
-
-    def on_result_found(self, original_node, updated_node):
-        maybe_name = self.get_aliased_prefix_name(original_node, self._module_name)
-        if (maybe_name := maybe_name or self._module_name) == self._module_name:
-            self.add_needed_import(self._module_name)
-        self.remove_unused_import(original_node)
-        return self.update_call_target(updated_node, maybe_name, "mkstemp")
+    ),
+    transformer=LibcstTransformerPipeline(TempfileMktempTransformer),
+)
```

### Comparing `codemodder-0.86.2/src/core_codemods/upgrade_sslcontext_minimum_version.py` & `codemodder-0.87.0/src/core_codemods/upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/upgrade_sslcontext_tls.py` & `codemodder-0.87.0/src/core_codemods/upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/url_sandbox.py` & `codemodder-0.87.0/src/core_codemods/url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/use_defused_xml.py` & `codemodder-0.87.0/src/core_codemods/use_defused_xml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/use_generator.py` & `codemodder-0.87.0/src/core_codemods/use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/use_set_literal.py` & `codemodder-0.87.0/src/core_codemods/use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/use_walrus_if.py` & `codemodder-0.87.0/src/core_codemods/use_walrus_if.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/src/core_codemods/with_threading_lock.py` & `codemodder-0.87.0/src/core_codemods/with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_add_requests_timeouts.py` & `codemodder-0.87.0/tests/codemods/test_add_requests_timeouts.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_async_fix_task_instantiation.py` & `codemodder-0.87.0/tests/codemods/test_async_fix_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_base_codemod.py` & `codemodder-0.87.0/tests/codemods/test_base_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_combine_startswith_endswith.py` & `codemodder-0.87.0/tests/codemods/test_combine_startswith_endswith.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_django_debug_flag_on.py` & `codemodder-0.87.0/tests/codemods/test_django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_django_json_response_type.py` & `codemodder-0.87.0/tests/codemods/test_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_django_model_without_dunder_str.py` & `codemodder-0.87.0/tests/codemods/test_django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_django_receiver_on_top.py` & `codemodder-0.87.0/tests/codemods/test_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_django_session_cookie_secure_off.py` & `codemodder-0.87.0/tests/codemods/test_django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_enable_jinja2_autoescape.py` & `codemodder-0.87.0/tests/codemods/test_enable_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_exception_without_raise.py` & `codemodder-0.87.0/tests/codemods/test_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_file_resource_leak.py` & `codemodder-0.87.0/tests/codemods/test_file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_fix_assert_tuple.py` & `codemodder-0.87.0/tests/codemods/test_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_fix_dataclass_defaults.py` & `codemodder-0.87.0/tests/codemods/test_fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_fix_deprecated_abstractproperty.py` & `codemodder-0.87.0/tests/codemods/test_fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_fix_deprecated_logging_warn.py` & `codemodder-0.87.0/tests/codemods/test_fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_fix_empty_sequence_comparison.py` & `codemodder-0.87.0/tests/codemods/test_fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_fix_hasattr_call.py` & `codemodder-0.87.0/tests/codemods/test_fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_fix_missing_self_or_cls.py` & `codemodder-0.87.0/tests/codemods/test_fix_missing_self_or_cls.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,7 +131,23 @@
                pass
         
             @classmethod
             def kls(**kwargs):
                pass
            """
         self.run_and_assert(tmpdir, input_code, input_code)
+
+    def test_exclude_line(self, tmpdir):
+        input_code = (
+            expected
+        ) = """
+        class A:
+            def method():
+                pass
+        """
+        lines_to_exclude = [3]
+        self.run_and_assert(
+            tmpdir,
+            input_code,
+            expected,
+            lines_to_exclude=lines_to_exclude,
+        )
```

### Comparing `codemodder-0.86.2/tests/codemods/test_fix_mutable_params.py` & `codemodder-0.87.0/tests/codemods/test_fix_mutable_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,7 +288,22 @@
 
         class Foo(ABC):
             @abstractmethod
             def foo(self, bar=None):
                 pass
         """
         self.run_and_assert(tmpdir, input_code, expected_output)
+
+    def test_exclude_line(self, tmpdir):
+        input_code = (
+            expected
+        ) = """
+        def foo(one, *args, bar=[]):
+            print(bar)
+        """
+        lines_to_exclude = [2]
+        self.run_and_assert(
+            tmpdir,
+            input_code,
+            expected,
+            lines_to_exclude=lines_to_exclude,
+        )
```

### Comparing `codemodder-0.86.2/tests/codemods/test_flask_enable_csrf_protection.py` & `codemodder-0.87.0/tests/codemods/test_flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_flask_json_response_type.py` & `codemodder-0.87.0/tests/codemods/test_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_harden_pickle_load.py` & `codemodder-0.87.0/tests/codemods/test_harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_harden_pyyaml.py` & `codemodder-0.87.0/tests/codemods/test_harden_pyyaml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_harden_ruamel.py` & `codemodder-0.87.0/tests/codemods/test_harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_https_connection.py` & `codemodder-0.87.0/tests/codemods/test_https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_include_exclude.py` & `codemodder-0.87.0/tests/codemods/test_include_exclude.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_jwt_decode_verify.py` & `codemodder-0.87.0/tests/codemods/test_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_lazy_logging.py` & `codemodder-0.87.0/tests/codemods/test_lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_limit_readline.py` & `codemodder-0.87.0/tests/codemods/test_limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_literal_or_new_object_identity.py` & `codemodder-0.87.0/tests/codemods/test_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_lxml_safe_parameter_defaults.py` & `codemodder-0.87.0/tests/codemods/test_lxml_safe_parameter_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_lxml_safe_parsing.py` & `codemodder-0.87.0/tests/codemods/test_lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_numpy_nan_equality.py` & `codemodder-0.87.0/tests/codemods/test_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_order_imports.py` & `codemodder-0.87.0/tests/codemods/test_order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_remove_assertion_in_pytest_raises.py` & `codemodder-0.87.0/tests/codemods/test_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_remove_debug_breakpoint.py` & `codemodder-0.87.0/tests/codemods/test_remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_remove_future_imports.py` & `codemodder-0.87.0/tests/codemods/test_remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_remove_module_global.py` & `codemodder-0.87.0/tests/codemods/test_remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_remove_unnecessary_f_str.py` & `codemodder-0.87.0/tests/codemods/test_remove_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_remove_unused_imports.py` & `codemodder-0.87.0/tests/codemods/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_replace_flask_send_file.py` & `codemodder-0.87.0/tests/codemods/test_replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_request_verify.py` & `codemodder-0.87.0/tests/codemods/test_request_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_secure_flask_cookie.py` & `codemodder-0.87.0/tests/codemods/test_secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_secure_flask_session_config.py` & `codemodder-0.87.0/tests/codemods/test_secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_secure_random.py` & `codemodder-0.87.0/tests/codemods/test_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_sonar_django_json_response_type.py` & `codemodder-0.87.0/tests/codemods/test_sonar_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_sonar_django_receiver_on_top.py` & `codemodder-0.87.0/tests/codemods/test_sonar_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_sonar_exception_without_raise.py` & `codemodder-0.87.0/tests/codemods/test_sonar_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_sonar_fix_assert_tuple.py` & `codemodder-0.87.0/tests/codemods/test_sonar_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_sonar_fix_missing_self_or_cls.py` & `codemodder-0.87.0/tests/codemods/test_sonar_fix_missing_self_or_cls.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,50 +10,50 @@
 
     def test_name(self):
         assert self.codemod.name == "fix-missing-self-or-cls-S5719"
 
     def test_simple(self, tmpdir):
         input_code = """
         class A:
-            def method():
+            def instance_method():
                 pass
             
             @classmethod
-            def clsmethod():
+            def class_method():
                 pass
         """
         expected_output = """
         class A:
-            def method(self):
+            def instance_method(self):
                 pass
             
             @classmethod
-            def clsmethod(cls):
+            def class_method(cls):
                 pass
         """
         issues = {
             "issues": [
                 {
                     "rule": "python:S5719",
                     "status": "OPEN",
                     "component": "code.py",
                     "textRange": {
-                        "startLine": 2,
-                        "endLine": 2,
+                        "startLine": 3,
+                        "endLine": 3,
                         "startOffset": 4,
                         "endOffset": 25,
                     },
                 },
                 {
                     "rule": "python:S5719",
                     "status": "OPEN",
                     "component": "code.py",
                     "textRange": {
-                        "startLine": 6,
-                        "endLine": 6,
+                        "startLine": 7,
+                        "endLine": 7,
                         "startOffset": 4,
                         "endOffset": 22,
                     },
                 },
             ]
         }
         self.run_and_assert(
```

### Comparing `codemodder-0.86.2/tests/codemods/test_sonar_flask_json_response_type.py` & `codemodder-0.87.0/tests/codemods/test_sonar_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_sonar_jwt_decode_verify.py` & `codemodder-0.87.0/tests/codemods/test_sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_sonar_literal_or_new_object_identity.py` & `codemodder-0.87.0/tests/codemods/test_sonar_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_sonar_numpy_nan_equality.py` & `codemodder-0.87.0/tests/codemods/test_sonar_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_sonar_remove_assertion_in_pytest_raises.py` & `codemodder-0.87.0/tests/codemods/test_sonar_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_sql_parameterization.py` & `codemodder-0.87.0/tests/codemods/test_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_str_concat_in_seq_literal.py` & `codemodder-0.87.0/tests/codemods/test_str_concat_in_seq_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_subprocess_shell_false.py` & `codemodder-0.87.0/tests/codemods/test_subprocess_shell_false.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_tempfile_mktemp.py` & `codemodder-0.87.0/tests/codemods/test_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_upgrade_sslcontext_minimum_version.py` & `codemodder-0.87.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_upgrade_sslcontext_tls.py` & `codemodder-0.87.0/tests/codemods/test_upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_url_sandbox.py` & `codemodder-0.87.0/tests/codemods/test_url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_use_defused_xml.py` & `codemodder-0.87.0/tests/codemods/test_use_defused_xml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_use_generator.py` & `codemodder-0.87.0/tests/codemods/test_use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_use_set_literal.py` & `codemodder-0.87.0/tests/codemods/test_use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_walrus_if.py` & `codemodder-0.87.0/tests/codemods/test_walrus_if.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/codemods/test_with_threading_lock.py` & `codemodder-0.87.0/tests/codemods/test_with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/conftest.py` & `codemodder-0.87.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/dependency_management/test_base_dependency_writer.py` & `codemodder-0.87.0/tests/dependency_management/test_base_dependency_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/dependency_management/test_dependency_manager.py` & `codemodder-0.87.0/tests/dependency_management/test_dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/dependency_management/test_pyproject_writer.py` & `codemodder-0.87.0/tests/dependency_management/test_pyproject_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/dependency_management/test_requirements_txt_writer.py` & `codemodder-0.87.0/tests/dependency_management/test_requirements_txt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/dependency_management/test_setup_py_writer.py` & `codemodder-0.87.0/tests/dependency_management/test_setup_py_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/dependency_management/test_setupcfgt_writer.py` & `codemodder-0.87.0/tests/dependency_management/test_setupcfgt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py` & `codemodder-0.87.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py` & `codemodder-0.87.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py` & `codemodder-0.87.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/project_analysis/file_parsers/test_setup_py_file_parser.py` & `codemodder-0.87.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/samples/semgrep.sarif` & `codemodder-0.87.0/tests/samples/semgrep.sarif`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/samples/webgoat_v8.2.0_codeql.sarif` & `codemodder-0.87.0/tests/samples/webgoat_v8.2.0_codeql.sarif`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_ancestorpatterns_mixin.py` & `codemodder-0.87.0/tests/test_ancestorpatterns_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_basetype.py` & `codemodder-0.87.0/tests/test_basetype.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_cli.py` & `codemodder-0.87.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_code_directory.py` & `codemodder-0.87.0/tests/test_code_directory.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_codemod_docs.py` & `codemodder-0.87.0/tests/test_codemod_docs.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_codemodder.py` & `codemodder-0.87.0/tests/test_codemodder.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_codetf.py` & `codemodder-0.87.0/tests/test_codetf.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_context.py` & `codemodder-0.87.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_format_string_parser.py` & `codemodder-0.87.0/tests/test_format_string_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_linearize_string_expression.py` & `codemodder-0.87.0/tests/test_linearize_string_expression.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_logging.py` & `codemodder-0.87.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_nameresolution_mixin.py` & `codemodder-0.87.0/tests/test_nameresolution_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_results.py` & `codemodder-0.87.0/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/test_sarif_processing.py` & `codemodder-0.87.0/tests/test_sarif_processing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/transformations/test_clean_code.py` & `codemodder-0.87.0/tests/transformations/test_clean_code.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/transformations/test_remove_empty_string_concatenation.py` & `codemodder-0.87.0/tests/transformations/test_remove_empty_string_concatenation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.86.2/tests/transformations/test_remove_unused_imports.py` & `codemodder-0.87.0/tests/transformations/test_remove_unused_imports.py`

 * *Files identical despite different names*

