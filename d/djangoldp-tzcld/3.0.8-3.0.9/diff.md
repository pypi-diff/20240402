# Comparing `tmp/djangoldp_tzcld-3.0.8.tar.gz` & `tmp/djangoldp_tzcld-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_tzcld-3.0.8.tar", last modified: Mon Jan 29 13:38:39 2024, max compression
+gzip compressed data, was "dist/djangoldp_tzcld-3.0.9.tar", last modified: Mon Jan 29 17:34:39 2024, max compression
```

## Comparing `djangoldp_tzcld-3.0.8.tar` & `djangoldp_tzcld-3.0.9.tar`

### file list

```diff
@@ -1,123 +1,127 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      831 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld.egg-info/
--rw-r--r--   0 root         (0) root         (0)      309 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     6223 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      306 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      309 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/
--rw-rw-rw-   0 root         (0) root         (0)      714 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/views.py
--rw-rw-rw-   0 root         (0) root         (0)    49499 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)     2088 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/password_change_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2333 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/password_reset_email.html
--rw-rw-rw-   0 root         (0) root         (0)     1970 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      650 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1290 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      538 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/lost_user.html
--rw-rw-rw-   0 root         (0) root         (0)      263 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/activate.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/logged_out.html
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      482 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/logout.html
--rw-rw-rw-   0 root         (0) root         (0)     4146 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/login.html
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/password_change_done.html
--rw-rw-rw-   0 root         (0) root         (0)      297 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/registration_complete.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/admin/
--rw-rw-rw-   0 root         (0) root         (0)     2458 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/admin/login.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/oidc_provider/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     2385 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/oidc_provider/authorize.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/django_registration/activation_email_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      620 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/django_registration/activation_email_body.txt
--rw-rw-rw-   0 root         (0) root         (0)      668 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/django_registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     2870 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/django_registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      399 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/django_registration/registration_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     3890 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)     1607 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/management/commands/create_community_related_objects.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-01-29 13:38:36.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/script/
--rw-rw-rw-   0 root         (0) root         (0)      461 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/script/deploy.sh
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/settings.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/djangoldp_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 13:38:39.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0036_auto_20230710_1703.py
--rw-rw-rw-   0 root         (0) root         (0)     5575 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py
--rw-rw-rw-   0 root         (0) root         (0)     4267 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0039_auto_20230711_1502.py
--rw-rw-rw-   0 root         (0) root         (0)     1140 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0052_auto_20231006_1250.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py
--rw-rw-rw-   0 root         (0) root         (0)     2754 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0053_auto_20231006_1300.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0043_auto_20230822_1742.py
--rw-rw-rw-   0 root         (0) root         (0)     9295 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py
--rw-rw-rw-   0 root         (0) root         (0)     1785 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0026_auto_20230703_1349.py
--rw-rw-rw-   0 root         (0) root         (0)     1099 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
--rw-rw-rw-   0 root         (0) root         (0)      960 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0038_tzcldterritoryregion_referers.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0002_tzcldcommunity_contact_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1836 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0046_rename_tzcldterritoriestrainingpromotoion_tzcldterritoriestrainingpromotion_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0058_rename_communityadmins_tzcldterritorysharedfile_community_admins_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0034_auto_20230710_1650.py
--rw-rw-rw-   0 root         (0) root         (0)      716 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0037_auto_20230710_1721.py
--rw-rw-rw-   0 root         (0) root         (0)     1550 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0050_auto_20230923_1422.py
--rw-rw-rw-   0 root         (0) root         (0)     5746 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0031_auto_20230706_1124.py
--rw-rw-rw-   0 root         (0) root         (0)     5854 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0032_auto_20230706_1509.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py
--rw-rw-rw-   0 root         (0) root         (0)     5617 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0057_alter_tzcldcommunitydeliberation_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1745 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0056_alter_tzcldterritorysynthesisfollowed_community.py
--rw-rw-rw-   0 root         (0) root         (0)     7009 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0059_tzcldterritoriesteamuserstate_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0025_auto_20230703_1343.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0040_auto_20230711_1512.py
--rw-rw-rw-   0 root         (0) root         (0)    17465 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0029_tzcldterritoryrequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0024_auto_20230703_1337.py
--rw-rw-rw-   0 root         (0) root         (0)    10081 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0023_auto_20230524_1456.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0054_tzcldcommunityidentity_conversations.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0060_rename_emergeance_date_tzcldcommunityidentity_emergence_date.py
--rw-rw-rw-   0 root         (0) root         (0)     4403 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py
--rw-rw-rw-   0 root         (0) root         (0)      910 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0042_auto_20230822_1724.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
--rw-rw-rw-   0 root         (0) root         (0)     5671 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0030_tzcldfollowedtrainingb_tzcldfollowedtrainingd_tzcldterritorysynthesisfollowed.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0022_tzcldcommunity_membership_organisation_name.py
--rw-rw-rw-   0 root         (0) root         (0)     1176 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0051_auto_20231006_1244.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0048_auto_20230904_1421.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
--rw-rw-rw-   0 root         (0) root         (0)     1175 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0044_auto_20230823_1237.py
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0062_tzcldcommunityidentity_birth_date.py
--rw-rw-rw-   0 root         (0) root         (0)    16662 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0033_auto_20230710_1223.py
--rw-rw-rw-   0 root         (0) root         (0)     3260 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0061_tzcldterritorycirconscription_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      920 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0045_auto_20230823_1242.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0041_auto_20230712_1141.py
--rw-rw-rw-   0 root         (0) root         (0)     1787 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0049_tzcldsharednote_date.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py
--rw-rw-rw-   0 root         (0) root         (0)     1281 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0063_remove_tzcldterritorypoliticallandscapedeputy_circonscriptions_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
--rw-rw-rw-   0 root         (0) root         (0)    18077 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0064_alter_tzcldcommunity_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     3648 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0028_tzcldsharednote_tzcldsharednotecomment.py
--rw-rw-rw-   0 root         (0) root         (0)      466 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0027_tzcldcommunityevaluationpointanswer_answer_option.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py
--rw-rw-rw-   0 root         (0) root         (0)     1659 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0055_auto_20231006_1539.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0047_auto_20230901_1744.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2024-01-29 13:38:12.000000 djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0035_auto_20230710_1657.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      831 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      309 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     6527 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      306 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      309 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/
+-rw-rw-rw-   0 root         (0) root         (0)      714 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/views.py
+-rw-rw-rw-   0 root         (0) root         (0)    49673 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)     2088 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/password_change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2333 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      650 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 17:34:09.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      538 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/lost_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/activate.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/logged_out.html
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/logout.html
+-rw-rw-rw-   0 root         (0) root         (0)     4146 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/login.html
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/password_change_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      297 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/registration_complete.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     2458 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/admin/login.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 17:34:09.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/oidc_provider/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     2385 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/oidc_provider/authorize.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/django_registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      620 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/django_registration/activation_email_body.txt
+-rw-rw-rw-   0 root         (0) root         (0)      668 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/django_registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     2870 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/django_registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      399 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/django_registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     3890 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/management/commands/create_community_related_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 17:34:09.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-01-29 17:34:36.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/script/
+-rw-rw-rw-   0 root         (0) root         (0)      461 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/script/deploy.sh
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/djangoldp_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 17:34:39.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      659 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0066_tzcldterritorytraining_training_person.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0036_auto_20230710_1703.py
+-rw-rw-rw-   0 root         (0) root         (0)     5575 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py
+-rw-rw-rw-   0 root         (0) root         (0)     4267 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0039_auto_20230711_1502.py
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0052_auto_20231006_1250.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py
+-rw-rw-rw-   0 root         (0) root         (0)     2754 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0053_auto_20231006_1300.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0043_auto_20230822_1742.py
+-rw-rw-rw-   0 root         (0) root         (0)     9295 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py
+-rw-rw-rw-   0 root         (0) root         (0)     1785 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0026_auto_20230703_1349.py
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
+-rw-rw-rw-   0 root         (0) root         (0)      960 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0038_tzcldterritoryregion_referers.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0002_tzcldcommunity_contact_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0046_rename_tzcldterritoriestrainingpromotoion_tzcldterritoriestrainingpromotion_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0058_rename_communityadmins_tzcldterritorysharedfile_community_admins_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 17:34:09.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0034_auto_20230710_1650.py
+-rw-rw-rw-   0 root         (0) root         (0)      716 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0037_auto_20230710_1721.py
+-rw-rw-rw-   0 root         (0) root         (0)     1550 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0050_auto_20230923_1422.py
+-rw-rw-rw-   0 root         (0) root         (0)     5746 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0031_auto_20230706_1124.py
+-rw-rw-rw-   0 root         (0) root         (0)     5854 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0032_auto_20230706_1509.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py
+-rw-rw-rw-   0 root         (0) root         (0)      373 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0067_remove_tzcldcommunity_primary_contact.py
+-rw-rw-rw-   0 root         (0) root         (0)     5617 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0057_alter_tzcldcommunitydeliberation_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0056_alter_tzcldterritorysynthesisfollowed_community.py
+-rw-rw-rw-   0 root         (0) root         (0)     7009 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0059_tzcldterritoriesteamuserstate_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      461 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0025_auto_20230703_1343.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0040_auto_20230711_1512.py
+-rw-rw-rw-   0 root         (0) root         (0)    17465 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0029_tzcldterritoryrequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0024_auto_20230703_1337.py
+-rw-rw-rw-   0 root         (0) root         (0)    10081 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0023_auto_20230524_1456.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0054_tzcldcommunityidentity_conversations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0065_remove_tzcldterritorysynthesisfollowed_context_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0060_rename_emergeance_date_tzcldcommunityidentity_emergence_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     4403 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0068_tzcldcommunity_primary_contact.py
+-rw-rw-rw-   0 root         (0) root         (0)      910 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0042_auto_20230822_1724.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
+-rw-rw-rw-   0 root         (0) root         (0)     5671 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0030_tzcldfollowedtrainingb_tzcldfollowedtrainingd_tzcldterritorysynthesisfollowed.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0022_tzcldcommunity_membership_organisation_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0051_auto_20231006_1244.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0048_auto_20230904_1421.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0044_auto_20230823_1237.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0062_tzcldcommunityidentity_birth_date.py
+-rw-rw-rw-   0 root         (0) root         (0)    16662 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0033_auto_20230710_1223.py
+-rw-rw-rw-   0 root         (0) root         (0)     3260 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0061_tzcldterritorycirconscription_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      920 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0045_auto_20230823_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0041_auto_20230712_1141.py
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0049_tzcldsharednote_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py
+-rw-rw-rw-   0 root         (0) root         (0)     1281 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0063_remove_tzcldterritorypoliticallandscapedeputy_circonscriptions_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)    18077 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0064_alter_tzcldcommunity_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     3648 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0028_tzcldsharednote_tzcldsharednotecomment.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0027_tzcldcommunityevaluationpointanswer_answer_option.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0055_auto_20231006_1539.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0047_auto_20230901_1744.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2024-01-29 17:34:08.000000 djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0035_auto_20230710_1657.py
```

### Comparing `djangoldp_tzcld-3.0.8/setup.cfg` & `djangoldp_tzcld-3.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld.egg-info/SOURCES.txt` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,18 @@
 djangoldp_tzcld/migrations/0058_rename_communityadmins_tzcldterritorysharedfile_community_admins_and_more.py
 djangoldp_tzcld/migrations/0059_tzcldterritoriesteamuserstate_and_more.py
 djangoldp_tzcld/migrations/0060_rename_emergeance_date_tzcldcommunityidentity_emergence_date.py
 djangoldp_tzcld/migrations/0061_tzcldterritorycirconscription_and_more.py
 djangoldp_tzcld/migrations/0062_tzcldcommunityidentity_birth_date.py
 djangoldp_tzcld/migrations/0063_remove_tzcldterritorypoliticallandscapedeputy_circonscriptions_and_more.py
 djangoldp_tzcld/migrations/0064_alter_tzcldcommunity_options_and_more.py
+djangoldp_tzcld/migrations/0065_remove_tzcldterritorysynthesisfollowed_context_and_more.py
+djangoldp_tzcld/migrations/0066_tzcldterritorytraining_training_person.py
+djangoldp_tzcld/migrations/0067_remove_tzcldcommunity_primary_contact.py
+djangoldp_tzcld/migrations/0068_tzcldcommunity_primary_contact.py
 djangoldp_tzcld/migrations/__init__.py
 djangoldp_tzcld/script/deploy.sh
 djangoldp_tzcld/templates/admin/login.html
 djangoldp_tzcld/templates/django_registration/activation_complete.html
 djangoldp_tzcld/templates/django_registration/activation_email_body.txt
 djangoldp_tzcld/templates/django_registration/activation_email_subject.txt
 djangoldp_tzcld/templates/django_registration/registration_complete.html
```

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/views.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/models.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,15 +390,16 @@
     kind = models.ForeignKey(TzcldTerritoriesKind, on_delete=models.DO_NOTHING,related_name='kind', blank=True, null=True)
     step_state = models.ForeignKey(TzcldTerritoriesStepState, on_delete=models.DO_NOTHING,related_name='step_state', blank=False, null=True)
     regions = models.ManyToManyField(TzcldTerritoryRegion, related_name='community_regions', blank=True)
     departments = models.ManyToManyField(TzcldTerritoryDepartment, related_name='community_departments', blank=True)
     membership = models.ForeignKey(TzcldProfilesMembership, on_delete=models.DO_NOTHING,related_name='membership', blank=False, null=True)
     membership_organisation_name = models.CharField(max_length=254, blank=True, null=True, default='')
     visible = models.BooleanField(default=True)
