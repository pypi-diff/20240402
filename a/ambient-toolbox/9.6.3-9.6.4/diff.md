# Comparing `tmp/ambient_toolbox-9.6.3.tar.gz` & `tmp/ambient_toolbox-9.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_toolbox-9.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ambient_toolbox-9.6.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ambient_toolbox-9.6.3.tar` & `ambient_toolbox-9.6.4.tar`

### file list

```diff
@@ -1,235 +1,235 @@
--rw-r--r--   0        0        0     3647 2024-02-28 11:40:45.710992 ambient_toolbox-9.6.3/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0      320 2024-02-28 11:13:49.957009 ambient_toolbox-9.6.3/.coveragerc
--rw-r--r--   0        0        0      288 2024-02-28 11:13:49.958009 ambient_toolbox-9.6.3/.editorconfig
--rw-r--r--   0        0        0     2757 2024-02-29 15:04:25.126139 ambient_toolbox-9.6.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3280 2024-02-29 15:01:43.481662 ambient_toolbox-9.6.3/.gitignore
--rw-r--r--   0        0        0      669 2024-02-28 11:40:45.712026 ambient_toolbox-9.6.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      773 2024-02-28 11:13:49.963008 ambient_toolbox-9.6.3/.readthedocs.yaml
--rw-r--r--   0        0        0    23195 2024-03-04 08:25:42.963673 ambient_toolbox-9.6.3/CHANGES.md
--rw-r--r--   0        0        0      934 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/Dockerfile
--rw-r--r--   0        0        0     1102 2024-02-28 11:13:49.995008 ambient_toolbox-9.6.3/LICENSE.md
--rw-r--r--   0        0        0      134 2024-02-28 11:13:49.964014 ambient_toolbox-9.6.3/MANIFEST.in
--rw-r--r--   0        0        0     6471 2024-02-28 11:13:49.980015 ambient_toolbox-9.6.3/README.md
--rw-r--r--   0        0        0      119 2024-03-04 08:25:42.969588 ambient_toolbox-9.6.3/ambient_toolbox/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/admin/model_admins/__init__.py
--rw-r--r--   0        0        0     1594 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.3/ambient_toolbox/admin/model_admins/classes.py
--rw-r--r--   0        0        0      795 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.3/ambient_toolbox/admin/model_admins/inlines.py
--rw-r--r--   0        0        0     4971 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.3/ambient_toolbox/admin/model_admins/mixins.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/admin/views/__init__.py
--rw-r--r--   0        0        0     1085 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.3/ambient_toolbox/admin/views/forms.py
--rw-r--r--   0        0        0     2366 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.3/ambient_toolbox/admin/views/mixins.py
--rw-r--r--   0        0        0      199 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.3/ambient_toolbox/apps.py
--rw-r--r--   0        0        0      913 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/context_manager.py
--rw-r--r--   0        0        0      142 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.3/ambient_toolbox/context_processors.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/drf/__init__.py
--rw-r--r--   0        0        0     1006 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.3/ambient_toolbox/drf/fields.py
--rw-r--r--   0        0        0     1109 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.3/ambient_toolbox/drf/serializers.py
--rw-r--r--   0        0        0     3150 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.3/ambient_toolbox/drf/tests.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/gitlab/__init__.py
--rw-r--r--   0        0        0    13666 2024-02-28 11:40:45.714060 ambient_toolbox-9.6.3/ambient_toolbox/gitlab/coverage.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/graphql/forms/__init__.py
--rw-r--r--   0        0        0     1636 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.3/ambient_toolbox/graphql/forms/mutations.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/graphql/schemes/__init__.py
--rw-r--r--   0        0        0     1996 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/graphql/schemes/mutations.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/graphql/sentry/__init__.py
--rw-r--r--   0        0        0      407 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/graphql/sentry/utils.py
--rw-r--r--   0        0        0     1307 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/graphql/sentry/views.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/graphql/tests/__init__.py
--rw-r--r--   0        0        0     2087 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/graphql/tests/base_test.py
--rw-r--r--   0        0        0     1538 2023-11-27 08:56:40.000000 ambient_toolbox-9.6.3/ambient_toolbox/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2498 2023-11-27 08:56:35.477473 ambient_toolbox-9.6.3/ambient_toolbox/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/mail/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/mail/backends/__init__.py
--rw-r--r--   0        0        0     3155 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/mail/backends/whitelist_smtp.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/management/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/management/commands/__init__.py
--rw-r--r--   0        0        0     1277 2024-03-04 07:18:44.573653 ambient_toolbox-9.6.3/ambient_toolbox/management/commands/create_translation_file.py
--rw-r--r--   0        0        0     1743 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/management/commands/install_permission_fixtures.py
--rw-r--r--   0        0        0      294 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/management/commands/validate_test_structure.py
--rw-r--r--   0        0        0     2478 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/managers.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/middleware/__init__.py
--rw-r--r--   0        0        0      889 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/middleware/current_request.py
--rw-r--r--   0        0        0      977 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/middleware/current_user.py
--rw-r--r--   0        0        0        0 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/mixins/__init__.py
--rw-r--r--   0        0        0     1886 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/mixins/bleacher.py
--rw-r--r--   0        0        0     1340 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/mixins/models.py
--rw-r--r--   0        0        0      238 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/mixins/validation.py
--rw-r--r--   0        0        0     2971 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/models.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/permissions/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/permissions/fixtures/__init__.py
--rw-r--r--   0        0        0      292 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/permissions/fixtures/declarations.py
--rw-r--r--   0        0        0      232 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/permissions/fixtures/helpers.py
--rw-r--r--   0        0        0     3235 2024-01-22 10:18:06.671277 ambient_toolbox-9.6.3/ambient_toolbox/permissions/fixtures/services.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/selectors/__init__.py
--rw-r--r--   0        0        0      351 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/selectors/base.py
--rw-r--r--   0        0        0     1027 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/selectors/permission.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.3/ambient_toolbox/sentry/__init__.py
--rw-r--r--   0        0        0     2164 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/sentry/helpers.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.3/ambient_toolbox/services/__init__.py
--rw-r--r--   0        0        0     3324 2024-02-02 15:54:55.522564 ambient_toolbox-9.6.3/ambient_toolbox/services/custom_scrubber.py
--rw-r--r--   0        0        0        0 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/templatetags/__init__.py
--rw-r--r--   0        0        0      229 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.3/ambient_toolbox/templatetags/ai_date_tags.py
--rw-r--r--   0        0        0      647 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/templatetags/ai_email_tags.py
--rw-r--r--   0        0        0      771 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/templatetags/ai_file_tags.py
--rw-r--r--   0        0        0      185 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.3/ambient_toolbox/templatetags/ai_helper_tags.py
--rw-r--r--   0        0        0     1165 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/templatetags/ai_number_tags.py
--rw-r--r--   0        0        0      364 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/templatetags/ai_object_tags.py
--rw-r--r--   0        0        0      620 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/templatetags/ai_string_tags.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.3/ambient_toolbox/tests/__init__.py
--rw-r--r--   0        0        0       58 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.3/ambient_toolbox/tests/errors.py
--rw-r--r--   0        0        0     5466 2024-02-02 15:54:07.436787 ambient_toolbox-9.6.3/ambient_toolbox/tests/mixins.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.3/ambient_toolbox/tests/structure_validator/__init__.py
--rw-r--r--   0        0        0      386 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/tests/structure_validator/settings.py
--rw-r--r--   0        0        0     4527 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/tests/structure_validator/test_structure_validator.py
--rw-r--r--   0        0        0      219 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.3/ambient_toolbox/utils/__init__.py
--rw-r--r--   0        0        0      119 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.3/ambient_toolbox/utils/cache.py
--rw-r--r--   0        0        0     5804 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/utils/date.py
--rw-r--r--   0        0        0     1383 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/utils/file.py
--rw-r--r--   0        0        0      331 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/utils/log_whodid.py
--rw-r--r--   0        0        0      557 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.3/ambient_toolbox/utils/math.py
--rw-r--r--   0        0        0      904 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/utils/model.py
--rw-r--r--   0        0        0     3822 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/utils/named_tuple.py
--rw-r--r--   0        0        0     3826 2024-02-28 11:40:45.714060 ambient_toolbox-9.6.3/ambient_toolbox/utils/string.py
--rw-r--r--   0        0        0        0 2023-11-24 13:16:44.820233 ambient_toolbox-9.6.3/ambient_toolbox/validators/__init__.py
--rw-r--r--   0        0        0        0 2023-11-24 13:16:44.820233 ambient_toolbox-9.6.3/ambient_toolbox/validators/auth_password/__init__.py
--rw-r--r--   0        0        0      651 2023-11-24 13:16:44.820233 ambient_toolbox-9.6.3/ambient_toolbox/validators/auth_password/special_chars.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.3/ambient_toolbox/view_layer/__init__.py
--rw-r--r--   0        0        0      728 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/view_layer/form_mixins.py
--rw-r--r--   0        0        0      473 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/view_layer/formset_mixins.py
--rw-r--r--   0        0        0     2910 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/view_layer/formset_view_mixin.py
--rw-r--r--   0        0        0     1539 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/view_layer/htmx_mixins.py
--rw-r--r--   0        0        0     2094 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/view_layer/mixins.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/ambient_toolbox/view_layer/tests/__init__.py
--rw-r--r--   0        0        0     4031 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/view_layer/tests/mixins.py
--rw-r--r--   0        0        0     1823 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/ambient_toolbox/view_layer/views.py
--rw-r--r--   0        0        0      654 2024-02-28 11:13:49.989008 ambient_toolbox-9.6.3/docs/Makefile
--rw-r--r--   0        0        0     2809 2024-02-28 11:40:45.714060 ambient_toolbox-9.6.3/docs/conf.py
--rw-r--r--   0        0        0     5945 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/admin.md
--rw-r--r--   0        0        0       33 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/changelog.rst
--rw-r--r--   0        0        0     2225 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/context_manager.md
--rw-r--r--   0        0        0      528 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/context_processors.md
--rw-r--r--   0        0        0     7103 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/database_anonymisation.md
--rw-r--r--   0        0        0     6612 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/djangorestframework.md
--rw-r--r--   0        0        0     2489 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/docs/features/gitlab.md
--rw-r--r--   0        0        0     6341 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/graphql.md
--rw-r--r--   0        0        0      999 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/mail.md
--rw-r--r--   0        0        0     5719 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/managers.md
--rw-r--r--   0        0        0     5802 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/mixins.md
--rw-r--r--   0        0        0     2394 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/models.md
--rw-r--r--   0        0        0     6340 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/permissions.md
--rw-r--r--   0        0        0     4327 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/selectors.md
--rw-r--r--   0        0        0     3224 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/sentry.md
--rw-r--r--   0        0        0     4858 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/services.md
--rw-r--r--   0        0        0     1512 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/setup.md
--rw-r--r--   0        0        0     5346 2024-01-12 08:49:19.726688 ambient_toolbox-9.6.3/docs/features/tests.md
--rw-r--r--   0        0        0     1969 2024-03-04 08:25:42.940504 ambient_toolbox-9.6.3/docs/features/translations.md
--rw-r--r--   0        0        0      223 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/utils.rst
--rw-r--r--   0        0        0      508 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/utils/cache.md
--rw-r--r--   0        0        0     7189 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/utils/date.md
--rw-r--r--   0        0        0      710 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/utils/math.md
--rw-r--r--   0        0        0     1061 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/utils/model.md
--rw-r--r--   0        0        0     2298 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/utils/named_tuple.md
--rw-r--r--   0        0        0     5640 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/utils/string.md
--rw-r--r--   0        0        0      824 2023-11-27 08:55:29.443896 ambient_toolbox-9.6.3/docs/features/validators.md
--rw-r--r--   0        0        0    15031 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.3/docs/features/view-layer.md
--rw-r--r--   0        0        0     1241 2024-02-29 15:04:25.128235 ambient_toolbox-9.6.3/docs/index.rst
--rwxr-xr-x   0        0        0      795 2024-02-28 11:13:49.988008 ambient_toolbox-9.6.3/docs/make.bat
--rw-r--r--   0        0        0      655 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/manage.py
--rw-r--r--   0        0        0     5892 2024-02-29 13:35:32.328102 ambient_toolbox-9.6.3/pyproject.toml
--rw-r--r--   0        0        0       56 2024-02-28 11:13:49.972009 ambient_toolbox-9.6.3/pytest.ini
--rw-r--r--   0        0        0      151 2024-02-28 11:13:49.991008 ambient_toolbox-9.6.3/scripts/unix/install_requirements.sh
--rw-r--r--   0        0        0       50 2024-02-28 11:13:49.992009 ambient_toolbox-9.6.3/scripts/unix/publish_to_pypi.sh
--rw-r--r--   0        0        0      151 2024-02-28 11:13:49.993010 ambient_toolbox-9.6.3/scripts/windows/install_requirements.ps1
--rw-r--r--   0        0        0       50 2024-02-28 11:13:49.994009 ambient_toolbox-9.6.3/scripts/windows/publish_to_pypi.ps1
--rw-r--r--   0        0        0     1896 2024-02-29 15:04:25.129284 ambient_toolbox-9.6.3/settings.py
--rw-r--r--   0        0        0      281 2024-02-28 11:13:49.981010 ambient_toolbox-9.6.3/setup.cfg
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/api/__init__.py
--rw-r--r--   0        0        0      275 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/testapp/api/serializers.py
--rw-r--r--   0        0        0      251 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/testapp/api/urls.py
--rw-r--r--   0        0        0      510 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/api/views.py
--rw-r--r--   0        0        0      210 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/testapp/forms.py
--rw-r--r--   0        0        0       92 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/managers.py
--rw-r--r--   0        0        0     6057 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/testapp/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/migrations/__init__.py
--rw-r--r--   0        0        0     3292 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/testapp/models.py
--rw-r--r--   0        0        0      406 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/testapp/permissions.py
--rw-r--r--   0        0        0      157 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/selectors.py
--rw-r--r--   0        0        0     1390 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/templates/403.html
--rw-r--r--   0        0        0      134 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/templates/testapp/test_template.html
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/tests/missing_init/test_ok.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/tests/subdirectory/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/tests/subdirectory/missing_test_prefix.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/tests/subdirectory/test_ok.py
--rw-r--r--   0        0        0      554 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.3/testapp/urls.py
--rw-r--r--   0        0        0      491 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/testapp/views.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/__init__.py
--rw-r--r--   0        0        0     2778 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
--rw-r--r--   0        0        0     1848 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
--rw-r--r--   0        0        0     1639 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
--rw-r--r--   0        0        0     1150 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
--rw-r--r--   0        0        0     4773 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_classes.py
--rw-r--r--   0        0        0     3792 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
--rw-r--r--   0        0        0     1446 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
--rw-r--r--   0        0        0     1854 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/ambient_toolbox/__init__.py
--rw-r--r--   0        0        0     7631 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/ambient_toolbox/test_test_structure_validator.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/drf/__init__.py
--rw-r--r--   0        0        0     3052 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/drf/test_fields.py
--rw-r--r--   0        0        0        0 2024-02-28 11:40:45.715077 ambient_toolbox-9.6.3/tests/gitlab/__init__.py
--rw-r--r--   0        0        0     1486 2024-02-28 11:40:45.715077 ambient_toolbox-9.6.3/tests/gitlab/test_coverage.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/mixins/__init__.py
--rw-r--r--   0        0        0      459 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/mixins/test_validation.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/permissions/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/permissions/fixtures/__init__.py
--rw-r--r--   0        0        0     1064 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/permissions/fixtures/test_declarations.py
--rw-r--r--   0        0        0      564 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/permissions/fixtures/test_helpers.py
--rw-r--r--   0        0        0     7053 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/permissions/fixtures/test_services_setup_service.py
--rw-r--r--   0        0        0     1466 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/permissions/test_install_permission_fixtures_command.py
--rw-r--r--   0        0        0      485 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/query_selectors/test_base.py
--rw-r--r--   0        0        0     1581 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/query_selectors/test_permission.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/selectors/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/sentry/__init__.py
--rw-r--r--   0        0        0     6048 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/sentry/mock_data.py
--rw-r--r--   0        0        0     1548 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/sentry/test_sentry_helper.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/templatetags/__init__.py
--rw-r--r--   0        0        0     1101 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/templatetags/test_ai_number_tags.py
--rw-r--r--   0        0        0      620 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/test_admin_forms.py
--rw-r--r--   0        0        0     1574 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/test_admin_inlines.py
--rw-r--r--   0        0        0     2829 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/test_admin_view_mixins.py
--rw-r--r--   0        0        0     2150 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/test_context_manager.py
--rw-r--r--   0        0        0      796 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/test_log_whodid.py
--rw-r--r--   0        0        0     3179 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/test_managers.py
--rw-r--r--   0        0        0     1581 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/test_math.py
--rw-r--r--   0        0        0     4121 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/test_middleware.py
--rw-r--r--   0        0        0     1163 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.3/tests/test_mixins_models.py
--rw-r--r--   0        0        0     2840 2023-12-05 10:03:55.292807 ambient_toolbox-9.6.3/tests/test_models.py
--rw-r--r--   0        0        0     1730 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/test_rest_api_mixins.py
--rw-r--r--   0        0        0     1157 2024-02-02 15:54:55.523069 ambient_toolbox-9.6.3/tests/test_scrubbing_service.py
--rw-r--r--   0        0        0      280 2023-10-22 11:06:15.893086 ambient_toolbox-9.6.3/tests/test_utils_cache.py
--rw-r--r--   0        0        0    12473 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/test_utils_date.py
--rw-r--r--   0        0        0     1839 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/test_utils_file.py
--rw-r--r--   0        0        0     1275 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/test_utils_model.py
--rw-r--r--   0        0        0     4112 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/test_utils_named_tuple.py
--rw-r--r--   0        0        0     5356 2024-02-28 11:21:15.672002 ambient_toolbox-9.6.3/tests/test_utils_string.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.893086 ambient_toolbox-9.6.3/tests/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.893086 ambient_toolbox-9.6.3/tests/tests/mixins/__init__.py
--rw-r--r--   0        0        0     1250 2024-02-02 16:00:03.078374 ambient_toolbox-9.6.3/tests/tests/mixins/test_django_message_framework.py
--rw-r--r--   0        0        0     1955 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/tests/mixins/test_mixins.py
--rw-r--r--   0        0        0      229 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/tests/mixins/test_models.py
--rw-r--r--   0        0        0     2418 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/tests/mixins/test_request_provider_mixin.py
--rw-r--r--   0        0        0     2711 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/tests/test_mail_backends.py
--rw-r--r--   0        0        0        0 2023-11-24 13:16:44.820233 ambient_toolbox-9.6.3/tests/validators/__init__.py
--rw-r--r--   0        0        0        0 2023-11-24 13:16:44.820233 ambient_toolbox-9.6.3/tests/validators/auth_password/__init__.py
--rw-r--r--   0        0        0     1443 2023-11-24 13:16:44.820233 ambient_toolbox-9.6.3/tests/validators/auth_password/test_special_chars.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:15.893086 ambient_toolbox-9.6.3/tests/view_layer/__init__.py
--rw-r--r--   0        0        0     1834 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/view_layer/test_formset_mixins.py
--rw-r--r--   0        0        0     1518 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/view_layer/test_htmx_response_mixin.py
--rw-r--r--   0        0        0     4426 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/view_layer/test_meta_mixins.py
--rw-r--r--   0        0        0     1325 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.3/tests/view_layer/test_views.py
--rw-r--r--   0        0        0     9015 1970-01-01 00:00:00.000000 ambient_toolbox-9.6.3/PKG-INFO
+-rw-r--r--   0        0        0     3713 2024-03-28 09:47:09.481466 ambient_toolbox-9.6.4/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0      320 2024-03-28 09:27:28.880891 ambient_toolbox-9.6.4/.coveragerc
+-rw-r--r--   0        0        0      288 2024-03-28 09:27:28.881924 ambient_toolbox-9.6.4/.editorconfig
+-rw-r--r--   0        0        0     2768 2024-03-28 09:47:09.481466 ambient_toolbox-9.6.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3280 2024-02-29 15:01:43.481662 ambient_toolbox-9.6.4/.gitignore
+-rw-r--r--   0        0        0      669 2024-03-28 09:27:28.884066 ambient_toolbox-9.6.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      773 2024-03-28 09:27:28.885051 ambient_toolbox-9.6.4/.readthedocs.yaml
+-rw-r--r--   0        0        0    23440 2024-03-28 09:47:09.481466 ambient_toolbox-9.6.4/CHANGES.md
+-rw-r--r--   0        0        0      934 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/Dockerfile
+-rw-r--r--   0        0        0     1102 2024-03-28 09:27:28.915313 ambient_toolbox-9.6.4/LICENSE.md
+-rw-r--r--   0        0        0      134 2024-03-28 09:27:28.886051 ambient_toolbox-9.6.4/MANIFEST.in
+-rw-r--r--   0        0        0     6471 2024-03-28 09:47:09.481466 ambient_toolbox-9.6.4/README.md
+-rw-r--r--   0        0        0      119 2024-03-28 09:47:09.481466 ambient_toolbox-9.6.4/ambient_toolbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/admin/model_admins/__init__.py
+-rw-r--r--   0        0        0     1594 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.4/ambient_toolbox/admin/model_admins/classes.py
+-rw-r--r--   0        0        0      795 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.4/ambient_toolbox/admin/model_admins/inlines.py
+-rw-r--r--   0        0        0     4971 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.4/ambient_toolbox/admin/model_admins/mixins.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/admin/views/__init__.py
+-rw-r--r--   0        0        0     1085 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.4/ambient_toolbox/admin/views/forms.py
+-rw-r--r--   0        0        0     2366 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.4/ambient_toolbox/admin/views/mixins.py
+-rw-r--r--   0        0        0      199 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.4/ambient_toolbox/apps.py
+-rw-r--r--   0        0        0      913 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/context_manager.py
+-rw-r--r--   0        0        0      142 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.4/ambient_toolbox/context_processors.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/drf/__init__.py
+-rw-r--r--   0        0        0     1006 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.4/ambient_toolbox/drf/fields.py
+-rw-r--r--   0        0        0     1109 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.4/ambient_toolbox/drf/serializers.py
+-rw-r--r--   0        0        0     3150 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.4/ambient_toolbox/drf/tests.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/gitlab/__init__.py
+-rw-r--r--   0        0        0    13666 2024-02-28 11:40:45.714060 ambient_toolbox-9.6.4/ambient_toolbox/gitlab/coverage.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/graphql/forms/__init__.py
+-rw-r--r--   0        0        0     1636 2023-11-21 10:36:16.877967 ambient_toolbox-9.6.4/ambient_toolbox/graphql/forms/mutations.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/graphql/schemes/__init__.py
+-rw-r--r--   0        0        0     1996 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/graphql/schemes/mutations.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/graphql/sentry/__init__.py
+-rw-r--r--   0        0        0      407 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/graphql/sentry/utils.py
+-rw-r--r--   0        0        0     1307 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/graphql/sentry/views.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/graphql/tests/__init__.py
+-rw-r--r--   0        0        0     2087 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/graphql/tests/base_test.py
+-rw-r--r--   0        0        0     1538 2023-11-27 08:56:40.000000 ambient_toolbox-9.6.4/ambient_toolbox/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2498 2023-11-27 08:56:35.477473 ambient_toolbox-9.6.4/ambient_toolbox/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/mail/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/mail/backends/__init__.py
+-rw-r--r--   0        0        0     3155 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/mail/backends/whitelist_smtp.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/management/commands/__init__.py
+-rw-r--r--   0        0        0     2050 2024-03-28 09:47:09.481466 ambient_toolbox-9.6.4/ambient_toolbox/management/commands/create_translation_file.py
+-rw-r--r--   0        0        0     1743 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/management/commands/install_permission_fixtures.py
+-rw-r--r--   0        0        0      294 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/management/commands/validate_test_structure.py
+-rw-r--r--   0        0        0     2478 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/managers.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/middleware/__init__.py
+-rw-r--r--   0        0        0      889 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/middleware/current_request.py
+-rw-r--r--   0        0        0      977 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/middleware/current_user.py
+-rw-r--r--   0        0        0        0 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/mixins/__init__.py
+-rw-r--r--   0        0        0     1886 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/mixins/bleacher.py
+-rw-r--r--   0        0        0     1340 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/mixins/models.py
+-rw-r--r--   0        0        0      238 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/mixins/validation.py
+-rw-r--r--   0        0        0     2971 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/models.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/permissions/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/permissions/fixtures/__init__.py
+-rw-r--r--   0        0        0      292 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/permissions/fixtures/declarations.py
+-rw-r--r--   0        0        0      232 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/permissions/fixtures/helpers.py
+-rw-r--r--   0        0        0     3235 2024-01-22 10:18:06.671277 ambient_toolbox-9.6.4/ambient_toolbox/permissions/fixtures/services.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/selectors/__init__.py
+-rw-r--r--   0        0        0      351 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/selectors/base.py
+-rw-r--r--   0        0        0     1027 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/selectors/permission.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.845804 ambient_toolbox-9.6.4/ambient_toolbox/sentry/__init__.py
+-rw-r--r--   0        0        0     2164 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/sentry/helpers.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.4/ambient_toolbox/services/__init__.py
+-rw-r--r--   0        0        0     3324 2024-02-02 15:54:55.522564 ambient_toolbox-9.6.4/ambient_toolbox/services/custom_scrubber.py
+-rw-r--r--   0        0        0        0 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/templatetags/__init__.py
+-rw-r--r--   0        0        0      229 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.4/ambient_toolbox/templatetags/ai_date_tags.py
+-rw-r--r--   0        0        0      647 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/templatetags/ai_email_tags.py
+-rw-r--r--   0        0        0      771 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/templatetags/ai_file_tags.py
+-rw-r--r--   0        0        0      185 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.4/ambient_toolbox/templatetags/ai_helper_tags.py
+-rw-r--r--   0        0        0     1165 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/templatetags/ai_number_tags.py
+-rw-r--r--   0        0        0      364 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/templatetags/ai_object_tags.py
+-rw-r--r--   0        0        0      620 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/templatetags/ai_string_tags.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.4/ambient_toolbox/tests/__init__.py
+-rw-r--r--   0        0        0       58 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.4/ambient_toolbox/tests/errors.py
+-rw-r--r--   0        0        0     5466 2024-02-02 15:54:07.436787 ambient_toolbox-9.6.4/ambient_toolbox/tests/mixins.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.4/ambient_toolbox/tests/structure_validator/__init__.py
+-rw-r--r--   0        0        0      386 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/tests/structure_validator/settings.py
+-rw-r--r--   0        0        0     4527 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/tests/structure_validator/test_structure_validator.py
+-rw-r--r--   0        0        0      219 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.4/ambient_toolbox/utils/__init__.py
+-rw-r--r--   0        0        0      119 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.4/ambient_toolbox/utils/cache.py
+-rw-r--r--   0        0        0     5971 2024-03-28 09:16:16.860241 ambient_toolbox-9.6.4/ambient_toolbox/utils/date.py
+-rw-r--r--   0        0        0     1383 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/utils/file.py
+-rw-r--r--   0        0        0      331 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/utils/log_whodid.py
+-rw-r--r--   0        0        0      557 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.4/ambient_toolbox/utils/math.py
+-rw-r--r--   0        0        0      904 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/utils/model.py
+-rw-r--r--   0        0        0     3822 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/utils/named_tuple.py
+-rw-r--r--   0        0        0     3826 2024-02-28 11:40:45.714060 ambient_toolbox-9.6.4/ambient_toolbox/utils/string.py
+-rw-r--r--   0        0        0        0 2023-11-24 13:16:44.820233 ambient_toolbox-9.6.4/ambient_toolbox/validators/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-24 13:16:44.820233 ambient_toolbox-9.6.4/ambient_toolbox/validators/auth_password/__init__.py
+-rw-r--r--   0        0        0      651 2023-11-24 13:16:44.820233 ambient_toolbox-9.6.4/ambient_toolbox/validators/auth_password/special_chars.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.861440 ambient_toolbox-9.6.4/ambient_toolbox/view_layer/__init__.py
+-rw-r--r--   0        0        0      728 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/view_layer/form_mixins.py
+-rw-r--r--   0        0        0      473 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/view_layer/formset_mixins.py
+-rw-r--r--   0        0        0     2910 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/view_layer/formset_view_mixin.py
+-rw-r--r--   0        0        0     1539 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/view_layer/htmx_mixins.py
+-rw-r--r--   0        0        0     2094 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/view_layer/mixins.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/ambient_toolbox/view_layer/tests/__init__.py
+-rw-r--r--   0        0        0     4031 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/view_layer/tests/mixins.py
+-rw-r--r--   0        0        0     1823 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/ambient_toolbox/view_layer/views.py
+-rw-r--r--   0        0        0      654 2024-03-28 09:27:28.908678 ambient_toolbox-9.6.4/docs/Makefile
+-rw-r--r--   0        0        0     2809 2024-03-28 09:27:28.906548 ambient_toolbox-9.6.4/docs/conf.py
+-rw-r--r--   0        0        0     5945 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/admin.md
+-rw-r--r--   0        0        0       33 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/changelog.rst
+-rw-r--r--   0        0        0     2225 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/context_manager.md
+-rw-r--r--   0        0        0      528 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/context_processors.md
+-rw-r--r--   0        0        0     7103 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/database_anonymisation.md
+-rw-r--r--   0        0        0     6612 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/djangorestframework.md
+-rw-r--r--   0        0        0     2489 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/docs/features/gitlab.md
+-rw-r--r--   0        0        0     6341 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/graphql.md
+-rw-r--r--   0        0        0      999 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/mail.md
+-rw-r--r--   0        0        0     5719 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/managers.md
+-rw-r--r--   0        0        0     5802 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/mixins.md
+-rw-r--r--   0        0        0     2394 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/models.md
+-rw-r--r--   0        0        0     6340 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/permissions.md
+-rw-r--r--   0        0        0     4327 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/selectors.md
+-rw-r--r--   0        0        0     3224 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/sentry.md
+-rw-r--r--   0        0        0     4858 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/services.md
+-rw-r--r--   0        0        0     1512 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/setup.md
+-rw-r--r--   0        0        0     5346 2024-01-12 08:49:19.726688 ambient_toolbox-9.6.4/docs/features/tests.md
+-rw-r--r--   0        0        0     1969 2024-03-04 08:25:42.940504 ambient_toolbox-9.6.4/docs/features/translations.md
+-rw-r--r--   0        0        0      223 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/utils.rst
+-rw-r--r--   0        0        0      508 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/utils/cache.md
+-rw-r--r--   0        0        0     7189 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/utils/date.md
+-rw-r--r--   0        0        0      710 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/utils/math.md
+-rw-r--r--   0        0        0     1061 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/utils/model.md
+-rw-r--r--   0        0        0     2298 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/utils/named_tuple.md
+-rw-r--r--   0        0        0     5640 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/utils/string.md
+-rw-r--r--   0        0        0      824 2023-11-27 08:55:29.443896 ambient_toolbox-9.6.4/docs/features/validators.md
+-rw-r--r--   0        0        0    15031 2023-10-22 11:06:15.867948 ambient_toolbox-9.6.4/docs/features/view-layer.md
+-rw-r--r--   0        0        0     1241 2024-02-29 15:04:25.128235 ambient_toolbox-9.6.4/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2024-03-28 09:27:28.907567 ambient_toolbox-9.6.4/docs/make.bat
+-rw-r--r--   0        0        0      655 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/manage.py
+-rw-r--r--   0        0        0     5905 2024-03-28 09:47:09.481466 ambient_toolbox-9.6.4/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-03-28 09:27:28.893393 ambient_toolbox-9.6.4/pytest.ini
+-rw-r--r--   0        0        0      151 2024-03-28 09:27:28.909773 ambient_toolbox-9.6.4/scripts/unix/install_requirements.sh
+-rw-r--r--   0        0        0       50 2024-03-28 09:27:28.910889 ambient_toolbox-9.6.4/scripts/unix/publish_to_pypi.sh
+-rw-r--r--   0        0        0      151 2024-03-28 09:27:28.913049 ambient_toolbox-9.6.4/scripts/windows/install_requirements.ps1
+-rw-r--r--   0        0        0       50 2024-03-28 09:27:28.914215 ambient_toolbox-9.6.4/scripts/windows/publish_to_pypi.ps1
+-rw-r--r--   0        0        0     1896 2024-02-29 15:04:25.129284 ambient_toolbox-9.6.4/settings.py
+-rw-r--r--   0        0        0      281 2024-03-28 09:27:28.901366 ambient_toolbox-9.6.4/setup.cfg
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/api/__init__.py
+-rw-r--r--   0        0        0      275 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/testapp/api/serializers.py
+-rw-r--r--   0        0        0      251 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/testapp/api/urls.py
+-rw-r--r--   0        0        0      510 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/api/views.py
+-rw-r--r--   0        0        0      210 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/testapp/forms.py
+-rw-r--r--   0        0        0       92 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/managers.py
+-rw-r--r--   0        0        0     6057 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/testapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/migrations/__init__.py
+-rw-r--r--   0        0        0     3292 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/testapp/models.py
+-rw-r--r--   0        0        0      406 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/testapp/permissions.py
+-rw-r--r--   0        0        0      157 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/selectors.py
+-rw-r--r--   0        0        0     1390 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/templates/403.html
+-rw-r--r--   0        0        0      134 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/templates/testapp/test_template.html
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/tests/missing_init/test_ok.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/tests/subdirectory/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/tests/subdirectory/missing_test_prefix.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/tests/subdirectory/test_ok.py
+-rw-r--r--   0        0        0      554 2023-11-21 10:36:16.893614 ambient_toolbox-9.6.4/testapp/urls.py
+-rw-r--r--   0        0        0      491 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/testapp/views.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/__init__.py
+-rw-r--r--   0        0        0     2778 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
+-rw-r--r--   0        0        0     1848 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
+-rw-r--r--   0        0        0     1639 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
+-rw-r--r--   0        0        0     1150 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
+-rw-r--r--   0        0        0     4773 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_classes.py
+-rw-r--r--   0        0        0     3792 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
+-rw-r--r--   0        0        0     1446 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
+-rw-r--r--   0        0        0     1854 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/ambient_toolbox/__init__.py
+-rw-r--r--   0        0        0     7631 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/ambient_toolbox/test_test_structure_validator.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/drf/__init__.py
+-rw-r--r--   0        0        0     3052 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/drf/test_fields.py
+-rw-r--r--   0        0        0        0 2024-02-28 11:40:45.715077 ambient_toolbox-9.6.4/tests/gitlab/__init__.py
+-rw-r--r--   0        0        0     1486 2024-02-28 11:40:45.715077 ambient_toolbox-9.6.4/tests/gitlab/test_coverage.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      459 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/mixins/test_validation.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/permissions/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/permissions/fixtures/__init__.py
+-rw-r--r--   0        0        0     1064 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/permissions/fixtures/test_declarations.py
+-rw-r--r--   0        0        0      564 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/permissions/fixtures/test_helpers.py
+-rw-r--r--   0        0        0     7053 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/permissions/fixtures/test_services_setup_service.py
+-rw-r--r--   0        0        0     1466 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/permissions/test_install_permission_fixtures_command.py
+-rw-r--r--   0        0        0      485 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/query_selectors/test_base.py
+-rw-r--r--   0        0        0     1581 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/query_selectors/test_permission.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/selectors/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/sentry/__init__.py
+-rw-r--r--   0        0        0     6048 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/sentry/mock_data.py
+-rw-r--r--   0        0        0     1548 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/sentry/test_sentry_helper.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/templatetags/__init__.py
+-rw-r--r--   0        0        0     1101 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/templatetags/test_ai_number_tags.py
+-rw-r--r--   0        0        0      620 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/test_admin_forms.py
+-rw-r--r--   0        0        0     1574 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/test_admin_inlines.py
+-rw-r--r--   0        0        0     2829 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/test_admin_view_mixins.py
+-rw-r--r--   0        0        0     2150 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/test_context_manager.py
+-rw-r--r--   0        0        0      796 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/test_log_whodid.py
+-rw-r--r--   0        0        0     3179 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/test_managers.py
+-rw-r--r--   0        0        0     1581 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/test_math.py
+-rw-r--r--   0        0        0     4121 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/test_middleware.py
+-rw-r--r--   0        0        0     1163 2023-10-22 11:06:15.877454 ambient_toolbox-9.6.4/tests/test_mixins_models.py
+-rw-r--r--   0        0        0     2840 2023-12-05 10:03:55.292807 ambient_toolbox-9.6.4/tests/test_models.py
+-rw-r--r--   0        0        0     1730 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/test_rest_api_mixins.py
+-rw-r--r--   0        0        0     1157 2024-02-02 15:54:55.523069 ambient_toolbox-9.6.4/tests/test_scrubbing_service.py
+-rw-r--r--   0        0        0      280 2023-10-22 11:06:15.893086 ambient_toolbox-9.6.4/tests/test_utils_cache.py
+-rw-r--r--   0        0        0    12473 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/test_utils_date.py
+-rw-r--r--   0        0        0     1839 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/test_utils_file.py
+-rw-r--r--   0        0        0     1275 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/test_utils_model.py
+-rw-r--r--   0        0        0     4112 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/test_utils_named_tuple.py
+-rw-r--r--   0        0        0     5492 2024-03-28 09:16:16.861299 ambient_toolbox-9.6.4/tests/test_utils_string.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.893086 ambient_toolbox-9.6.4/tests/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.893086 ambient_toolbox-9.6.4/tests/tests/mixins/__init__.py
+-rw-r--r--   0        0        0     1250 2024-02-02 16:00:03.078374 ambient_toolbox-9.6.4/tests/tests/mixins/test_django_message_framework.py
+-rw-r--r--   0        0        0     1955 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/tests/mixins/test_mixins.py
+-rw-r--r--   0        0        0      229 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/tests/mixins/test_models.py
+-rw-r--r--   0        0        0     2418 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/tests/mixins/test_request_provider_mixin.py
+-rw-r--r--   0        0        0     2711 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/tests/test_mail_backends.py
+-rw-r--r--   0        0        0        0 2023-11-24 13:16:44.820233 ambient_toolbox-9.6.4/tests/validators/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-24 13:16:44.820233 ambient_toolbox-9.6.4/tests/validators/auth_password/__init__.py
+-rw-r--r--   0        0        0     1443 2023-11-24 13:16:44.820233 ambient_toolbox-9.6.4/tests/validators/auth_password/test_special_chars.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:15.893086 ambient_toolbox-9.6.4/tests/view_layer/__init__.py
+-rw-r--r--   0        0        0     1834 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/view_layer/test_formset_mixins.py
+-rw-r--r--   0        0        0     1518 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/view_layer/test_htmx_response_mixin.py
+-rw-r--r--   0        0        0     4426 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/view_layer/test_meta_mixins.py
+-rw-r--r--   0        0        0     1325 2023-11-21 10:36:16.909224 ambient_toolbox-9.6.4/tests/view_layer/test_views.py
+-rw-r--r--   0        0        0     9035 1970-01-01 00:00:00.000000 ambient_toolbox-9.6.4/PKG-INFO
```