-    primary_contact = models.ForeignKey(CommunityMember, on_delete=models.DO_NOTHING,related_name='primary_contact', blank=True, null=True)
+    primary_contact = models.ForeignKey(settings.AUTH_USER_MODEL, related_name='primary_contact', blank=True, null=True, on_delete=models.SET_NULL)
+    information = models.TextField(blank=True, null=True)
 
     def __str__(self):
         try:
             return '{} ({})'.format(self.community.urlid, self.urlid)
         except:
             return self.urlid
 
@@ -407,15 +408,15 @@
         verbose_name_plural = _("TZCLD Territories Profiles")
         
         # authenticated_perms = ['view', 'add']
         # owner_perms = ['inherit', 'change', 'delete']
         # superuser_perms = ['inherit']
         ordering = ['community']
         container_path = "tzcld-communities/"
-        serializer_fields = ['@id', 'community', 'kind', 'step_state', 'kind', 'departments', 'regions', 'locations', 'primary_contact', 'membership', 'membership_organisation_name', 'visible']
+        serializer_fields = ['@id', 'community', 'kind', 'step_state', 'kind', 'departments', 'regions', 'locations', 'primary_contact', 'membership', 'membership_organisation_name', 'visible', 'information']
         rdf_type = "tzcld:communityProfile"
         nested_fields = ['regions', 'departments', 'locations']
         permission_classes=[LDPBasePermission]
         depth = 0
 
 class TzcldCommunityIdentity(Model):
     community = models.OneToOneField(Community, on_delete=models.CASCADE, related_name='tzcld_profile_identity', null=True, blank=True)
@@ -557,15 +558,15 @@
         nested_fields = ['community_identity']
         rdf_type = "tzcld:territoryPoliticalLandscapeSenator"
         permission_classes=[LDPBasePermission]
 
 class TzcldTerritoryTraining(Model):
     training_course = models.ForeignKey(TzcldTerritoriesTrainingCourse, on_delete=models.DO_NOTHING,related_name='territory_training_course', blank=True, null=True)
     training_promotion = models.ForeignKey(TzcldTerritoriesTrainingPromotion, on_delete=models.DO_NOTHING,related_name='territory_training_promotion', blank=True, null=True)
-    training_person = models.CharField(max_length=255, blank=True, null=True, default='')
+    training_person = models.ForeignKey(settings.AUTH_USER_MODEL, null=True, on_delete=models.SET_NULL)
     community_identity = models.ForeignKey(TzcldCommunityIdentity, on_delete=models.CASCADE,related_name='territories_trainings', blank=True, null=True)
 
     def __str__(self):
         try:
             return '{} ({})'.format(self.community_identity.urlid, self.urlid)
         except:
             return self.urlid
@@ -689,14 +690,15 @@
         (TYPE_FALSE, 'Checkboxe'),
         (TYPE_DELIBERATION, 'TZCLD Territory deliberation'),
         (TYPE_OTHER_DELIBERATION, 'TZCLD Other Territory deliberation'),
         (TYPE_CONCILS_DELIBERATION, 'TZCLD Council department deliberation'),
     ]
 
     name = models.CharField(max_length=1024, blank=True, null=True, default='')