### Comparing `ambient_toolbox-9.6.3/.ambient-package-update/metadata.py` & `ambient_toolbox-9.6.4/.ambient-package-update/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     company="Ambient Innovation: GmbH",
     authors=[
         PackageAuthor(
             name="Ambient Digital",
             email="hello@ambient.digital",
         ),
     ],
-    min_coverage=96.52,
+    min_coverage=86.51,
     development_status="5 - Production/Stable",
     license=LICENSE_MIT,
     license_year=2012,
     readme_content=ReadmeContent(
         tagline="Python toolbox of Ambient Digital containing an abundance of useful tools and gadgets.",
         content="""## Features
 
@@ -51,14 +51,16 @@
 [django-pony-express](https://pypi.org/project/django-pony-express/).
 """,
     ),
     dependencies=[
         "Django>=3.2.20",
         "bleach>=1.4,<6",
         "python-dateutil>=2.5.3",
+        # We keep this until we drop Python 3.8
+        "pytz",
     ],
     supported_django_versions=SUPPORTED_DJANGO_VERSIONS,
     supported_python_versions=SUPPORTED_PYTHON_VERSIONS,
     has_migrations=True,
     optional_dependencies={
         "dev": [
             *DEV_DEPENDENCIES,
```

### Comparing `ambient_toolbox-9.6.3/.github/workflows/ci.yml` & `ambient_toolbox-9.6.4/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 jobs:
   linting:
     runs-on: ubuntu-22.04
     steps:
       - uses: actions/checkout@v4
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.12"
 
       - name: Install required packages
         run: pip install pre-commit
 
       - name: Run pre-commit hooks
@@ -23,15 +23,15 @@
 
   validate_migrations:
     name: Validate migrations
     runs-on: ubuntu-22.04
     steps:
       - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: '3.12'
 
       - name: Install dependencies
         run: python -m pip install -U pip-tools && pip-compile --extra dev,drf,graphql,sentry,view-layer, -o requirements.txt pyproject.toml --resolver=backtracking && pip-sync
 
       - name: Validate migration integrity
@@ -56,15 +56,15 @@
             django-version: 50
           - python-version: '3.9'
             django-version: 50
 
     steps:
       - uses: actions/checkout@v4
       - name: setup python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install tox
         run: pip install tox
       - name: Run Tests
         env:
           TOXENV: django${{ matrix.django-version }}
@@ -78,23 +78,23 @@
   coverage:
     name: Coverage
     runs-on: ubuntu-22.04
     needs: tests
     steps:
       - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: '3.12'
 
       - name: Install dependencies
         run: python -m pip install --upgrade coverage[toml]
 
       - name: Download data
         uses: actions/download-artifact@v3
         with:
           name: coverage-data
 
-      - name: Combine coverage and fail if it's too low
+      - name: Combine coverage and fail if it's <100%
         run: |
-          python -m coverage html --skip-covered
+          python -m coverage html --skip-covered --skip-empty
           python -m coverage report --fail-under=86.51
```

### Comparing `ambient_toolbox-9.6.3/.gitignore` & `ambient_toolbox-9.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/.pre-commit-config.yaml` & `ambient_toolbox-9.6.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/.readthedocs.yaml` & `ambient_toolbox-9.6.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/CHANGES.md` & `ambient_toolbox-9.6.4/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+**9.6.4** (2024-03-28)
+  * Added convenience feature for `create_translation_file` so the user can omit the `--lang` param if there is only
+one language
+  * Added `pytz` as a dependency until we can drop it when removing Python 3.8 compat
+
 **9.6.3** (2024-03-04)
   * Fixed a bug in the documentation
 
 **9.6.2** (2024-03-04)
   * Fixed a bug in the documentation
 
 **9.6.1** (2024-03-04)
```

### Comparing `ambient_toolbox-9.6.3/Dockerfile` & `ambient_toolbox-9.6.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/LICENSE.md` & `ambient_toolbox-9.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/README.md` & `ambient_toolbox-9.6.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![PyPI release](https://img.shields.io/pypi/v/ambient-toolbox.svg)](https://pypi.org/project/ambient-toolbox/)
 [![Downloads](https://static.pepy.tech/badge/ambient-toolbox)](https://pepy.tech/project/ambient-toolbox)
-[![Coverage](https://img.shields.io/badge/Coverage-96.52%25-success)](https://github.com/ambient-innovation/ambient-toolbox/actions?workflow=CI)
+[![Coverage](https://img.shields.io/badge/Coverage-86.51%25-success)](https://github.com/ambient-innovation/ambient-toolbox/actions?workflow=CI)
 [![Linting](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Coding Style](https://img.shields.io/badge/code%20style-Ruff-000000.svg)](https://github.com/astral-sh/ruff)
 [![Documentation Status](https://readthedocs.org/projects/ambient-toolbox/badge/?version=latest)](https://ambient-toolbox.readthedocs.io/en/latest/?badge=latest)
 
 Python toolbox of Ambient Digital containing an abundance of useful tools and gadgets.
 
 * [PyPI](https://pypi.org/project/ambient-toolbox/)
```

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/admin/model_admins/classes.py` & `ambient_toolbox-9.6.4/ambient_toolbox/admin/model_admins/classes.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/admin/model_admins/inlines.py` & `ambient_toolbox-9.6.4/ambient_toolbox/admin/model_admins/inlines.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/admin/model_admins/mixins.py` & `ambient_toolbox-9.6.4/ambient_toolbox/admin/model_admins/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/admin/views/forms.py` & `ambient_toolbox-9.6.4/ambient_toolbox/admin/views/forms.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/admin/views/mixins.py` & `ambient_toolbox-9.6.4/ambient_toolbox/admin/views/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/context_manager.py` & `ambient_toolbox-9.6.4/ambient_toolbox/context_manager.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/drf/fields.py` & `ambient_toolbox-9.6.4/ambient_toolbox/drf/fields.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/drf/serializers.py` & `ambient_toolbox-9.6.4/ambient_toolbox/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/drf/tests.py` & `ambient_toolbox-9.6.4/ambient_toolbox/drf/tests.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/gitlab/coverage.py` & `ambient_toolbox-9.6.4/ambient_toolbox/gitlab/coverage.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/graphql/forms/mutations.py` & `ambient_toolbox-9.6.4/ambient_toolbox/graphql/forms/mutations.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/graphql/schemes/mutations.py` & `ambient_toolbox-9.6.4/ambient_toolbox/graphql/schemes/mutations.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/graphql/sentry/views.py` & `ambient_toolbox-9.6.4/ambient_toolbox/graphql/sentry/views.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/graphql/tests/base_test.py` & `ambient_toolbox-9.6.4/ambient_toolbox/graphql/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/locale/de/LC_MESSAGES/django.mo` & `ambient_toolbox-9.6.4/ambient_toolbox/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/locale/de/LC_MESSAGES/django.po` & `ambient_toolbox-9.6.4/ambient_toolbox/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/mail/backends/whitelist_smtp.py` & `ambient_toolbox-9.6.4/ambient_toolbox/mail/backends/whitelist_smtp.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/management/commands/install_permission_fixtures.py` & `ambient_toolbox-9.6.4/ambient_toolbox/management/commands/install_permission_fixtures.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/managers.py` & `ambient_toolbox-9.6.4/ambient_toolbox/managers.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/middleware/current_request.py` & `ambient_toolbox-9.6.4/ambient_toolbox/middleware/current_request.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/middleware/current_user.py` & `ambient_toolbox-9.6.4/ambient_toolbox/middleware/current_user.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/mixins/bleacher.py` & `ambient_toolbox-9.6.4/ambient_toolbox/mixins/bleacher.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/mixins/models.py` & `ambient_toolbox-9.6.4/ambient_toolbox/mixins/models.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/models.py` & `ambient_toolbox-9.6.4/ambient_toolbox/models.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/permissions/fixtures/services.py` & `ambient_toolbox-9.6.4/ambient_toolbox/permissions/fixtures/services.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/selectors/permission.py` & `ambient_toolbox-9.6.4/ambient_toolbox/selectors/permission.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/sentry/helpers.py` & `ambient_toolbox-9.6.4/ambient_toolbox/sentry/helpers.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/services/custom_scrubber.py` & `ambient_toolbox-9.6.4/ambient_toolbox/services/custom_scrubber.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/templatetags/ai_email_tags.py` & `ambient_toolbox-9.6.4/ambient_toolbox/templatetags/ai_email_tags.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/templatetags/ai_file_tags.py` & `ambient_toolbox-9.6.4/ambient_toolbox/templatetags/ai_file_tags.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/templatetags/ai_number_tags.py` & `ambient_toolbox-9.6.4/ambient_toolbox/templatetags/ai_number_tags.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/templatetags/ai_string_tags.py` & `ambient_toolbox-9.6.4/ambient_toolbox/templatetags/ai_string_tags.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/tests/mixins.py` & `ambient_toolbox-9.6.4/ambient_toolbox/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/tests/structure_validator/test_structure_validator.py` & `ambient_toolbox-9.6.4/ambient_toolbox/tests/structure_validator/test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/utils/date.py` & `ambient_toolbox-9.6.4/ambient_toolbox/utils/date.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-import datetime
-from calendar import monthrange
-from typing import Tuple, Union
-
-import pytz
-from dateutil.relativedelta import relativedelta
-from django.conf import settings
-from django.utils import timezone
-from django.utils.translation import gettext_lazy as _
-from pytz import UnknownTimeZoneError
-
-
-class DateHelper:
-    """
-    Constants to use for django ORMs `__weekday` lookup to avoid usage of integers directly.
-    Unfortunately python's calendar weekdays are not equivalent to the database ones.
-    """
-
-    ORM_SUNDAY = 1
-    ORM_MONDAY = 2
-    ORM_TUESDAY = 3
-    ORM_WEDNESDAY = 4
-    ORM_THURSDAY = 5
-    ORM_FRIDAY = 6
-    ORM_SATURDAY = 7
-
-
-def tz_today(str_format=None):
-    """
-    Returns either a timezone-aware today object or string. Depending on if the `str_format` param is set.
-    :param str_format: If set, formats the date object to a string. Pass strftime-compatible value
-    :return:
-    """
-    if settings.USE_TZ:
-        date = timezone.now().date()
-    else:
-        date = datetime.datetime.now().date()
-
-    if str_format:
-        return date.strftime(str_format)
-    return date
-
-
-def add_months(
-    source_date: Union[datetime.date, datetime.datetime], months: Union[int, float]
-) -> Union[datetime.date, datetime.datetime]:
-    return source_date + relativedelta(months=months)
-
-
-def add_days(
-    source_date: Union[datetime.date, datetime.datetime], days: int
-) -> Union[datetime.date, datetime.datetime]:
-    return source_date + datetime.timedelta(days=days)
-
-
-def add_minutes(source_datetime: datetime.datetime, minutes: int) -> Union[datetime.date, datetime.datetime]:
-    return source_datetime + relativedelta(minutes=minutes)
-
-
-def get_next_month() -> datetime.date:
-    return add_months(tz_today(), 1)
-
-
-def first_day_of_month(source_date: datetime.date) -> datetime.date:
-    return datetime.date(source_date.year, source_date.month, 1)
-
-
-def get_formatted_date_str(source_date: Union[datetime.date, datetime.datetime]) -> str:
-    return source_date.strftime("%d.%m.%Y")
-
-
-def get_time_from_seconds(seconds: int) -> str:
-    if seconds < 0:
-        raise ValueError(_("Seconds must be positive."))
-    hours = seconds // 3600
-    minutes = (seconds - (hours * 3600)) // 60
-    seconds = seconds - ((hours * 3600) + (minutes * 60))
-    return "%02d:%02d:%02d" % (hours, minutes, seconds)
-
-
-def datetime_format(target_datetime: datetime.datetime, dt_format: str) -> str:
-    """
-    Uses strftime, but considers timezone (only for datetime objects)
-    """
-    try:
-        dt_format = target_datetime.astimezone(tz=pytz.timezone(settings.TIME_ZONE)).strftime(dt_format)
-    except UnknownTimeZoneError:
-        dt_format = target_datetime.strftime(dt_format)
-    return dt_format
-
-
-def get_start_and_end_date_from_calendar_week(year: int, calendar_week: int) -> (datetime.date, datetime.date):
-    """
-    Returns the first and last day of a given calendar week
-    """
-    monday = datetime.datetime.strptime(f"{year}-{calendar_week}-1", "%Y-%W-%w").astimezone().date()
-    return monday, monday + datetime.timedelta(days=6.9)
-
-
-def get_next_calendar_week(compare_date: datetime.date) -> int:
-    """
-    Returns the next calendar week as an integer
-    """
-    day_in_one_week = compare_date + datetime.timedelta(days=(7 - compare_date.weekday()))
-    return day_in_one_week.isocalendar()[1]
-
-
-def next_weekday(given_date: datetime.date, weekday: int) -> datetime.date:
-    """
-    Returns the next date of the given weekday
-    For example: next_weekday(d, calendar.MONDAY) would return the next monday starting at date "given_date"
-    """
-    days_ahead = weekday - given_date.weekday()
-    if days_ahead <= 0:
-        days_ahead += 7
-    return given_date + datetime.timedelta(days_ahead)
-
-
-def date_month_delta(start_date: datetime.date, end_date: datetime.date) -> float:
-    """
-    Calculates the number of months lying between two dates.
-    So from April 15th to May 1st it's 0.5 months.
-    Attention: `end_date` will be excluded in the result (outer border)
-    """
-    # If `start_date` is greater, this logic doesn't make any sense
-    if start_date > end_date:
-        raise NotImplementedError("Start date > end date")
-
-    # Calculate date difference between dates
-    date_diff = (end_date - start_date).days
-
-    # Iteration variable
-    delta = 0
-    iter_date = start_date
-    # Loop until all days are processed
-    while date_diff > 0:
-        # Get days of month we are currently looking at
-        iter_month, iter_month_days = monthrange(iter_date.year, iter_date.month)
-        # Calculate how many days are left to end of this month
-        days_to_month_end = min((iter_month_days - (iter_date.day - 1)), date_diff)
-        # Add percentage of the month these days cover to return variable
-        delta += days_to_month_end / iter_month_days
-        # Reduce leftover days by the amount we already processed
-        date_diff -= days_to_month_end
-
-        # Set iteration date to first of next month
-        iter_date += relativedelta(months=1, day=1)
-
-    # Return data
-    return delta
-
-
-def get_first_and_last_of_month(date_object: datetime.date = None) -> Tuple[datetime.date, datetime.date]:
-    """
-    Returns first and last day of a month as date objects.
-    Will either return first/last of current month (if no datetime_object is passed), or will determine first/last of
-    the month of the passed datetime.date object
-    """
-    first_of_month = timezone.now().replace(day=1).date() if not date_object else date_object.replace(day=1)
-
-    # Add one month to first_of_month
-    first_of_next_month = first_of_month + relativedelta(months=1)
-
-    # Subtract one day, to get the last of month
-    last_of_month = first_of_next_month - datetime.timedelta(days=1)
-
-    return first_of_month, last_of_month
+import datetime
+from calendar import monthrange
+from typing import Tuple, Union
+
+import pytz
+from dateutil.relativedelta import relativedelta
+from django.conf import settings
+from django.utils import timezone
+from django.utils.translation import gettext_lazy as _
+from pytz import UnknownTimeZoneError
+
+
+class DateHelper:
+    """
+    Constants to use for django ORMs `__weekday` lookup to avoid usage of integers directly.
+    Unfortunately python's calendar weekdays are not equivalent to the database ones.
+    """
+
+    ORM_SUNDAY = 1
+    ORM_MONDAY = 2
+    ORM_TUESDAY = 3
+    ORM_WEDNESDAY = 4
+    ORM_THURSDAY = 5
+    ORM_FRIDAY = 6
+    ORM_SATURDAY = 7
+
+
+def tz_today(str_format=None):
+    """
+    Returns either a timezone-aware today object or string. Depending on if the `str_format` param is set.
+    :param str_format: If set, formats the date object to a string. Pass strftime-compatible value
+    :return:
+    """
+    if settings.USE_TZ:
+        date = timezone.now().date()
+    else:
+        date = datetime.datetime.now().date()
+
+    if str_format:
+        return date.strftime(str_format)
+    return date
+
+
+def add_months(
+    source_date: Union[datetime.date, datetime.datetime], months: Union[int, float]
+) -> Union[datetime.date, datetime.datetime]:
+    return source_date + relativedelta(months=months)
+
+
+def add_days(
+    source_date: Union[datetime.date, datetime.datetime], days: int
+) -> Union[datetime.date, datetime.datetime]:
+    return source_date + datetime.timedelta(days=days)
+
+
+def add_minutes(source_datetime: datetime.datetime, minutes: int) -> Union[datetime.date, datetime.datetime]:
+    return source_datetime + relativedelta(minutes=minutes)
+
+
+def get_next_month() -> datetime.date:
+    return add_months(tz_today(), 1)
+
+
+def first_day_of_month(source_date: datetime.date) -> datetime.date:
+    return datetime.date(source_date.year, source_date.month, 1)
+
+
+def get_formatted_date_str(source_date: Union[datetime.date, datetime.datetime]) -> str:
+    return source_date.strftime("%d.%m.%Y")
+
+
+def get_time_from_seconds(seconds: int) -> str:
+    if seconds < 0:
+        raise ValueError(_("Seconds must be positive."))
+    hours = seconds // 3600
+    minutes = (seconds - (hours * 3600)) // 60
+    seconds = seconds - ((hours * 3600) + (minutes * 60))
+    return "%02d:%02d:%02d" % (hours, minutes, seconds)
+
+
+def datetime_format(target_datetime: datetime.datetime, dt_format: str) -> str:
+    """
+    Uses strftime, but considers timezone (only for datetime objects)
+    """
+    try:
+        dt_format = target_datetime.astimezone(tz=pytz.timezone(settings.TIME_ZONE)).strftime(dt_format)
+    except UnknownTimeZoneError:
+        dt_format = target_datetime.strftime(dt_format)
+    return dt_format
+
+
+def get_start_and_end_date_from_calendar_week(year: int, calendar_week: int) -> (datetime.date, datetime.date):
+    """
+    Returns the first and last day of a given calendar week
+    """
+    monday = datetime.datetime.strptime(f"{year}-{calendar_week}-1", "%Y-%W-%w").astimezone().date()
+    return monday, monday + datetime.timedelta(days=6.9)
+
+
+def get_next_calendar_week(compare_date: datetime.date) -> int:
+    """
+    Returns the next calendar week as an integer
+    """
+    day_in_one_week = compare_date + datetime.timedelta(days=(7 - compare_date.weekday()))
+    return day_in_one_week.isocalendar()[1]
+
+
+def next_weekday(given_date: datetime.date, weekday: int) -> datetime.date:
+    """
+    Returns the next date of the given weekday
+    For example: next_weekday(d, calendar.MONDAY) would return the next monday starting at date "given_date"
+    """
+    days_ahead = weekday - given_date.weekday()
+    if days_ahead <= 0:
+        days_ahead += 7
+    return given_date + datetime.timedelta(days_ahead)
+
+
+def date_month_delta(start_date: datetime.date, end_date: datetime.date) -> float:
+    """
+    Calculates the number of months lying between two dates.
+    So from April 15th to May 1st it's 0.5 months.
+    Attention: `end_date` will be excluded in the result (outer border)
+    """
+    # If `start_date` is greater, this logic doesn't make any sense
+    if start_date > end_date:
+        raise NotImplementedError("Start date > end date")
+
+    # Calculate date difference between dates
+    date_diff = (end_date - start_date).days
+
+    # Iteration variable
+    delta = 0
+    iter_date = start_date
+    # Loop until all days are processed
+    while date_diff > 0:
+        # Get days of month we are currently looking at
+        iter_month, iter_month_days = monthrange(iter_date.year, iter_date.month)
+        # Calculate how many days are left to end of this month
+        days_to_month_end = min((iter_month_days - (iter_date.day - 1)), date_diff)
+        # Add percentage of the month these days cover to return variable
+        delta += days_to_month_end / iter_month_days
+        # Reduce leftover days by the amount we already processed
+        date_diff -= days_to_month_end
+
+        # Set iteration date to first of next month
+        iter_date += relativedelta(months=1, day=1)
+
+    # Return data
+    return delta
+
+
+def get_first_and_last_of_month(date_object: datetime.date = None) -> Tuple[datetime.date, datetime.date]:
+    """
+    Returns first and last day of a month as date objects.
+    Will either return first/last of current month (if no datetime_object is passed), or will determine first/last of
+    the month of the passed datetime.date object
+    """
+    first_of_month = timezone.now().replace(day=1).date() if not date_object else date_object.replace(day=1)
+
+    # Add one month to first_of_month
+    first_of_next_month = first_of_month + relativedelta(months=1)
+
+    # Subtract one day, to get the last of month
+    last_of_month = first_of_next_month - datetime.timedelta(days=1)
+
+    return first_of_month, last_of_month
```

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/utils/file.py` & `ambient_toolbox-9.6.4/ambient_toolbox/utils/file.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/utils/math.py` & `ambient_toolbox-9.6.4/ambient_toolbox/utils/math.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/utils/model.py` & `ambient_toolbox-9.6.4/ambient_toolbox/utils/model.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/utils/named_tuple.py` & `ambient_toolbox-9.6.4/ambient_toolbox/utils/named_tuple.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/utils/string.py` & `ambient_toolbox-9.6.4/ambient_toolbox/utils/string.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/validators/auth_password/special_chars.py` & `ambient_toolbox-9.6.4/ambient_toolbox/validators/auth_password/special_chars.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/view_layer/form_mixins.py` & `ambient_toolbox-9.6.4/ambient_toolbox/view_layer/form_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/view_layer/formset_view_mixin.py` & `ambient_toolbox-9.6.4/ambient_toolbox/view_layer/formset_view_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/view_layer/htmx_mixins.py` & `ambient_toolbox-9.6.4/ambient_toolbox/view_layer/htmx_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/view_layer/mixins.py` & `ambient_toolbox-9.6.4/ambient_toolbox/view_layer/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/view_layer/tests/mixins.py` & `ambient_toolbox-9.6.4/ambient_toolbox/view_layer/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/ambient_toolbox/view_layer/views.py` & `ambient_toolbox-9.6.4/ambient_toolbox/view_layer/views.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/Makefile` & `ambient_toolbox-9.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/conf.py` & `ambient_toolbox-9.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/admin.md` & `ambient_toolbox-9.6.4/docs/features/admin.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/context_manager.md` & `ambient_toolbox-9.6.4/docs/features/context_manager.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/context_processors.md` & `ambient_toolbox-9.6.4/docs/features/context_processors.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/database_anonymisation.md` & `ambient_toolbox-9.6.4/docs/features/database_anonymisation.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/djangorestframework.md` & `ambient_toolbox-9.6.4/docs/features/djangorestframework.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/gitlab.md` & `ambient_toolbox-9.6.4/docs/features/gitlab.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/graphql.md` & `ambient_toolbox-9.6.4/docs/features/graphql.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/mail.md` & `ambient_toolbox-9.6.4/docs/features/mail.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/managers.md` & `ambient_toolbox-9.6.4/docs/features/managers.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/mixins.md` & `ambient_toolbox-9.6.4/docs/features/mixins.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/models.md` & `ambient_toolbox-9.6.4/docs/features/models.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/permissions.md` & `ambient_toolbox-9.6.4/docs/features/permissions.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/selectors.md` & `ambient_toolbox-9.6.4/docs/features/selectors.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/sentry.md` & `ambient_toolbox-9.6.4/docs/features/sentry.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/services.md` & `ambient_toolbox-9.6.4/docs/features/services.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/setup.md` & `ambient_toolbox-9.6.4/docs/features/setup.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/tests.md` & `ambient_toolbox-9.6.4/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/translations.md` & `ambient_toolbox-9.6.4/docs/features/translations.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/utils/date.md` & `ambient_toolbox-9.6.4/docs/features/utils/date.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/utils/math.md` & `ambient_toolbox-9.6.4/docs/features/utils/math.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/utils/model.md` & `ambient_toolbox-9.6.4/docs/features/utils/model.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/utils/named_tuple.md` & `ambient_toolbox-9.6.4/docs/features/utils/named_tuple.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/utils/string.md` & `ambient_toolbox-9.6.4/docs/features/utils/string.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/validators.md` & `ambient_toolbox-9.6.4/docs/features/validators.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/features/view-layer.md` & `ambient_toolbox-9.6.4/docs/features/view-layer.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/index.rst` & `ambient_toolbox-9.6.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/docs/make.bat` & `ambient_toolbox-9.6.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/manage.py` & `ambient_toolbox-9.6.4/manage.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/pyproject.toml` & `ambient_toolbox-9.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 ]
 dynamic = ["version", "description"]
 license = {"file" = "LICENSE.md"}
 dependencies = [
     'Django>=3.2.20',
     'bleach>=1.4,<6',
     'python-dateutil>=2.5.3',
+    'pytz',
 ]
 
 
 [project.optional-dependencies]
 dev = [
    'typer~=0.9',
    'freezegun~=1.3',
```

### Comparing `ambient_toolbox-9.6.3/settings.py` & `ambient_toolbox-9.6.4/settings.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/testapp/migrations/0001_initial.py` & `ambient_toolbox-9.6.4/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/testapp/models.py` & `ambient_toolbox-9.6.4/testapp/models.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/testapp/templates/403.html` & `ambient_toolbox-9.6.4/testapp/templates/403.html`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/testapp/urls.py` & `ambient_toolbox-9.6.4/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py` & `ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py` & `ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py` & `ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py` & `ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_classes.py` & `ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_classes.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py` & `ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_fetch_object_mixin.py` & `ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_fetch_object_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py` & `ambient_toolbox-9.6.4/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/ambient_toolbox/test_test_structure_validator.py` & `ambient_toolbox-9.6.4/tests/ambient_toolbox/test_test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/drf/test_fields.py` & `ambient_toolbox-9.6.4/tests/drf/test_fields.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/gitlab/test_coverage.py` & `ambient_toolbox-9.6.4/tests/gitlab/test_coverage.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/permissions/fixtures/test_declarations.py` & `ambient_toolbox-9.6.4/tests/permissions/fixtures/test_declarations.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/permissions/fixtures/test_helpers.py` & `ambient_toolbox-9.6.4/tests/permissions/fixtures/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/permissions/fixtures/test_services_setup_service.py` & `ambient_toolbox-9.6.4/tests/permissions/fixtures/test_services_setup_service.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/permissions/test_install_permission_fixtures_command.py` & `ambient_toolbox-9.6.4/tests/permissions/test_install_permission_fixtures_command.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/query_selectors/test_permission.py` & `ambient_toolbox-9.6.4/tests/query_selectors/test_permission.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/sentry/mock_data.py` & `ambient_toolbox-9.6.4/tests/sentry/mock_data.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/sentry/test_sentry_helper.py` & `ambient_toolbox-9.6.4/tests/sentry/test_sentry_helper.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/templatetags/test_ai_number_tags.py` & `ambient_toolbox-9.6.4/tests/templatetags/test_ai_number_tags.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_admin_forms.py` & `ambient_toolbox-9.6.4/tests/test_admin_forms.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_admin_inlines.py` & `ambient_toolbox-9.6.4/tests/test_admin_inlines.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_admin_view_mixins.py` & `ambient_toolbox-9.6.4/tests/test_admin_view_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_context_manager.py` & `ambient_toolbox-9.6.4/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_log_whodid.py` & `ambient_toolbox-9.6.4/tests/test_log_whodid.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_managers.py` & `ambient_toolbox-9.6.4/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_math.py` & `ambient_toolbox-9.6.4/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_middleware.py` & `ambient_toolbox-9.6.4/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_mixins_models.py` & `ambient_toolbox-9.6.4/tests/test_mixins_models.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_models.py` & `ambient_toolbox-9.6.4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_rest_api_mixins.py` & `ambient_toolbox-9.6.4/tests/test_rest_api_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_scrubbing_service.py` & `ambient_toolbox-9.6.4/tests/test_scrubbing_service.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_utils_date.py` & `ambient_toolbox-9.6.4/tests/test_utils_date.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_utils_file.py` & `ambient_toolbox-9.6.4/tests/test_utils_file.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_utils_model.py` & `ambient_toolbox-9.6.4/tests/test_utils_model.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_utils_named_tuple.py` & `ambient_toolbox-9.6.4/tests/test_utils_named_tuple.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/test_utils_string.py` & `ambient_toolbox-9.6.4/tests/test_utils_string.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-import datetime
-
-import pytz
-from django.test import TestCase
-
-from ambient_toolbox.utils.string import (
-    date_to_string,
-    datetime_to_string,
-    distinct,
-    encode_to_xml,
-    float_to_string,
-    number_to_string,
-    slugify_file_name,
-    smart_truncate,
-    string_or_none_to_string,
-)
-
-
-class UtilsStringTest(TestCase):
-    def test_distinct_regular(self):
-        not_distinct_list = ["Beer", "Wine", "Whiskey", "Beer"]
-        distinct_list = distinct(not_distinct_list)
-
-        self.assertEqual(len(distinct_list), 3)
-        self.assertIn("Beer", distinct_list)
-        self.assertIn("Whiskey", distinct_list)
-        self.assertIn("Wine", distinct_list)
-
-    def test_slugify_file_name_regular(self):
-        filename = "hola and hello.txt"
-        slug = slugify_file_name(filename)
-        self.assertEqual(slug, "hola_and_hello.txt")
-
-    def test_slugify_file_name_nothing_to_slugify(self):
-        filename = "hola.txt"
-        slug = slugify_file_name(filename)
-        self.assertEqual(slug, filename)
-
-    def test_slugify_file_name_max_length(self):
-        filename = "a very long filename.txt"
-        slug = slugify_file_name(filename, 6)
-        self.assertEqual(slug, "a_very.txt")
-
-    def test_smart_truncate_in_word(self):
-        my_sentence = "I am a very interesting sentence."
-        truncated_str = smart_truncate(my_sentence, 10)
-        self.assertEqual(truncated_str, "I am a...")
-
-    def test_smart_truncate_after_word(self):
-        my_sentence = "I am a very interesting sentence."
-        truncated_str = smart_truncate(my_sentence, 14)
-        self.assertEqual(truncated_str, "I am a very...")
-
-    def test_smart_truncate_changed_postfix(self):
-        my_sentence = "I am a very interesting sentence."
-        truncated_str = smart_truncate(my_sentence, 10, "[...]")
-        self.assertEqual(truncated_str, "I am a[...]")
-
-    def test_smart_truncate_not_cutting_on_too_short_strings(self):
-        my_sentence = "I am a very interesting sentence."
-        truncated_str = smart_truncate(my_sentence, 100, "---")
-        self.assertEqual(truncated_str, my_sentence)
-
-    def test_smart_truncate_no_text(self):
-        truncated_str = smart_truncate(None, 100, "---")
-        self.assertEqual(truncated_str, "")
-
-    def test_float_to_string_regular(self):
-        self.assertEqual(float_to_string(5.61), "5,61")
-
-    def test_float_to_string_value_replacement_not_used(self):
-        self.assertEqual(float_to_string(4.41, "-"), "4,41")
-
-    def test_float_to_string_no_value_replacement_used(self):
-        self.assertEqual(float_to_string(None, "Heureka"), "Heureka")
-
-    def test_float_to_string_value_greater_thousand(self):
-        self.assertEqual(float_to_string(1234.56), "1234,56")
-
-    def test_date_to_string_regular(self):
-        self.assertEqual(date_to_string(datetime.date(2020, 9, 19)), "19.09.2020")
-
-    def test_date_to_string_other_format(self):
-        self.assertEqual(date_to_string(datetime.date(2020, 9, 19), str_format="%Y-%m-%d"), "2020-09-19")
-
-    def test_date_to_string_replacement_undefined(self):
-        self.assertEqual(date_to_string(None), "-")
-
-    def test_date_to_string_replacement_defined(self):
-        self.assertEqual(date_to_string(None, "no date"), "no date")
-
-    def test_datetime_to_string_regular(self):
-        self.assertEqual(datetime_to_string(datetime.datetime(2020, 9, 19, 8, tzinfo=pytz.UTC)), "19.09.2020 08:00")
-
-    def test_datetime_to_string_other_format(self):
-        self.assertEqual(
-            datetime_to_string(datetime.datetime(2020, 9, 19, 8, tzinfo=pytz.UTC), str_format="%Y-%m-%d"), "2020-09-19"
-        )
-
-    def test_datetime_to_string_replacement_undefined(self):
-        self.assertEqual(datetime_to_string(None), "-")
-
-    def test_datetime_to_string_replacement_defined(self):
-        self.assertEqual(datetime_to_string(None, "no date"), "no date")
-
-    def test_number_to_string_regular(self):
-        self.assertEqual(number_to_string(5.61, decimal_digits=2), "5.61")
-
-    def test_number_to_string_value_replacement_not_used(self):
-        self.assertEqual(number_to_string(4.41, decimal_digits=2, replacement="-"), "4.41")
-
-    def test_number_to_string_no_value_replacement_used(self):
-        self.assertEqual(number_to_string(None, replacement="Heureka"), "Heureka")
-
-    def test_number_to_string_value_greater_thousand(self):
-        self.assertEqual(number_to_string(1234.56, decimal_digits=2), "1,234.56")
-
-    def test_number_to_string_int_value_no_digits(self):
-        self.assertEqual(number_to_string(117), "117")
-
-    def test_number_to_string_int_value_with_digits(self):
-        self.assertEqual(number_to_string(117, decimal_digits=2), "117.00")
-
-    def test_string_or_none_to_string_regular(self):
-        my_str = "I am a string."
-        self.assertEqual(string_or_none_to_string(my_str), my_str)
-
-    def test_string_or_none_to_string_replacement_undefined(self):
-        self.assertEqual(string_or_none_to_string(None), "-")
-
-    def test_string_or_none_to_string_replacement_defined(self):
-        self.assertEqual(string_or_none_to_string(None, "no value"), "no value")
-
-    def test_encode_to_xml_regular(self):
-        xml_str = "<tag>Something with an ampersand (&)</tag>"
-        self.assertEqual(encode_to_xml(xml_str), "&lt;tag&gt;Something with an ampersand (&amp;)&lt;/tag&gt;")
+import datetime
+
+import pytz
+from django.test import TestCase
+
+from ambient_toolbox.utils.string import (
+    date_to_string,
+    datetime_to_string,
+    distinct,
+    encode_to_xml,
+    float_to_string,
+    number_to_string,
+    slugify_file_name,
+    smart_truncate,
+    string_or_none_to_string,
+)
+
+
+class UtilsStringTest(TestCase):
+    def test_distinct_regular(self):
+        not_distinct_list = ["Beer", "Wine", "Whiskey", "Beer"]
+        distinct_list = distinct(not_distinct_list)
+
+        self.assertEqual(len(distinct_list), 3)
+        self.assertIn("Beer", distinct_list)
+        self.assertIn("Whiskey", distinct_list)
+        self.assertIn("Wine", distinct_list)
+
+    def test_slugify_file_name_regular(self):
+        filename = "hola and hello.txt"
+        slug = slugify_file_name(filename)
+        self.assertEqual(slug, "hola_and_hello.txt")
+
+    def test_slugify_file_name_nothing_to_slugify(self):
+        filename = "hola.txt"
+        slug = slugify_file_name(filename)
+        self.assertEqual(slug, filename)
+
+    def test_slugify_file_name_max_length(self):
+        filename = "a very long filename.txt"
+        slug = slugify_file_name(filename, 6)
+        self.assertEqual(slug, "a_very.txt")
+
+    def test_smart_truncate_in_word(self):
+        my_sentence = "I am a very interesting sentence."
+        truncated_str = smart_truncate(my_sentence, 10)
+        self.assertEqual(truncated_str, "I am a...")
+
+    def test_smart_truncate_after_word(self):
+        my_sentence = "I am a very interesting sentence."
+        truncated_str = smart_truncate(my_sentence, 14)
+        self.assertEqual(truncated_str, "I am a very...")
+
+    def test_smart_truncate_changed_postfix(self):
+        my_sentence = "I am a very interesting sentence."
+        truncated_str = smart_truncate(my_sentence, 10, "[...]")
+        self.assertEqual(truncated_str, "I am a[...]")
+
+    def test_smart_truncate_not_cutting_on_too_short_strings(self):
+        my_sentence = "I am a very interesting sentence."
+        truncated_str = smart_truncate(my_sentence, 100, "---")
+        self.assertEqual(truncated_str, my_sentence)
+
+    def test_smart_truncate_no_text(self):
+        truncated_str = smart_truncate(None, 100, "---")
+        self.assertEqual(truncated_str, "")
+
+    def test_float_to_string_regular(self):
+        self.assertEqual(float_to_string(5.61), "5,61")
+
+    def test_float_to_string_value_replacement_not_used(self):
+        self.assertEqual(float_to_string(4.41, "-"), "4,41")
+
+    def test_float_to_string_no_value_replacement_used(self):
+        self.assertEqual(float_to_string(None, "Heureka"), "Heureka")
+
+    def test_float_to_string_value_greater_thousand(self):
+        self.assertEqual(float_to_string(1234.56), "1234,56")
+
+    def test_date_to_string_regular(self):
+        self.assertEqual(date_to_string(datetime.date(2020, 9, 19)), "19.09.2020")
+
+    def test_date_to_string_other_format(self):
+        self.assertEqual(date_to_string(datetime.date(2020, 9, 19), str_format="%Y-%m-%d"), "2020-09-19")
+
+    def test_date_to_string_replacement_undefined(self):
+        self.assertEqual(date_to_string(None), "-")
+
+    def test_date_to_string_replacement_defined(self):
+        self.assertEqual(date_to_string(None, "no date"), "no date")
+
+    def test_datetime_to_string_regular(self):
+        self.assertEqual(datetime_to_string(datetime.datetime(2020, 9, 19, 8, tzinfo=pytz.UTC)), "19.09.2020 08:00")
+
+    def test_datetime_to_string_other_format(self):
+        self.assertEqual(
+            datetime_to_string(datetime.datetime(2020, 9, 19, 8, tzinfo=pytz.UTC), str_format="%Y-%m-%d"), "2020-09-19"
+        )
+
+    def test_datetime_to_string_replacement_undefined(self):
+        self.assertEqual(datetime_to_string(None), "-")
+
+    def test_datetime_to_string_replacement_defined(self):
+        self.assertEqual(datetime_to_string(None, "no date"), "no date")
+
+    def test_number_to_string_regular(self):
+        self.assertEqual(number_to_string(5.61, decimal_digits=2), "5.61")
+
+    def test_number_to_string_value_replacement_not_used(self):
+        self.assertEqual(number_to_string(4.41, decimal_digits=2, replacement="-"), "4.41")
+
+    def test_number_to_string_no_value_replacement_used(self):
+        self.assertEqual(number_to_string(None, replacement="Heureka"), "Heureka")
+
+    def test_number_to_string_value_greater_thousand(self):
+        self.assertEqual(number_to_string(1234.56, decimal_digits=2), "1,234.56")
+
+    def test_number_to_string_int_value_no_digits(self):
+        self.assertEqual(number_to_string(117), "117")
+
+    def test_number_to_string_int_value_with_digits(self):
+        self.assertEqual(number_to_string(117, decimal_digits=2), "117.00")
+
+    def test_string_or_none_to_string_regular(self):
+        my_str = "I am a string."
+        self.assertEqual(string_or_none_to_string(my_str), my_str)
+
+    def test_string_or_none_to_string_replacement_undefined(self):
+        self.assertEqual(string_or_none_to_string(None), "-")
+
+    def test_string_or_none_to_string_replacement_defined(self):
+        self.assertEqual(string_or_none_to_string(None, "no value"), "no value")
+
+    def test_encode_to_xml_regular(self):
+        xml_str = "<tag>Something with an ampersand (&)</tag>"
+        self.assertEqual(encode_to_xml(xml_str), "&lt;tag&gt;Something with an ampersand (&amp;)&lt;/tag&gt;")
```

### Comparing `ambient_toolbox-9.6.3/tests/tests/mixins/test_django_message_framework.py` & `ambient_toolbox-9.6.4/tests/tests/mixins/test_django_message_framework.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/tests/mixins/test_mixins.py` & `ambient_toolbox-9.6.4/tests/tests/mixins/test_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/tests/mixins/test_request_provider_mixin.py` & `ambient_toolbox-9.6.4/tests/tests/mixins/test_request_provider_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/tests/test_mail_backends.py` & `ambient_toolbox-9.6.4/tests/tests/test_mail_backends.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/validators/auth_password/test_special_chars.py` & `ambient_toolbox-9.6.4/tests/validators/auth_password/test_special_chars.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/view_layer/test_formset_mixins.py` & `ambient_toolbox-9.6.4/tests/view_layer/test_formset_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/view_layer/test_htmx_response_mixin.py` & `ambient_toolbox-9.6.4/tests/view_layer/test_htmx_response_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/view_layer/test_meta_mixins.py` & `ambient_toolbox-9.6.4/tests/view_layer/test_meta_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/tests/view_layer/test_views.py` & `ambient_toolbox-9.6.4/tests/view_layer/test_views.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-9.6.3/PKG-INFO` & `ambient_toolbox-9.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient-toolbox
-Version: 9.6.3
+Version: 9.6.4
 Summary: Python toolbox of Ambient Digital containing an abundance of useful tools and gadgets.
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Dist: Django>=3.2.20
 Requires-Dist: bleach>=1.4,<6
 Requires-Dist: python-dateutil>=2.5.3
+Requires-Dist: pytz
 Requires-Dist: typer~=0.9 ; extra == "dev"
 Requires-Dist: freezegun~=1.3 ; extra == "dev"
 Requires-Dist: pytest-django~=4.7 ; extra == "dev"
 Requires-Dist: pytest-mock~=3.12 ; extra == "dev"
 Requires-Dist: coverage~=7.3 ; extra == "dev"
 Requires-Dist: pre-commit~=3.5 ; extra == "dev"
 Requires-Dist: ruff~=0.1.7 ; extra == "dev"
@@ -55,15 +56,15 @@
 Provides-Extra: drf
 Provides-Extra: graphql
 Provides-Extra: sentry
 Provides-Extra: view-layer
 
 [![PyPI release](https://img.shields.io/pypi/v/ambient-toolbox.svg)](https://pypi.org/project/ambient-toolbox/)
 [![Downloads](https://static.pepy.tech/badge/ambient-toolbox)](https://pepy.tech/project/ambient-toolbox)
-[![Coverage](https://img.shields.io/badge/Coverage-96.52%25-success)](https://github.com/ambient-innovation/ambient-toolbox/actions?workflow=CI)
+[![Coverage](https://img.shields.io/badge/Coverage-86.51%25-success)](https://github.com/ambient-innovation/ambient-toolbox/actions?workflow=CI)
 [![Linting](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Coding Style](https://img.shields.io/badge/code%20style-Ruff-000000.svg)](https://github.com/astral-sh/ruff)
 [![Documentation Status](https://readthedocs.org/projects/ambient-toolbox/badge/?version=latest)](https://ambient-toolbox.readthedocs.io/en/latest/?badge=latest)
 
 Python toolbox of Ambient Digital containing an abundance of useful tools and gadgets.
 
 * [PyPI](https://pypi.org/project/ambient-toolbox/)
```