+    description = models.CharField(max_length=1024, blank=True, null=True, default='')
     order = models.IntegerField(blank=True, null=True, default=1)
     part = models.ForeignKey(TzcldCommunityEvaluationPointPart, on_delete=models.CASCADE,related_name='part_points', blank=True, null=True)
     points = models.IntegerField(blank=True, null=True, default=0)
     fieldType = models.CharField(
         max_length=125,
         choices=TYPE_OF_FIELD_CHOICES,
         default=TYPE_FALSE,
@@ -713,15 +715,15 @@
         verbose_name_plural = _("TZCLD Territories Evaluation Points")
         
         # authenticated_perms = ['view', 'add']
         # owner_perms = ['inherit', 'change', 'delete']
         # superuser_perms = ['inherit']
         ordering = ['order']
         container_path = "tzcld-communities-evaluation-points/"
-        serializer_fields = ['@id', 'name', 'order', 'part', 'points', 'fieldType', 'evaluation_point_answer']
+        serializer_fields = ['@id', 'name', 'description', 'order', 'part', 'points', 'fieldType', 'evaluation_point_answer']
         rdf_type = "tzcld:communityEvaluationPoint"
         permission_classes=[LDPBasePermission]
         depth = 0
 
 
 class TzcldCommunityEvaluationPointAnswer(Model):
 
@@ -838,16 +840,16 @@
         nested_fields = ['user', 'community']
         rdf_type = "tzcld:territoryRequest"
         permission_classes=[LDPBasePermission]
 
 
 class TzcldTerritorySynthesisFollowed(Model):
     
-    context = models.TextField(blank=True, null=True, verbose_name="Context")
-    strongPoints = models.TextField(blank=True, null=True, verbose_name="Strong Points")
+    # context = models.TextField(blank=True, null=True, verbose_name="Context")
+    # strongPoints = models.TextField(blank=True, null=True, verbose_name="Strong Points")
     questions = models.TextField(blank=True, null=True, verbose_name="Questions")
     needs = models.TextField(blank=True, null=True, verbose_name="Needs, Actions")
     targetdate =  models.DateField(verbose_name="Target date", blank=True, null=True)
     community = models.OneToOneField(Community, on_delete=models.DO_NOTHING,related_name='tzcld_community_synthesis_followed', blank=False, null=True)
     date =  models.DateField(verbose_name="Date", auto_now=True)
     author = models.ForeignKey(settings.AUTH_USER_MODEL, null=True, on_delete=models.SET_NULL)
 
@@ -862,15 +864,15 @@
         verbose_name = _('TZCLD Territory Synthesis Followed')
         verbose_name_plural = _("TZCLD Territories Synthesis Followed")
         
         # authenticated_perms = ['view', 'add']
         # owner_perms = ['inherit', 'change', 'delete']
         # superuser_perms = ['inherit']
         container_path = "tzcld-territory-synthesis-followed/"
-        serializer_fields = ['@id', 'context', 'strongPoints', 'questions', 'needs', 'targetdate', 'community', 'tzcld_referents_community_shared_notes', 'date', 'author', 'tzcld_referents_community_shared_files']
+        serializer_fields = ['@id', 'questions', 'needs', 'targetdate', 'community', 'tzcld_referents_community_shared_notes', 'date', 'author', 'tzcld_referents_community_shared_files']
         nested_fields = ['community', 'tzcld_referents_community_shared_notes', 'tzcld_referents_community_shared_files']
         rdf_type = "tzcld:territorySynthesisFollowed"
         permission_classes=[LDPBasePermission]
 
 
 class TzcldCommunityFollowedPointPart(Model):
     name = models.CharField(max_length=254, blank=True, null=True, default='')
```

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/password_change_form.html` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/password_reset_email.html` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/password_reset_confirm.html` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/activation_complete.html` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/password_reset_form.html` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/password_reset_complete.html` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/registration_closed.html` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/registration_closed.html`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/registration/login.html` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/admin/login.html` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/oidc_provider/authorize.html` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/django_registration/activation_email_body.txt` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/django_registration/activation_email_body.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/django_registration/activation_complete.html` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/django_registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/templates/django_registration/registration_form.html` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/templates/django_registration/registration_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/admin.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/management/commands/create_community_related_objects.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/management/commands/create_community_related_objects.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0036_auto_20230710_1703.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0036_auto_20230710_1703.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0039_auto_20230711_1502.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0039_auto_20230711_1502.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0052_auto_20231006_1250.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0052_auto_20231006_1250.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0053_auto_20231006_1300.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0053_auto_20231006_1300.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0043_auto_20230822_1742.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0043_auto_20230822_1742.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0001_initial.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0026_auto_20230703_1349.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0026_auto_20230703_1349.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0038_tzcldterritoryregion_referers.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0038_tzcldterritoryregion_referers.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0046_rename_tzcldterritoriestrainingpromotoion_tzcldterritoriestrainingpromotion_and_more.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0046_rename_tzcldterritoriestrainingpromotoion_tzcldterritoriestrainingpromotion_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0058_rename_communityadmins_tzcldterritorysharedfile_community_admins_and_more.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0058_rename_communityadmins_tzcldterritorysharedfile_community_admins_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0034_auto_20230710_1650.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0034_auto_20230710_1650.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0037_auto_20230710_1721.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0037_auto_20230710_1721.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0050_auto_20230923_1422.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0050_auto_20230923_1422.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0031_auto_20230706_1124.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0031_auto_20230706_1124.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0032_auto_20230706_1509.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0032_auto_20230706_1509.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0057_alter_tzcldcommunitydeliberation_options_and_more.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0057_alter_tzcldcommunitydeliberation_options_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0056_alter_tzcldterritorysynthesisfollowed_community.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0056_alter_tzcldterritorysynthesisfollowed_community.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0059_tzcldterritoriesteamuserstate_and_more.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0059_tzcldterritoriesteamuserstate_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0040_auto_20230711_1512.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0040_auto_20230711_1512.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0029_tzcldterritoryrequest.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0029_tzcldterritoryrequest.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0024_auto_20230703_1337.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0024_auto_20230703_1337.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0023_auto_20230524_1456.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0023_auto_20230524_1456.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0054_tzcldcommunityidentity_conversations.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0054_tzcldcommunityidentity_conversations.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0042_auto_20230822_1724.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0042_auto_20230822_1724.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0030_tzcldfollowedtrainingb_tzcldfollowedtrainingd_tzcldterritorysynthesisfollowed.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0030_tzcldfollowedtrainingb_tzcldfollowedtrainingd_tzcldterritorysynthesisfollowed.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0051_auto_20231006_1244.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0051_auto_20231006_1244.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0044_auto_20230823_1237.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0044_auto_20230823_1237.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0033_auto_20230710_1223.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0033_auto_20230710_1223.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0061_tzcldterritorycirconscription_and_more.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0061_tzcldterritorycirconscription_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0045_auto_20230823_1242.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0045_auto_20230823_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0041_auto_20230712_1141.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0041_auto_20230712_1141.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0063_remove_tzcldterritorypoliticallandscapedeputy_circonscriptions_and_more.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0063_remove_tzcldterritorypoliticallandscapedeputy_circonscriptions_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0064_alter_tzcldcommunity_options_and_more.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0064_alter_tzcldcommunity_options_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0028_tzcldsharednote_tzcldsharednotecomment.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0028_tzcldsharednote_tzcldsharednotecomment.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0055_auto_20231006_1539.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0055_auto_20231006_1539.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-3.0.8/djangoldp_tzcld/migrations/0035_auto_20230710_1657.py` & `djangoldp_tzcld-3.0.9/djangoldp_tzcld/migrations/0035_auto_20230710_1657.py`

 * *Files identical despite different names*

