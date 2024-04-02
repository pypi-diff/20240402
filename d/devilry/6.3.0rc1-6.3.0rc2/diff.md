# Comparing `tmp/devilry-6.3.0rc1.tar.gz` & `tmp/devilry-6.3.0rc2.tar.gz`

## Comparing `devilry-6.3.0rc1.tar` & `devilry-6.3.0rc2.tar`

### file list

```diff
@@ -1,1670 +1,1673 @@
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/.coveragerc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/__init__.py
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/admin.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/apps.py
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/baker_recipes.py
--rw-r--r--   0        0        0    10440 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/deliverystore.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/devilry_core_baker_factories.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/group_user_lookup.py
--rw-r--r--   0        0        0    39763 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/testhelper.py
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/testhelpers.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/api/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/api/applicationstate.py
--rw-r--r--   0        0        0    34188 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0001_initial.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0002_auto_20150915_1127.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0003_auto_20150917_1537.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0004_examiner_relatedexaminer.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0005_relatedexaminer_automatic_anonymous_id.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0006_auto_20151112_1851.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0007_assignment_gradeform_setup_json.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0008_auto_20151222_1955.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0009_assignmentgroup_batchoperation.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0010_assignment_anonymizationmode.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0011_datamigrate_anonymous_to_anonymizationmode.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0012_auto_20160111_2019.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0013_auto_20160111_2021.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0014_auto_20160112_1052.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0015_assignment_uses_custom_candidate_ids.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0016_auto_20160112_1831.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0017_candidate_relatedstudent_replaces_student_field.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0018_auto_20160112_1923.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0019_auto_20160113_2037.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0020_relatedexaminer_active.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0021_examiner_relatedexaminer_replaces_user_field.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0022_auto_20160114_1520.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0023_auto_20160114_1522.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0024_auto_20160114_1524.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0025_auto_20160114_1525.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0026_auto_20160114_1528.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0027_auto_20160116_1843.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0028_auto_20160119_0337.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0029_assignmentgrouphistory.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0030_auto_20170124_1504.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0031_auto_20170125_1601.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0032_datamigrate_update_for_no_none_values_in_assignment_firstdeadline.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0033_auto_20170220_1330.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0034_auto_20170303_1308.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0035_auto_20170523_1747.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0036_auto_20170523_1748.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0037_auto_20170620_1515.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0038_auto_20170621_1720.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0039_assignmentgroup_internal_is_being_deleted.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0040_auto_20180214_1654.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0041_auto_20180220_0651.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0042_candidateassignmentgrouphistory_examinerassignmentgrouphistory.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0043_auto_20180302_1139.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0044_auto_20190624_1238.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0045_auto_20210427_1350.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/0046_auto_20220519_1043.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/migrations/__init__.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/__init__.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/abstract_applicationkeyvalue.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/abstract_is_admin.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/abstract_is_candidate.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/abstract_is_examiner.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/administrators.py
--rw-r--r--   0        0        0    50913 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/assignment.py
--rw-r--r--   0        0        0    76482 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/assignment_group.py
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/assignment_group_history.py
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/basenode.py
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/candidate.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/custom_db_fields.py
--rw-r--r--   0        0        0    16062 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/deadline.py
--rw-r--r--   0        0        0    13166 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/delivery.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/deliverytypes.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/devilryuserprofile.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/examiner.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/examiner_candidate_group_history.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/filemeta.py
--rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/groupinvite.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/model_utils.py
--rw-r--r--   0        0        0    10652 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/period.py
--rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/period_tag.py
--rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/pointrange_to_grade.py
--rw-r--r--   0        0        0    19027 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/relateduser.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/save_interface.py
--rw-r--r--   0        0        0    10883 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/static_feedback.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/models/subject.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/comment-summary.django.html
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-base-plain.django.html
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-base.django.html
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-full-plain.django.html
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-full.django.html
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-short.django.html
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/groupstatus.django.html
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/multiple-candidates-long-displayname.django.html
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/multiple-candidates-short-displayname.django.html
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/multiple-examiners-long-displayname.django.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/multiple-examiners-short-displayname.django.html
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/period-tags-on-period.django.html
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/relatedexaminers-on-period-tag.django.html
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/relatedstudents-on-period-tag.django.html
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/relatedusers-on-period-tag.django.html
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/single-candidate-long-displayname.django.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/single-candidate-short-displayname.django.html
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/single-examiner-long-displayname-plain.django.html
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/single-examiner-long-displayname.django.html
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/single-examiner-short-displayname.django.html
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/search/indexes/core/assignment_text.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/search/indexes/core/assignmentgroup_candidates.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/search/indexes/core/assignmentgroup_examiners.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/search/indexes/core/assignmentgroup_tags.txt
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/search/indexes/core/assignmentgroup_text.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/search/indexes/core/basenode_text.txt
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/search/indexes/core/format_user.django.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/search/indexes/core/node_text.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/search/indexes/core/period_text.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templates/search/indexes/core/subject_text.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templatetags/__init__.py
--rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/templatetags/devilry_core_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/__init__.py
--rw-r--r--   0        0        0    79383 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_assignment.py
--rw-r--r--   0        0        0   180651 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_assignment_group.py
--rw-r--r--   0        0        0     8857 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_assignment_group_history.py
--rw-r--r--   0        0        0     8276 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_candidate.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_deadline.py
--rw-r--r--   0        0        0    78327 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_devilry_core_tags.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_examiner.py
--rw-r--r--   0        0        0    30450 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_group_user_lookup.py
--rw-r--r--   0        0        0    28214 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_groupinvite.py
--rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_period.py
--rw-r--r--   0        0        0    12030 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_period_tags.py
--rw-r--r--   0        0        0    19992 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_pointrange_to_grade.py
--rw-r--r--   0        0        0    38546 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_relateduser.py
--rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/tests/test_subject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/views/__init__.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/apps/core/views/download_staticfeedbackfileattachment.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/coreutils/__init__.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/coreutils/utils.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/defaults/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/defaults/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/__init__.py
--rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/admin.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/apps.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/baker_recipes.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/crinstance_account.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/exceptions.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/middleware.py
--rw-r--r--   0        0        0    52183 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/models.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/urls.py
--rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/user_merger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/authbackend/__init__.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/authbackend/default.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/authbackend/ldap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/cradminextensions/__init__.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/cradminextensions/devilry_crmenu_account.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/crapps/__init__.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/crapps/account/__init__.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/crapps/account/index.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/crapps/account/select_language.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/crapps/account/utils.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/migrations/0001_initial.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/migrations/0002_auto_20150917_1731.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/migrations/0003_datamigrate-admins-into-permissiongroups.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/migrations/0004_auto_20151222_1955.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/migrations/0005_auto_20160113_2037.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/migrations/0006_auto_20160120_0424.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/migrations/0007_auto_20210427_1350.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/migrations/0008_auto_20220510_1307.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/migrations/0009_mergeduser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/migrations/__init__.py
--rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/templates/devilry_account/crapps/account/select_language.django.html
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/templates/devilry_account/templatetags/multiple-users-verbose-inline.django.html
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/templates/devilry_account/templatetags/user-verbose-inline-plain.django.html
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/templates/devilry_account/templatetags/user-verbose-inline.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/templatetags/__init__.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/templatetags/devilry_account_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/tests/__init__.py
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/tests/test_devilry_account_tags.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/tests/test_middleware.py
--rw-r--r--   0        0        0    46608 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/tests/test_models.py
--rw-r--r--   0        0        0    16979 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/tests/test_user_merger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/tests/authbackend/__init__.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/tests/authbackend/test_default.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/tests/test_crapps/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/tests/test_crapps/test_account/__init__.py
--rw-r--r--   0        0        0    18890 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/tests/test_crapps/test_account/test_index.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_account/tests/test_crapps/test_account/test_select_language.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/__init__.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/models.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tasks.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/__init__.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/devilry_crinstance_admin.py
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/devilry_crmenu_admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_assignmentgroup.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedexaminer.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedstudent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listfilter/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listfilter/listfilter_assignmentgroup.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listfilter/listfilter_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/multiselect2/__init__.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/multiselect2/multiselect2_relatedstudent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/listbuilder/__init__.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/listbuilder/admindashboard_subject_listbuilder.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/overview.django.html
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/add_groups_to_examiner.django.html
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/examinerdetails.django.html
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/overview.django.html
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/remove_groups_from_examiner.django.html
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-add.django.html
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-replace.django.html
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag-item-value.django.html
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag.django.html
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/random.django.html
--rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/select_method.django.html
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/custom-table.django.html
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/gradingconfiguration-update.django.html
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/examiners.django.html
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/gradingconfiguration.django.html
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/published.django.html
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/settings.django.html
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/statistics.django.html
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/students.django.html
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/utilities.django.html
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/includes/batchdownload_assignment.django.html
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-item-value.django.html
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-overview.django.html
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/candidate-item-value.django.html
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/confirm-view.django.html
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/overview.django.html
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select-period-view.django.html
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select_groups_to_pass.django.html
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/statistics/overview.django.html
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups.django.html
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/merge_groups.django.html
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/overview.django.html
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/split_groups.django.html
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-accumulated-score.django.html
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-assignment-item-value.django.html
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-method.django.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-period-item-value.django.html
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/confirm.django.html
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/manual-select-students.django.html
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/preview-relatedstudent-item-value.django.html
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/preview.django.html
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/select-assignments.django.html
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/selectable-assignment-item-value.django.html
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/selected-assignment-item-value.django.html
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/includes/select-assignment-item-value-description.django.html
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-assignment-item-value.django.html
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-method.django.html
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-period-item-value.django.html
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/confirm.django.html
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupdetails/details-renderable.django.html
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupdetails/view.django.html
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupview_base/base-info-view.django.html
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupview_base/base-multiselect-view.django.html
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupview_base/include/no-items-message.django.html
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/common/abstract-type-in-users.django.html
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/common/admin-list-view.django.html
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/common/admins-explained.django.html
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/overview.django.html
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/group_by_assignment.django.html
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_groups.django.html
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_users.django.html
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/listbuilder/admindashboard_subject_listbuilder/value.django.html
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/listbuilder/assignmentgroup_listbuilder/value.django.html
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/listbuilder/listbuilder_relatedexaminer/onassignment-itemvalue.django.html
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/listbuilder/listbuilder_relatedstudent/readonly-itemvalue.django.html
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/multiselect2/multiselect2_relatedstudent/itemvalue.django.html
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/multiselect2/multiselect2_relatedstudent/selecteditem.django.html
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/overview.django.html
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/admins/add.django.html
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/admins/overview-itemvalue.django.html
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/admins/overview.django.html
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/column_header_item.django.html
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/devilry_admin_all_results_overview_table.django.html
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/devilry_all_results_overview.django.html
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/result_cell_value.django.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/student_cell_value.django.html
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/createassignment.django.html
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/helpbox.django.html
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/success_message.django.html
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/suggested_deadlines.django.html
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/edit/updateview.django.html
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/examiners/add.django.html
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview-itemvalue.django.html
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview.django.html
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/add-tag.django.html
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/base-multiselect-view.django.html
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/crud.django.html
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/delete.django.html
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/manage-tags-list-view.django.html
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/tag-item-value.django.html
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/relatedusers/select-method.django.html
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/qualifiedforfinalexams/statuslistview-info-column.django.html
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/qualifiedforfinalexams/userlistview-info-column.django.html
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/add.django.html
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/overview-itemvalue.django.html
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/overview.django.html
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/students-not-added-to-assignments-warning.django.html
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/userselectview-no-searchresults-message.django.html
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/overview.django.html
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/overview_for_period_admins.html
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/admins/add.django.html
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview-itemvalue.django.html
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview.django.html
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/edit/updateview.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/__init__.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_anonymizationmode.py
--rw-r--r--   0        0        0    44944 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_batchframework_tasks.py
--rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_crinstance_assignment.py
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_deadline_handling.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_examiner_selfassign.py
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_examiner_statistics.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_first_deadline.py
--rw-r--r--   0        0        0    12214 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_grading_configuration.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_long_and_shortname.py
--rw-r--r--   0        0        0    48383 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_overview.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_projectgroups.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_publishing_time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/examiners/__init__.py
--rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_add_groups_to_examiner.py
--rw-r--r--   0        0        0    63295 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_bulk_organize.py
--rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_examinerdetails.py
--rw-r--r--   0        0        0    12880 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_overview.py
--rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_remove_groups_from_examiner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/__init__.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_overview.py
--rw-r--r--   0        0        0    51914 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period.py
--rw-r--r--   0        0        0    10256 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period_manual.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/__init__.py
--rw-r--r--   0        0        0    44849 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_create_groups.py
--rw-r--r--   0        0        0    45703 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_create_groups_accumulated_score.py
--rw-r--r--   0        0        0    46531 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_delete_groups.py
--rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupdetails.py
--rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_merge_groups.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_overview.py
--rw-r--r--   0        0        0    50909 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_replace_groups.py
--rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_split_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/__init__.py
--rw-r--r--   0        0        0    19748 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_baseinforview.py
--rw-r--r--   0        0        0    19777 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_basemultiselectview.py
--rw-r--r--   0        0        0    77200 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_groupviewmixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_download_files/__init__.py
--rw-r--r--   0        0        0    33016 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_download_files/test_batchdownload_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/common/__init__.py
--rw-r--r--   0        0        0    16683 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/common/admins_common_testmixins.py
--rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/common/test_bulkimport_users_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/cradminextensions/__init__.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/cradminextensions/test_devilry_crmenu_admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/__init__.py
--rw-r--r--   0        0        0     8928 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedexaminer.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedstudent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/cradminextensions/test_multiselect2/__init__.py
--rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/cradminextensions/test_multiselect2/test_multiselect2_relatedstudent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/dashboard/__init__.py
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/dashboard/test_createsubject.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/dashboard/test_crinstance_dashboard.py
--rw-r--r--   0        0        0    18818 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/dashboard/test_overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/__init__.py
--rw-r--r--   0        0        0    29261 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_assignment_listview.py
--rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_student_listview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/__init__.py
--rw-r--r--   0        0        0    29781 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_admins.py
--rw-r--r--   0        0        0    40873 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_createassignment.py
--rw-r--r--   0        0        0    15268 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_crinstance_period.py
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_edit.py
--rw-r--r--   0        0        0    34091 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_examiners.py
--rw-r--r--   0        0        0    19450 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_overview.py
--rw-r--r--   0        0        0    10863 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_overview_all_results.py
--rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_period_all_results_collector.py
--rw-r--r--   0        0        0    34017 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_students.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_manage_tags/__init__.py
--rw-r--r--   0        0        0    51030 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags.py
--rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags_relatedusers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_report/__init__.py
--rw-r--r--   0        0        0    42098 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_report/test_all_results_generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/subject/__init__.py
--rw-r--r--   0        0        0    26747 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/subject/test_admins.py
--rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/subject/test_createperiod.py
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/subject/test_crinstance_subject.py
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/subject/test_edit.py
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/subject/test_overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/__init__.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/test_crinstance_for_periodadmin.py
--rw-r--r--   0        0        0    11399 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/test_overview_for_periodadmin.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/test_subject_redirect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/__init__.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/anonymizationmode.py
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/crinstance_assignment.py
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/deadline_handling.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiner_selfassign.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/first_deadline.py
--rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/gradingconfiguration.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/long_and_shortname.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/overview.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/projectgroups.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/publishing_time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/download_files/__init__.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/download_files/backends.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/download_files/batch_download_api.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/download_files/download_archive.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiners/__init__.py
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiners/add_groups_to_examiner.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiners/base_single_examinerview.py
--rw-r--r--   0        0        0    24438 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiners/bulk_organize.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiners/examinerdetails.py
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiners/overview.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiners/remove_groups_from_examiner.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/__init__.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/overview.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_period.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_semester_manual.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/statistics/__init__.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/statistics/statistics_overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/__init__.py
--rw-r--r--   0        0        0    18351 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/create_groups.py
--rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/create_groups_accumulated_score.py
--rw-r--r--   0        0        0    19774 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/delete_groups.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/groupdetails.py
--rw-r--r--   0        0        0    11479 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/groupview_base.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/manage_deadlines.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/merge_groups.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/overview.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/replace_groups.py
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/split_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/common/__init__.py
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/common/bulkimport_users_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/__init__.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/createsubject.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/crinstance_dashboard.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/overview.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/__init__.py
--rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/assignment_list.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/filters.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/student_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/period/__init__.py
--rw-r--r--   0        0        0    11280 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/period/admins.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/period/all_results_generator.py
--rw-r--r--   0        0        0    16100 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/period/createassignment.py
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/period/crinstance_period.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/period/edit.py
--rw-r--r--   0        0        0    11244 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/period/examiners.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/period/overview.py
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/period/overview_all_results.py
--rw-r--r--   0        0        0    12995 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/period/overview_all_results_collector.py
--rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/period/students.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/period/manage_tags/__init__.py
--rw-r--r--   0        0        0    24353 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/period/manage_tags/manage_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/subject/__init__.py
--rw-r--r--   0        0        0    10432 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/subject/admins.py
--rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/subject/createperiod.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/subject/crinstance_subject.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/subject/edit.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/subject/overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/subject_for_period_admin/__init__.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/subject_for_period_admin/crinstance_subject_for_periodadmin.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/subject_for_period_admin/overview_for_periodadmin.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_admin/views/subject_for_period_admin/subject_redirect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_authenticate/__init__.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_authenticate/allauth_adapter.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_authenticate/apps.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_authenticate/socialaccount_user_updaters.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_authenticate/urls.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/login.django.html
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/logout.django.html
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_authenticate/views/__init__.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_authenticate/views/allauth_views.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_authenticate/views/custom_login_view.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_bulkcreate_users/__init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_bulkcreate_users/create_users.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_bulkcreate_users/urls.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/confirm_bulkcreated_users.django.html
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/show_bulkcreated_users.django.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/submit_bulkcreate_users.django.html
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_bulkcreate_users/views/__init__.py
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_bulkcreate_users/views/submit_bulk_users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_changelog/__init__.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_changelog/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/__init__.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/admin.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/apps.py
--rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/editor_widget.py
--rw-r--r--   0        0        0    14740 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/models.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/api/__init__.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/api/preview_markdown.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/migrations/0001_initial.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/migrations/0002_auto_20160109_1210.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/migrations/0003_auto_20160109_1239.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/migrations/0004_commentfile_created_datetime.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/migrations/0005_auto_20160122_1709.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/migrations/0006_auto_20170621_1720.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/migrations/0007_auto_20170630_0309.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/migrations/0008_commentfile_v2_id.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/migrations/0009_auto_20180509_1528.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/migrations/0010_commentedithistory.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/migrations/0011_auto_20220421_1242.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/migrations/__init__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/templates/devilry_comment/devilry_markdown_editor.django.html
--rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/tests/__init__.py
--rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/tests/test_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/views/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_comment/views/markdown_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/__init__.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/abstract_batch_action.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/admin.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/apps.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/backend_registry.py
--rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/backends/__init__.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/backends/backend_mock.py
--rw-r--r--   0        0        0    14852 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/backends/backends_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/batchjob_mixins/__init__.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/batchjob_mixins/assignment_mixin.py
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/batchjob_mixins/feedbackset_mixin.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/migrations/0001_initial.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/migrations/0002_auto_20170119_1202.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/migrations/0003_auto_20170119_1648.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/migrations/0004_auto_20170120_1733.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/migrations/0005_compressedarchivemeta_created_by.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/migrations/0006_compressedarchivemeta_created_by_role.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/migrations/0007_auto_20181002_1053.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/tests/__init__.py
--rw-r--r--   0        0        0    16151 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/tests/test_backend.py
--rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/tests/test_model.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_compressionutil/tests/test_registry.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/__init__.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_acemarkdown.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_crinstance.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_crmenu.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_css_icon_map.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/assignment.py
--rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/assignmentgroup.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/common.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_sidebar.py
--rw-r--r--   0        0        0    22529 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_timeline.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/period.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/permissiongroup.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/permissiongroupuser.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/subject.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/user.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listfilter/__init__.py
--rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listfilter/assignment.py
--rw-r--r--   0        0        0    28185 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listfilter/assignmentgroup.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listfilter/user.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listfilter/utils.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_multiselect2/__init__.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_multiselect2/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_tablebuilder/__init__.py
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_tablebuilder/base.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_tablebuilder/base_new.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/cradmin_legacy/standalone-base.django.html
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_acemarkdown.django.html
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/common/goforwardlinkitemframe.django.html
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/account-menuitem.django.html
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/breadcrumb-menuitem.django.html
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/menu.django.html
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignment/description.django.html
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/examiner-item-value.django.html
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/fully-anonymous-subjectadmin-group-item-value.django.html
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/item-value.django.html
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/minimal-item-value.django.html
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/minimal-unanonymized-selected-item.django.html
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-examiner-item-value.django.html
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-fully-anonymous-subjectadmin-group-item-value.django.html
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-item-value.django.html
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/selected-item-full.django.html
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/student-item-value.django.html
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/groupdetails.django.html
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/grouptitle.django.html
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/admin-itemvalue.django.html
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/student-itemvalue.django.html
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/permissiongroup/subjectorperiodpermissiongroup-itemvalue.django.html
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/subject/admin-itemvalue.django.html
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listfilter/utils/devilry_with_result_value_renderable.django.html
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/header_itemvalue.django.html
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/itemframe.django.html
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/itemvalue.django.html
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/row.django.html
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/table.django.html
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_cell.django.html
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_row.django.html
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_tablebuilder.django.html
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_confirmview.django.html
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_createview_with_backlink.django.html
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_updateview_with_backlink.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/__init__.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignment.py
--rw-r--r--   0        0        0    73418 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignmentgroup.py
--rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_sidebar.py
--rw-r--r--   0        0        0    14121 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_timeline.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_period.py
--rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroup.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroupuser.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listfilter/__init__.py
--rw-r--r--   0        0        0    21241 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listfilter/test_assignmentgroup_listfilter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_multiselect2/__init__.py
--rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_multiselect2/test_user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_tablebuilder/__init__.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_tablebuilder/test_table.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/viewhelpers/__init__.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_cradmin/viewhelpers/devilry_confirmview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dataporten_allauth/__init__.py
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dataporten_allauth/callback.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dataporten_allauth/models.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dataporten_allauth/provider.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dataporten_allauth/urls.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dataporten_allauth/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/__init__.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/admin.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/apps.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/bulk_create_queryset_mixin.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql.py
--rw-r--r--   0        0        0     7900 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/models.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/general_purpose_functions.sql
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/assignment/triggers.sql
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/assignment_group/triggers.sql
--rw-r--r--   0        0        0    17478 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/assignment_group_cached_data/rebuild.sql
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/candidate/triggers.sql
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/comment/triggers.sql
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/commentfile/helperfunctions.sql
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/commentfile/triggers.sql
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/examiner/triggers.sql
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/helperfunctions.sql
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/triggers.sql
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/validate.sql
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/groupcomment/triggers.sql
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/imageannotationcomment/triggers.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/devilry_dbcache_testapp/__init__.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/devilry_dbcache_testapp/models.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/migrations/0001_initial.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/migrations/0002_auto_20170108_0948.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/migrations/0003_auto_20170108_1341.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/migrations/0004_auto_20170108_1453.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/migrations/0005_auto_20170124_1504.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/tests/__init__.py
--rw-r--r--   0        0        0    76816 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_assignment_group_cached_data_triggers.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_assignment_group_triggers.py
--rw-r--r--   0        0        0    10410 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_benchmarks.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_bulk_create_queryset_mixin.py
--rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_candidate_triggers.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_comment_triggers.py
--rw-r--r--   0        0        0     7767 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_examiner_triggers.py
--rw-r--r--   0        0        0    17528 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_feedbackset_triggers.py
--rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_groupcomment_triggers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/__init__.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/cradmin_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/models.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/deadline-bulk-multiselect-filterlistview.django.html
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/manage-deadline.django.html
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline-item-value.django.html
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline.django.html
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/suggested-deadlines.django.html
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-base.django.html
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-excluded-groups-move-deadline.django.html
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-excluded-groups-new-attempt.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/tests/__init__.py
--rw-r--r--   0        0        0    33071 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/tests/test_deadline_listview.py
--rw-r--r--   0        0        0    33393 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_admin.py
--rw-r--r--   0        0        0    87456 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_examiner.py
--rw-r--r--   0        0        0    76838 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/tests/test_multiselect_groups.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/views/__init__.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/views/deadline_listview.py
--rw-r--r--   0        0        0    20342 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/views/manage_deadline_view.py
--rw-r--r--   0        0        0     8626 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/views/multiselect_groups_view.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/views/viewutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_detektor/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_detektor/models.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_detektor/migrations/0001_initial.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_detektor/migrations/0002_auto_20180119_1137.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_detektor/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_developemail/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_developemail/admin.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_developemail/email_backend.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_developemail/models.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_developemail/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_developemail/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/models.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/rq_backend.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/rq_jobs.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/comment_email/__init__.py
--rw-r--r--   0        0        0    12475 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/comment_email/comment_email.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/deadline_email/__init__.py
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/deadline_email/deadline_email.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/feedback_email/__init__.py
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/feedback_email/feedback_email.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/groupinvite_email/__init__.py
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/groupinvite_email/groupinvite_email.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/management/commands/__init__.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/management/commands/devilry_send_testemail.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/templates/devilry_email/comment_email/comment.txt
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/templates/devilry_email/deadline_email/deadline_moved.txt
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/templates/devilry_email/deadline_email/new_attempt.txt
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/templates/devilry_email/feedback_email/assignment_feedback_student.txt
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/templates/devilry_email/groupinvite_email/accepted.txt
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/templates/devilry_email/groupinvite_email/invite.txt
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/templates/devilry_email/groupinvite_email/rejected.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/templatetags/__init__.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/templatetags/comment_email_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/tests/__init__.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/tests/test_bulk_feedback.py
--rw-r--r--   0        0        0    72034 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/tests/test_comment_email.py
--rw-r--r--   0        0        0    17611 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/tests/test_deadline_email.py
--rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_email/tests/test_feedback_email.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_errortemplates/__init__.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_errortemplates/views.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_errortemplates/static/devilry_errortemplates/style.css
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_errortemplates/templates/devilry_errortemplates/404.django.html
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_errortemplates/templates/devilry_errortemplates/500.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/__init__.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/models.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tasks.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/cradminextensions/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/cradminextensions/devilry_crinstance_examiner.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/cradminextensions/devilry_crmenu_examiner.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_create_feedback.django.html
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_new_attempt.django.html
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/grouplist.django.html
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/includes/batchdownload_assignment.django.html
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/column_header_item.django.html
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/grade_cell_value.django.html
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/group_cell_value.django.html
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/simple_group_bulk_feedbackview.django.html
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/text_cell_value.django.html
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/dashboard/assignmentlist.django.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign-group-item-value.django.html
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templatetags/__init__.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/templatetags/devilry_examiner_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_assignment/__init__.py
--rw-r--r--   0        0        0    31945 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_assignment/test_batchdownload_api.py
--rw-r--r--   0        0        0    35476 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_assignment/test_batchframework_tasks.py
--rw-r--r--   0        0        0    65831 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback.py
--rw-r--r--   0        0        0    28101 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback_simple.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_assignment/test_crinstance_assignment.py
--rw-r--r--   0        0        0   126915 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_assignment/test_grouplist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_cradminextensions/__init__.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_cradminextensions/test_devilry_crmenu_examiner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_dashboard/__init__.py
--rw-r--r--   0        0        0    34779 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_dashboard/test_assignmentlist.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_dashboard/test_crinstance_dashboard.py
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_api.py
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_crinstance_selfassign.py
--rw-r--r--   0        0        0    36880 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_grouplist.py
--rw-r--r--   0        0        0    12281 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/__init__.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/crinstance_assignment.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/grouplist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/__init__.py
--rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py
--rw-r--r--   0        0        0    11506 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_manage_deadline.py
--rw-r--r--   0        0        0    11298 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_operations_grouplist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/download_files/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/download_files/backends.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/download_files/batch_download_api.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/download_files/download_archive.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/dashboard/__init__.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/dashboard/assignmentlist.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/dashboard/crinstance_dashboard.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/selfassign/__init__.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/selfassign/api.py
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/selfassign/crinstance_selfassign.py
--rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/selfassign/selfassign.py
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_examiner/views/selfassign/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/__init__.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/crinstance_frontpage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/cradminextensions/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/cradminextensions/devilry_crmenu_frontpage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/cradminextensions/listbuilder/__init__.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/cradminextensions/listbuilder/listbuilder_role.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/templates/devilry_frontpage/base.django.html
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/templates/devilry_frontpage/frontpage.django.html
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/tests/__init__.py
--rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/tests/test_frontpage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/tests/test_cradminextensions/__init__.py
--rw-r--r--   0        0        0    11517 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/tests/test_cradminextensions/test_listbuilder_role.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/views/__init__.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_frontpage/views/frontpage.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/models.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/urls.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/templates/devilry_gradeform/advanced.editable.gradeform.django.html
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/templates/devilry_gradeform/advanced.gradeform.django.html
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/templates/devilry_gradeform/base.django.html
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/templates/devilry_gradeform/create.gradeform.django.html
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/templates/devilry_gradeform/setup.gradeform.django.html
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/templatetags/__init__.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/templatetags/devilry_gradeform_tags.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/views/__init__.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/views/editable_gradeform.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/views/grade_form.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/views/points_grade_form.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/views/setup_create_gradeform.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/views/setup_gradeform.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradeform/views/viewable_gradeform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/__init__.py
--rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/models.py
--rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/pluginregistry.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/urls.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/migrations/0001_initial.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/migrations/0002_auto_20170108_0948.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/migrations/__init__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/bulkeditfeedbackbuttonbar.django.html
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/editfeedbackbuttonbar.django.html
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/editfeedbackbuttonbar_savedraftonly.django.html
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackbulkeditorbase.django.html
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_bulkpreview.django.html
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_preview.django.html
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackeditorbase.django.html
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/backandforward-bar.django.html
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/backbutton-bar.django.html
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/backward-button.django.html
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/base.django.html
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/currentprogress.django.html
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/forward-button.django.html
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/reconfigurebase.django.html
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/select_points_to_grade_mapper.django.html
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/selectplugin.django.html
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setmaxpoints.django.html
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setpassing_grade_min_points.django.html
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setup_custom_table.django.html
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/summary.django.html
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/use-this-button.django.html
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/editmarkdown.django.html
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/feedbackeditorfilewidget.django.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/__init__.py
--rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/helpers.py
--rw-r--r--   0        0        0    10027 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/test_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/__init__.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/test_download_feedbackdraftfile.py
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/test_feedbackdraft_preview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/__init__.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/base.py
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_select_points_to_grade_mapper.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_selectplugin.py
--rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_setmaxpoints.py
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_setpassing_grade_min_points.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_setup_custom_table.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_summary.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/__init__.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/download_feedbackdraftfile.py
--rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/feedbackbulkeditorbase.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/feedbackdraft_bulkpreview.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/feedbackdraft_preview.py
--rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/feedbackeditorbase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/__init__.py
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/base.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/select_points_to_grade_mapper.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/selectplugin.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/setmaxpoints.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/setpassing_grade_min_points.py
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/setup_custom_table.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/summary.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/widgets/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/widgets/editfeedbackbuttonbar.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/widgets/editmarkdown.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystem/widgets/filewidget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_approved/__init__.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_approved/apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_approved/models.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_approved/urls.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_approved/templates/devilry_gradingsystemplugin_approved/feedbackbulkeditor.django.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_approved/templates/devilry_gradingsystemplugin_approved/feedbackeditor.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_approved/views/__init__.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_approved/views/feedbackeditor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_points/__init__.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_points/apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_points/models.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_points/urls.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_points/templates/devilry_gradingsystemplugin_points/feedbackbulkeditor.django.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_points/templates/devilry_gradingsystemplugin_points/feedbackeditor.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_points/views/__init__.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_points/views/feedbackeditor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/__init__.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/admin.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/apps.py
--rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/devilry_group_baker_factories.py
--rw-r--r--   0        0        0    34983 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/models.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tasks.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/urls.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/cradmin_instances/__init__.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/cradmin_instances/crinstance_admin.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/cradmin_instances/crinstance_base.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/cradmin_instances/crinstance_examiner.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/cradmin_instances/crinstance_student.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/feedbackfeed_builder/__init__.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/feedbackfeed_builder/builder_base.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_sidebarbuilder.py
--rw-r--r--   0        0        0    10659 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_timelinebuilder.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0001_initial.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0002_feedbackset_gradeform_json.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0003_auto_20160106_1418.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0004_auto_20160107_0918.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0005_auto_20160107_0958.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0006_auto_20160107_1000.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0007_auto_20160107_1031.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0008_auto_20160107_1053.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0009_auto_20160107_1100.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0010_auto_20160107_1106.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0011_auto_20160107_1111.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0012_auto_20160107_1129.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0013_auto_20160110_1621.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0014_feedbackset_grading_status.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0015_auto_20160111_1245.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0016_auto_20160114_2202.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0017_auto_20160122_1518.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0018_auto_20160122_1712.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0019_auto_20160822_1945.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0019_auto_20160912_1649.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0020_feedbackset_ignored_datetime.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0021_merge.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0022_auto_20170103_2308.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0023_auto_20170104_0551.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0024_auto_20170107_1838.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0025_auto_20170124_1504.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0026_datamigrate_update_for_no_none_values_in_feedbackset_deadline.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0027_auto_20170206_1146.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0027_auto_20170207_1951.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0028_auto_20170208_1344.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0029_merge.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0030_auto_20170621_1734.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0031_groupcomment_v2_id.py
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0032_auto_20180214_1654.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0033_feedbacksetgradingupdatehistory.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0034_feedbackset_last_updated_by.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/0035_groupcommentedithistory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/migrations/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/base.django.html
--rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed.django.html
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_guidelines.django.html
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/group_comment_edit_base.django.html
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_base.django.html
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_discuss.django.html
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_examiner_admin_discuss.django.html
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_base.django.html
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_delete_groupcomment.html
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_discuss.django.html
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_examiner_admin_discuss.django.html
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_feedback.django.html
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/group_comment_history/comment_history.django.html
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/group_comment_history/history_item_value.django.html
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/admin_commentform_discuss_examiner_headingtext.django.html
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/admin_commentform_discuss_public_headingtext.django.html
--rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/batch_download_archive_script.django.html
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/buttonbar.django.html
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/comments_disabled.django.html
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/examiner.editlastdelivery.django.html
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/examiner_commentform_discuss_examiner_headingtext.django.html
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/examiner_commentform_discuss_public_headingtext.django.html
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/fileupload.django.html
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/groupcomment_edit_delete_option.html
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/student_commentform_headingtext.django.html
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/admin_groupcomment_item_value.django.html
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/base_event_item_value.django.html
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/base_groupcomment_item_value.django.html
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/deadline_expired_item_value.django.html
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/deadline_moved_item_value.django.html
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/examiner_groupcomment_item_value.django.html
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/feedbackset_info_item_value.django.html
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_item_value.django.html
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_updated_item_value.django.html
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/student_groupcomment_item_value.django.html
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/base_sidebar_file_item_value.django.html
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_comment_item_value.django.html
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_feedbackset_item_value.django.html
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_file_item_value.django.html
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_list.django.html
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/template_tags/devilry_group_comment_user_is_none.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templatetags/__init__.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/templatetags/devilry_group_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/__init__.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_devilry_group_mommy_factories.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_templatetags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_crinstance/__init__.py
--rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_crinstance/test_crinstance_admin.py
--rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_crinstance/test_crinstance_examiner.py
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_crinstance/test_crinstance_student.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_download/__init__.py
--rw-r--r--   0        0        0    21694 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_download/test_batchdownload_api.py
--rw-r--r--   0        0        0    10095 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_download/test_batchframework_compression.py
--rw-r--r--   0        0        0    17151 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_download/test_feedbackfeed_bulkfiledownload.py
--rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_download/test_feedbackfeed_filedownload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/admin/__init__.py
--rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/admin/test_comment_edit_history.py
--rw-r--r--   0        0        0    37226 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/admin/test_feedbackfeed_admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/__init__.py
--rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_comment_edit_history.py
--rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_delete_comment.py
--rw-r--r--   0        0        0    50866 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_discuss.py
--rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_comment.py
--rw-r--r--   0        0        0    13104 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_grade.py
--rw-r--r--   0        0        0    37037 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_feedback.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/__init__.py
--rw-r--r--   0        0        0    30200 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_admin.py
--rw-r--r--   0        0        0    25291 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_common.py
--rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_examiner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/student/__init__.py
--rw-r--r--   0        0        0    14087 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/student/test_comment_edit_history.py
--rw-r--r--   0        0        0   109725 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/student/test_feedbackfeed_student.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed_builders/__init__.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_sidebarbuilder.py
--rw-r--r--   0        0        0    21620 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_timeline_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_models/__init__.py
--rw-r--r--   0        0        0    18792 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_models/test_feedback_set.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_models/test_feedbackfeed_model.py
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_models/test_feedbackset_passed_pervious_period.py
--rw-r--r--   0        0        0    17503 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/tests/test_models/test_group_comment.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/utils/__init__.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/utils/download_response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/__init__.py
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/cradmin_comment_history.py
--rw-r--r--   0        0        0    24391 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/cradmin_feedbackfeed_base.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/group_comment_edit_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/admin/__init__.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/admin/feedbackfeed_admin.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/admin/group_comment_history.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/admin/manage_deadline.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/download_files/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/download_files/backends.py
--rw-r--r--   0        0        0    16091 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/download_files/batch_download_api.py
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/download_files/batch_download_files.py
--rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/download_files/feedbackfeed_bulkfiledownload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/examiner/__init__.py
--rw-r--r--   0        0        0    21303 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/examiner/feedbackfeed_examiner.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/examiner/group_comment_history.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/examiner/manage_deadline.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/student/__init__.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/student/feedbackfeed_student.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_group/views/student/group_comment_history.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/models.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/urls.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/templates/devilry_header/about_me.django.html
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/templates/devilry_header/app.django.html
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/templates/devilry_header/header2_extjsinclude.django.html
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/templates/devilry_header/header2include.django.html
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/templates/devilry_header/includes/change_language.django.html
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/tests/__init__.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/tests/test_aboutme.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/tests/test_change_language.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/views/__init__.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/views/about_me.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_header/views/change_language.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_help/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_help/tests.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_help/urls.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_help/views.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_help/templates/devilry_help/help.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_i18n/__init__.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_i18n/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_i18n/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/__init__.py
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporter.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/models.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/management/commands/__init__.py
--rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/management/commands/devilry_import_v2_database.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/migrations/0001_initial.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/migrations/0002_auto_20190624_1238.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/migrations/0003_auto_20210427_1350.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/migrations/__init__.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/__init__.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/assignment_importer.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/assignmentgroup_importer.py
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/candidate_examiner_importer.py
--rw-r--r--   0        0        0    13855 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/delivery_feedback_importers.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/feedbackset_importer.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/modelimporter_utils.py
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/node_importer.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/period_importer.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/pointrange_to_grade_importer.py
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/qualifiesforexam_importer.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/relateduser_importer.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/subject_importer.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/user_importer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/scripts/__init__.py
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/scripts/user_add_missing_data_from_json.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/__init__.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/importer_testcase_mixin.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentgroupimporter.py
--rw-r--r--   0        0        0    11674 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentimporter.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_candidateimporter.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_commentfilecontentimporter.py
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_deliveryimporter.py
--rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_examinerimporter.py
--rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_feedbacksetimporter.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_filemetaimporter.py
--rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_nodeimporter.py
--rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_periodimporter.py
--rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointrangetogradeimporter.py
--rw-r--r--   0        0        0     7374 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointtogrademapimporter.py
--rw-r--r--   0        0        0    14419 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_qualifiesforexam_importer.py
--rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedexaminerimporter.py
--rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedstudentimporter.py
--rw-r--r--   0        0        0    22341 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_staticfeedbackimporter.py
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_subjectimporter.py
--rw-r--r--   0        0        0     8108 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_userimporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_scripts/__init__.py
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_scripts/test_user_add_missing_data_from_json.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/__init__.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2assignment_directoryparser.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2assignmentgroup_directoryparser.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2candidate_directoryparser.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2deadline_directoryparser.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2delivery_directoryparser.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2examiner_directoryparser.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2filemeta_directoryparser.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2node_directoryparser.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2period_directoryparser.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2pointrangetograde_directoryparser.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2pointtogrademap_directoryparser.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2qualifiesforexam_finalexam_directoryparser.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2qualifiesforexam_status_directoryparser.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2relatedexaminer_directoryparser.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2relatedstudent_directoryparser.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2staticfeedback_directoryparser.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2subject_directoryparser.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2user_directoryparser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_markup/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_markup/models.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_markup/parse_markdown.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_markup/urls.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_markup/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_markup/markdown_extensions/__init__.py
--rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_markup/markdown_extensions/code_diff.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_markup/markdown_extensions/latex_math.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_markup/templates/devilry_markup/code_diff.html
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_markup/templates/devilry_markup/latex_math.html
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_markup/templates/markup/load_latex_support.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/admin.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/migrations/0001_initial.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/migrations/0002_auto_20210427_1350.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/migrations/0003_alter_message_context_type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/migrations/__init__.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/models/__init__.py
--rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/models/base.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/templates/devilry_message/for_test.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/tests/__init__.py
--rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/tests/test_message.py
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/tests/test_message_receiver.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/utils/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_message/utils/subject_generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/__init__.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/admin.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/apps.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/cradmin_app.py
--rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/models.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/pluginhelpers.py
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/plugintyperegistry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/listbuilder/__init__.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/listbuilder/assignment_listbuilder_list.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/listbuilder/plugin_listbuilder_list.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/migrations/0001_initial.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/migrations/0002_auto_20170223_1112.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/migrations/0003_auto_20170629_1914.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/migrations/0004_auto_20210427_1350.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/migrations/0005_deletedqualifiesforfinalexam.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/migrations/0006_status_plugin_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tablebuilder/__init__.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tablebuilder/tablebuilder.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/base.django.html
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/list_statuses.django.html
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/print_view.html
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/retract_status.django.html
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/selectplugin.django.html
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_preview.django.html
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_show.html
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/includes/qualification_table.django.html
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/assignment_item_value.django.html
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/description.django.html
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/plugin_item_value.django.html
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/tablebuilder/qualificationstatus_valueitem.django.html
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/tablebuilder/relatedstudent_valueitem.django.html
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/tablebuilder/tableheader_valueitem.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/__init__.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_list_statuses_view.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_models.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_plugin_listbuilder_list.py
--rw-r--r--   0        0        0    16296 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_pluginhelpers.py
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_pluginselection_view.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_plugintyperegistry.py
--rw-r--r--   0        0        0    17221 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_preview.py
--rw-r--r--   0        0        0    22999 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_showstatus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/utils/__init__.py
--rw-r--r--   0        0        0    21904 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/utils/groups_groupedby_relatedstudent_and_assignments.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/views/__init__.py
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/views/list_statuses_view.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/views/plugin_mixin.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/views/pluginselection_view.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/views/proxyview.py
--rw-r--r--   0        0        0    14987 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/views/qualification_preview_view.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/views/plugin_base_views/__init__.py
--rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/views/plugin_base_views/base_multiselect_view.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/apps.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/models.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/plugin.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/resultscollector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/tests/__init__.py
--rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/tests/test_resultscollector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/views/__init__.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/views/select_assignment.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_points/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_points/apps.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_points/models.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_points/plugin.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_points/resultscollector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_points/tests/__init__.py
--rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_points/tests/test_resultscollector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_points/views/__init__.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_points/views/select_assignment_and_points.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_students/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_students/apps.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_students/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_students/tests/__init__.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_students/tests/test_student_selection_view.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_students/views/__init__.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_students/views/select_students.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/__init__.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/abstract_generator.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/admin.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/generator_registry.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/models.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/rq_task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/urls.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/migrations/0001_initial.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/migrations/0002_auto_20210427_1350.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/migrations/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/templates/devilry_report/download_report.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/tests/__init__.py
--rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/tests/test_download_report_view.py
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/tests/test_generator_registry.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/tests/test_report_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/views/__init__.py
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_report/views/download_report.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_resetpassword/__init__.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_resetpassword/urls.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_rest/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_rest/__init__.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_rest/auth.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_rest/formfields.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_rest/models.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_rest/serializehelpers.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_rest/testclient.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_rest/tests/__init__.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_rest/tests/test_serializehelpers.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_sandbox/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_sandbox/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_sandbox/models.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_sandbox/sandbox.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_sandbox/urls.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_sandbox/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_sandbox/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_sandbox/management/commands/__init__.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_sandbox/management/commands/devilry_sandboxcreate.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_sandbox/templates/devilry_sandbox/createsubject.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_settings/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_settings/models.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_settings/urls.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_settings/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/__init__.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/api/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/api/assignment/__init__.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/api/assignment/api_utils.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/api/assignment/examiner_average_grading_points.py
--rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/api/assignment/examiner_details.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/api/assignment/examiner_group_results.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/management/commands/__init__.py
--rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/management/commands/devilry_create_test_course.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/management/commands/devilry_statistics_make_assignment_with_graded_groups.py
--rw-r--r--   0        0        0   606439 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/static/devilry_statistics/6.3.0rc1/devilry_statistics_all.js
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/.babelrc
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/.editorconfig
--rw-r--r--   0        0        0   475670 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/package-lock.json
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/package.json
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/webpack.config.js
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/devilry_statistics_all.js
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerAverageGradingPointsWidget.js
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerDetailsWidget.js
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerGroupResultWidget.js
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/registerAllWidgets.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/tests/__init__.py
--rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/tests/test_api_examiner_average_grading_points.py
--rw-r--r--   0        0        0    18649 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/tests/test_api_examiner_details.py
--rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_statistics/tests/test_api_examiner_group_result.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/__init__.py
--rw-r--r--   0        0        0     5154 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/models.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/cradminextensions/__init__.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/cradminextensions/columntypes.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/cradminextensions/devilry_crinstance_student.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/cradminextensions/devilry_crmenu_student.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/cradminextensions/studentobjecttable.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/migrations/__init__.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/add_delivery.django.html
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/contactapp/contact.django.html
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery-number-column.django.html
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery-status-column.django.html
--rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_details.django.html
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_list.django.html
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/overviewapp/overview.django.html
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_delete.django.html
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond.django.html
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond_standalone.django.html
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/projectgroup_overview.django.html
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_period/assignmentsapp/assignmentgroup-list.django.html
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_period/assignmentsapp/statuscolumn.django.html
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_student/allperiods/allperiods.django.html
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_student/recentdeliveriesapp/delivery-summary-with-assignment-column.django.html
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_student/waitingfordeliveriesapp/last-deadline.django.html
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_student/waitingfordeliveriesapp/waiting-for-deliveries-list.django.html
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/delivery-summary-column.django.html
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/naturaltime-and-datetime-column.django.html
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/naturaltime-column.django.html
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/dashboard/dashboard.django.html
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/include/feedback-rendered-view.django.html
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/include/group_breadcrumb.django.html
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/period/overview.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templatetags/__init__.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/templatetags/devilry_student_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/tests/__init__.py
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/tests/test_models.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/tests/test_templatetags.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/tests/upload_testfile1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/tests/test_cradminextensions/__init__.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/tests/test_cradminextensions/test_devilry_crmenu_student.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/tests/test_dashboard/__init__.py
--rw-r--r--   0        0        0    14380 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/tests/test_dashboard/test_allperiods.py
--rw-r--r--   0        0        0    41388 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/tests/test_dashboard/test_dashboard.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/tests/test_group/__init__.py
--rw-r--r--   0        0        0    88623 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/tests/test_group/test_projectgroupapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/tests/test_period/__init__.py
--rw-r--r--   0        0        0    28524 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/tests/test_period/test_overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/views/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/views/show_delivery.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/views/dashboard/__init__.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/views/dashboard/allperiods.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/views/dashboard/crinstance_dashboard.py
--rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/views/dashboard/dashboard.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/views/group/__init__.py
--rw-r--r--   0        0        0    14862 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/views/group/projectgroupapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/views/period/__init__.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/views/period/crinstance_period.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_student/views/period/overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/models.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tasks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/delete_periods/__init__.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/delete_periods/period_delete.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/examples/relatedexaminers.json
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/examples/relatedstudents.json
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/examples/relatedstudents_email_instead_of_username.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_anonymize_database.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_clear_allauth_account_tables.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_compressed_archives.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_inactive_users.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_message_receivers.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_messages_without_receivers.py
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_periods.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_fix_missing_first_feedbackset.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_mark_as_passed_in_previous_period.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodadd.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodadminadd.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodadminclear.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodsearch.py
--rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedexaminers.py
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedstudents.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_permissiongroup_add_subject.py
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_qualifiedforfinalexam_delete_duplicates.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_rename_periodtag_prefix.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_resend_failed_messages.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_setup_dataporten_provider.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_setup_primary_domain.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_show_assignment_guidelines.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectadd.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectadminadd.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectadminclear.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectsearch.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_test_rq_task.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_useradd.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_useraddbulk.py
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_usermerge.py
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_usermod.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/__init__.py
--rw-r--r--   0        0        0    14750 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_inactive_users.py
--rw-r--r--   0        0        0    19826 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_periods.py
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminadd.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminclear.py
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_permissiongroup_add_subject.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_qualifiedforfinalexam_delete_duplicates.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadd.py
--rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminadd.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminclear.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_useraddbulk.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_usermod.py
--rw-r--r--   0        0        0     7755 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_resend_failed_messages.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/models.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/urls.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/views.py
--rw-r--r--   0        0        0    40723 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/media/images/groovepaper.png
--rw-r--r--   0        0        0    14235 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/media/images/favicons/apple-touch-icon.png
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/media/images/favicons/favicon.ico
--rw-r--r--   0        0        0    65078 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/devilry_all.js
--rw-r--r--   0        0        0   474892 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/devilry_all.js.map
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/LICENSE
--rw-r--r--   0        0        0    23112 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/katex.min.css
--rw-r--r--   0        0        0   598523 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/katex.mjs
--rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/auto-render.js
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/auto-render.min.js
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/auto-render.mjs
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/copy-tex.css
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/copy-tex.js
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/copy-tex.min.css
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/copy-tex.min.js
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/copy-tex.mjs
--rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/mathtex-script-type.js
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/mathtex-script-type.min.js
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/mathtex-script-type.mjs
--rw-r--r--   0        0        0    79571 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/mhchem.js
--rw-r--r--   0        0        0    33776 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/mhchem.min.js
--rw-r--r--   0        0        0    75577 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/mhchem.mjs
--rw-r--r--   0        0        0    24069 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/render-a11y-string.js
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/render-a11y-string.min.js
--rw-r--r--   0        0        0    20207 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/render-a11y-string.mjs
--rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_AMS-Regular.ttf
--rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_AMS-Regular.woff
--rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_AMS-Regular.woff2
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Caligraphic-Bold.ttf
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Caligraphic-Regular.ttf
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Fraktur-Bold.ttf
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Fraktur-Regular.ttf
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Bold.ttf
--rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Bold.woff2
--rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-BoldItalic.ttf
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Italic.ttf
--rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Italic.woff2
--rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Regular.ttf
--rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Regular.woff2
--rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Math-BoldItalic.ttf
--rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Math-Italic.ttf
--rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Math-Italic.woff2
--rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Bold.ttf
--rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Italic.ttf
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Regular.ttf
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Script-Regular.ttf
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Script-Regular.woff2
--rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size1-Regular.ttf
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size1-Regular.woff2
--rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size2-Regular.ttf
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size2-Regular.woff2
--rw-r--r--   0        0        0     7588 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size3-Regular.ttf
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size3-Regular.woff2
--rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size4-Regular.ttf
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size4-Regular.woff2
--rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Typewriter-Regular.ttf
--rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Typewriter-Regular.woff2
--rw-r--r--   0        0        0    28426 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/commentEditor.js
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/cookie.js
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/examinerSelfAssignButton.js
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/feedbackfeedNavigationHandler.js
--rw-r--r--   0        0        0    20380 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/fileupload.js
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/helloWorld.js
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/latex_math.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/webcomponent_utils.js
--rw-r--r--   0        0        0   292259 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/styles/cradmin_theme_devilry_mainpages/theme.css
--rw-r--r--   0        0        0   220567 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/styles/cradmin_theme_devilry_superuserui/theme.css
--rw-r--r--   0        0        0    20335 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/vendor/fonts/glyphicons/glyphicons-halflings-regular.eot
--rw-r--r--   0        0        0    62927 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/vendor/fonts/glyphicons/glyphicons-halflings-regular.svg
--rw-r--r--   0        0        0    41280 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/vendor/fonts/glyphicons/glyphicons-halflings-regular.ttf
--rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/vendor/fonts/glyphicons/glyphicons-halflings-regular.woff
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/templates/devilry_deploy/custom_css.django.css
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/templates/devilry_deploy/custom_css_base.django.html
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/templates/devilry_deploy/footer.django.html
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/templates/devilry_deploy/footer_base.django.html
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/templates/devilry_deploy/frontpage_footer.django.html
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/templates/devilry_deploy/login_footer.django.html
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/templates/devilry_theme3/favicons.django.html
--rw-r--r--   0        0        0    25100 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/templates/devilry_theme3/wcag-debug.django.html
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/templates/devilry_theme3/include/devilry_all_js.django.html
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/templates/devilry_theme3/include/includetest.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/templatetags/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/devilry_theme3/templatetags/devilry_theme3_tags.py
--rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/django_decoupled_docs/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/django_decoupled_docs/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/django_decoupled_docs/models.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/django_decoupled_docs/registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/django_decoupled_docs/templatetags/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/django_decoupled_docs/templatetags/django_decoupled_docs_tags.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   267831 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/locale/en/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0   174762 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   374320 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/locale/nb/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/__init__.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/log.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/settingsproxy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/cradmin_legacy_settings.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/default_urls.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/devilry_test_runner.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/docproxies.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/http_error_handlers.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/i18n.py
--rw-r--r--   0        0        0     9810 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/projectspecific_settings.py
--rw-r--r--   0        0        0     8578 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/settings.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/templatecontext.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/formats/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/formats/en/__init__.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/formats/en/formats.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/formats/nb/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/formats/nb/formats.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/management/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/management/commands/__init__.py
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/common/management/commands/devilry_common_merge_candidates.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/__init__.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/dev_urls.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/fabrictasks.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/models.py
--rw-r--r--   0        0        0   353927 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/dumps/old_default.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/management/commands/__init__.py
--rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/management/commands/devilry_developer_create_deliveries_from_filesystemtree.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/management/commands/devilry_developer_delete_all_except_users.py
--rw-r--r--   0        0        0    15531 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/management/commands/devilry_developer_performance_test_db.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/management/commands/devilry_developer_set_all_passwords_to_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/settings/__init__.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/settings/base.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/settings/codeship_test.py
--rw-r--r--   0        0        0    10094 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/settings/develop.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/settings/docs.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/settings/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/testhelpers/__init__.py
--rw-r--r--   0        0        0    22236 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/testhelpers/corebuilder.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/testhelpers/datebuilder.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/testhelpers/login.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/testhelpers/skip_rq_tests.py
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/develop/testhelpers/soupselect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/production/__init__.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/production/settings.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/production/urls.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/project/production/wsgi.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/GroupAssignments.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/GroupNodes.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/OrderedDictFallback.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/__init__.py
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/anonymize_database.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/command.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/create_absolute_url.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/custom_templates.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/datetimeutils.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/delay_middleware.py
--rw-r--r--   0        0        0     8118 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/delivery_collection.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/devilry_djangoaggregate_functions.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/devilry_email.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/dictutils.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/filewrapperwithexplicitclose.py
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/groups_groupedby_relatedstudent_and_assignment.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/importutils.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/logexceptionsmiddleware.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/management.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/migrationutils.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/models.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/module.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/nodenamesuggestor.py
--rw-r--r--   0        0        0    11545 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/passed_in_previous_period.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/profile.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/rq_setup.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/setting_utils.py
--rw-r--r--   0        0        0     7675 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/stream_archives.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/verify_unique_entries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/api/__init__.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/api/api_test_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/demodb/__init__.py
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/demodb/demousers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/graphviz/__init__.py
--rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/graphviz/djangomodels.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/graphviz/dot.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/graphviz/sphinx.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/tests/__init__.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/tests/delivery_collection_tests.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/tests/importutils.py
--rwxr-xr-x   0        0        0     7534 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/tests/streamable_archive_tests.py
--rw-r--r--   0        0        0    15352 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/tests/test_anonymize_db.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/tests/test_datetimeutils.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/tests/test_groups_groupedby_relatedstudent_and_assignment.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/tests/test_nodenamesuggestor.py
--rw-r--r--   0        0        0    47879 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/tests/test_passed_in_previous_period.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/tests/test_setting_utils.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/devilry/utils/tests/test_url_datetime.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/LICENSE
--rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/README.md
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0    10910 2020-02-02 00:00:00.000000 devilry-6.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/.coveragerc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/__init__.py
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/admin.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/apps.py
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/baker_recipes.py
+-rw-r--r--   0        0        0    10440 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/deliverystore.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/devilry_core_baker_factories.py
+-rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/group_user_lookup.py
+-rw-r--r--   0        0        0    39763 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/testhelper.py
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/testhelpers.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/api/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/api/applicationstate.py
+-rw-r--r--   0        0        0    34188 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0002_auto_20150915_1127.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0003_auto_20150917_1537.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0004_examiner_relatedexaminer.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0005_relatedexaminer_automatic_anonymous_id.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0006_auto_20151112_1851.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0007_assignment_gradeform_setup_json.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0008_auto_20151222_1955.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0009_assignmentgroup_batchoperation.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0010_assignment_anonymizationmode.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0011_datamigrate_anonymous_to_anonymizationmode.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0012_auto_20160111_2019.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0013_auto_20160111_2021.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0014_auto_20160112_1052.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0015_assignment_uses_custom_candidate_ids.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0016_auto_20160112_1831.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0017_candidate_relatedstudent_replaces_student_field.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0018_auto_20160112_1923.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0019_auto_20160113_2037.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0020_relatedexaminer_active.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0021_examiner_relatedexaminer_replaces_user_field.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0022_auto_20160114_1520.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0023_auto_20160114_1522.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0024_auto_20160114_1524.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0025_auto_20160114_1525.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0026_auto_20160114_1528.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0027_auto_20160116_1843.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0028_auto_20160119_0337.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0029_assignmentgrouphistory.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0030_auto_20170124_1504.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0031_auto_20170125_1601.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0032_datamigrate_update_for_no_none_values_in_assignment_firstdeadline.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0033_auto_20170220_1330.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0034_auto_20170303_1308.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0035_auto_20170523_1747.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0036_auto_20170523_1748.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0037_auto_20170620_1515.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0038_auto_20170621_1720.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0039_assignmentgroup_internal_is_being_deleted.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0040_auto_20180214_1654.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0041_auto_20180220_0651.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0042_candidateassignmentgrouphistory_examinerassignmentgrouphistory.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0043_auto_20180302_1139.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0044_auto_20190624_1238.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0045_auto_20210427_1350.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/0046_auto_20220519_1043.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/migrations/__init__.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/__init__.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/abstract_applicationkeyvalue.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/abstract_is_admin.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/abstract_is_candidate.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/abstract_is_examiner.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/administrators.py
+-rw-r--r--   0        0        0    50913 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/assignment.py
+-rw-r--r--   0        0        0    76482 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/assignment_group.py
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/assignment_group_history.py
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/basenode.py
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/candidate.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/custom_db_fields.py
+-rw-r--r--   0        0        0    16062 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/deadline.py
+-rw-r--r--   0        0        0    13166 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/delivery.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/deliverytypes.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/devilryuserprofile.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/examiner.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/examiner_candidate_group_history.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/filemeta.py
+-rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/groupinvite.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/model_utils.py
+-rw-r--r--   0        0        0    10652 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/period.py
+-rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/period_tag.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/pointrange_to_grade.py
+-rw-r--r--   0        0        0    19027 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/relateduser.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/save_interface.py
+-rw-r--r--   0        0        0    10883 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/static_feedback.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/models/subject.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/comment-summary.django.html
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-base-plain.django.html
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-base.django.html
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-full-plain.django.html
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-full.django.html
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-short.django.html
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/groupstatus.django.html
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/multiple-candidates-long-displayname.django.html
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/multiple-candidates-short-displayname.django.html
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/multiple-examiners-long-displayname.django.html
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/multiple-examiners-short-displayname.django.html
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/period-tags-on-period.django.html
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/relatedexaminers-on-period-tag.django.html
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/relatedstudents-on-period-tag.django.html
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/relatedusers-on-period-tag.django.html
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/single-candidate-long-displayname.django.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/single-candidate-short-displayname.django.html
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/single-examiner-long-displayname-plain.django.html
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/single-examiner-long-displayname.django.html
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/single-examiner-short-displayname.django.html
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/search/indexes/core/assignment_text.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/search/indexes/core/assignmentgroup_candidates.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/search/indexes/core/assignmentgroup_examiners.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/search/indexes/core/assignmentgroup_tags.txt
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/search/indexes/core/assignmentgroup_text.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/search/indexes/core/basenode_text.txt
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/search/indexes/core/format_user.django.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/search/indexes/core/node_text.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/search/indexes/core/period_text.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templates/search/indexes/core/subject_text.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templatetags/__init__.py
+-rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/templatetags/devilry_core_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/__init__.py
+-rw-r--r--   0        0        0    79383 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_assignment.py
+-rw-r--r--   0        0        0   180651 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_assignment_group.py
+-rw-r--r--   0        0        0     8857 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_assignment_group_history.py
+-rw-r--r--   0        0        0     8276 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_candidate.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_deadline.py
+-rw-r--r--   0        0        0    78327 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_devilry_core_tags.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_examiner.py
+-rw-r--r--   0        0        0    30450 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_group_user_lookup.py
+-rw-r--r--   0        0        0    28214 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_groupinvite.py
+-rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_period.py
+-rw-r--r--   0        0        0    12030 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_period_tags.py
+-rw-r--r--   0        0        0    19992 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_pointrange_to_grade.py
+-rw-r--r--   0        0        0    38546 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_relateduser.py
+-rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/tests/test_subject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/views/__init__.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/apps/core/views/download_staticfeedbackfileattachment.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/coreutils/__init__.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/coreutils/utils.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/defaults/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/defaults/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/__init__.py
+-rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/admin.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/apps.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/baker_recipes.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/crinstance_account.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/exceptions.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/middleware.py
+-rw-r--r--   0        0        0    52183 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/models.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/urls.py
+-rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/user_merger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/authbackend/__init__.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/authbackend/default.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/authbackend/ldap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/cradminextensions/__init__.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/cradminextensions/devilry_crmenu_account.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/crapps/__init__.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/crapps/account/__init__.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/crapps/account/index.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/crapps/account/select_language.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/crapps/account/utils.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/migrations/0001_initial.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/migrations/0002_auto_20150917_1731.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/migrations/0003_datamigrate-admins-into-permissiongroups.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/migrations/0004_auto_20151222_1955.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/migrations/0005_auto_20160113_2037.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/migrations/0006_auto_20160120_0424.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/migrations/0007_auto_20210427_1350.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/migrations/0008_auto_20220510_1307.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/migrations/0009_mergeduser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/migrations/__init__.py
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/templates/devilry_account/crapps/account/select_language.django.html
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/templates/devilry_account/templatetags/multiple-users-verbose-inline.django.html
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/templates/devilry_account/templatetags/user-verbose-inline-plain.django.html
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/templates/devilry_account/templatetags/user-verbose-inline.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/templatetags/__init__.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/templatetags/devilry_account_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/tests/__init__.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/tests/test_devilry_account_tags.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/tests/test_middleware.py
+-rw-r--r--   0        0        0    46608 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/tests/test_models.py
+-rw-r--r--   0        0        0    16979 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/tests/test_user_merger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/tests/authbackend/__init__.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/tests/authbackend/test_default.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/tests/test_crapps/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/tests/test_crapps/test_account/__init__.py
+-rw-r--r--   0        0        0    18890 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/tests/test_crapps/test_account/test_index.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_account/tests/test_crapps/test_account/test_select_language.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/__init__.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/models.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tasks.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/__init__.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/devilry_crinstance_admin.py
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/devilry_crmenu_admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_assignmentgroup.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedexaminer.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedstudent.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listfilter/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listfilter/listfilter_assignmentgroup.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listfilter/listfilter_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/multiselect2/__init__.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/multiselect2/multiselect2_relatedstudent.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/listbuilder/__init__.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/listbuilder/admindashboard_subject_listbuilder.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/overview.django.html
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/add_groups_to_examiner.django.html
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/examinerdetails.django.html
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/overview.django.html
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/remove_groups_from_examiner.django.html
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-add.django.html
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-replace.django.html
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag-item-value.django.html
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag.django.html
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/random.django.html
+-rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/select_method.django.html
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/custom-table.django.html
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/gradingconfiguration-update.django.html
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/examiners.django.html
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/gradingconfiguration.django.html
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/published.django.html
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/settings.django.html
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/statistics.django.html
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/students.django.html
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/utilities.django.html
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/includes/batchdownload_assignment.django.html
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-item-value.django.html
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-overview.django.html
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/candidate-item-value.django.html
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/confirm-view.django.html
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/overview.django.html
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select-period-view.django.html
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select_groups_to_pass.django.html
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/statistics/overview.django.html
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups.django.html
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/merge_groups.django.html
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/overview.django.html
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/split_groups.django.html
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-accumulated-score.django.html
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-assignment-item-value.django.html
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-method.django.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-period-item-value.django.html
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/confirm.django.html
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/manual-select-students.django.html
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/preview-relatedstudent-item-value.django.html
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/preview.django.html
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/select-assignments.django.html
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/selectable-assignment-item-value.django.html
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/selected-assignment-item-value.django.html
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/includes/select-assignment-item-value-description.django.html
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-assignment-item-value.django.html
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-method.django.html
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-period-item-value.django.html
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/confirm.django.html
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupdetails/details-renderable.django.html
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupdetails/view.django.html
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupview_base/base-info-view.django.html
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupview_base/base-multiselect-view.django.html
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupview_base/include/no-items-message.django.html
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/common/abstract-type-in-users.django.html
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/common/admin-list-view.django.html
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/common/admins-explained.django.html
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/overview.django.html
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/group_by_assignment.django.html
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_groups.django.html
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_users.django.html
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/listbuilder/admindashboard_subject_listbuilder/value.django.html
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/listbuilder/assignmentgroup_listbuilder/value.django.html
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/listbuilder/listbuilder_relatedexaminer/onassignment-itemvalue.django.html
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/listbuilder/listbuilder_relatedstudent/readonly-itemvalue.django.html
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/multiselect2/multiselect2_relatedstudent/itemvalue.django.html
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/multiselect2/multiselect2_relatedstudent/selecteditem.django.html
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/overview.django.html
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/admins/add.django.html
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/admins/overview-itemvalue.django.html
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/admins/overview.django.html
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/column_header_item.django.html
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/devilry_admin_all_results_overview_table.django.html
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/devilry_all_results_overview.django.html
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/result_cell_value.django.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/student_cell_value.django.html
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/createassignment.django.html
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/helpbox.django.html
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/success_message.django.html
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/suggested_deadlines.django.html
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/edit/updateview.django.html
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/examiners/add.django.html
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview-itemvalue.django.html
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview.django.html
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/add-tag.django.html
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/base-multiselect-view.django.html
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/crud.django.html
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/delete.django.html
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/manage-tags-list-view.django.html
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/tag-item-value.django.html
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/relatedusers/select-method.django.html
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/qualifiedforfinalexams/statuslistview-info-column.django.html
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/qualifiedforfinalexams/userlistview-info-column.django.html
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/add.django.html
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/overview-itemvalue.django.html
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/overview.django.html
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/students-not-added-to-assignments-warning.django.html
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/userselectview-no-searchresults-message.django.html
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/overview.django.html
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/overview_for_period_admins.html
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/admins/add.django.html
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview-itemvalue.django.html
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview.django.html
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/edit/updateview.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/__init__.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_anonymizationmode.py
+-rw-r--r--   0        0        0    44944 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_batchframework_tasks.py
+-rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_crinstance_assignment.py
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_deadline_handling.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_examiner_selfassign.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_examiner_statistics.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_first_deadline.py
+-rw-r--r--   0        0        0    12214 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_grading_configuration.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_long_and_shortname.py
+-rw-r--r--   0        0        0    48383 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_overview.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_projectgroups.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_publishing_time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/examiners/__init__.py
+-rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_add_groups_to_examiner.py
+-rw-r--r--   0        0        0    63295 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_bulk_organize.py
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_examinerdetails.py
+-rw-r--r--   0        0        0    12880 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_overview.py
+-rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_remove_groups_from_examiner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/__init__.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_overview.py
+-rw-r--r--   0        0        0    51914 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period.py
+-rw-r--r--   0        0        0    10256 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period_manual.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/__init__.py
+-rw-r--r--   0        0        0    44849 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_create_groups.py
+-rw-r--r--   0        0        0    45703 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_create_groups_accumulated_score.py
+-rw-r--r--   0        0        0    46531 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_delete_groups.py
+-rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupdetails.py
+-rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_merge_groups.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_overview.py
+-rw-r--r--   0        0        0    50909 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_replace_groups.py
+-rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_split_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/__init__.py
+-rw-r--r--   0        0        0    19748 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_baseinforview.py
+-rw-r--r--   0        0        0    19777 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_basemultiselectview.py
+-rw-r--r--   0        0        0    77200 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_groupviewmixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_download_files/__init__.py
+-rw-r--r--   0        0        0    33016 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_download_files/test_batchdownload_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/common/__init__.py
+-rw-r--r--   0        0        0    16683 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/common/admins_common_testmixins.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/common/test_bulkimport_users_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/cradminextensions/__init__.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/cradminextensions/test_devilry_crmenu_admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/__init__.py
+-rw-r--r--   0        0        0     8928 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedexaminer.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedstudent.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/cradminextensions/test_multiselect2/__init__.py
+-rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/cradminextensions/test_multiselect2/test_multiselect2_relatedstudent.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/dashboard/__init__.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/dashboard/test_createsubject.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/dashboard/test_crinstance_dashboard.py
+-rw-r--r--   0        0        0    18818 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/dashboard/test_overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/__init__.py
+-rw-r--r--   0        0        0    29261 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_assignment_listview.py
+-rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_student_listview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/__init__.py
+-rw-r--r--   0        0        0    29781 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_admins.py
+-rw-r--r--   0        0        0    40873 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_createassignment.py
+-rw-r--r--   0        0        0    15268 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_crinstance_period.py
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_edit.py
+-rw-r--r--   0        0        0    34091 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_examiners.py
+-rw-r--r--   0        0        0    19450 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_overview.py
+-rw-r--r--   0        0        0    10863 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_overview_all_results.py
+-rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_period_all_results_collector.py
+-rw-r--r--   0        0        0    34017 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_students.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_manage_tags/__init__.py
+-rw-r--r--   0        0        0    51030 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags.py
+-rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags_relatedusers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_report/__init__.py
+-rw-r--r--   0        0        0    42098 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_report/test_all_results_generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/subject/__init__.py
+-rw-r--r--   0        0        0    26747 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/subject/test_admins.py
+-rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/subject/test_createperiod.py
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/subject/test_crinstance_subject.py
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/subject/test_edit.py
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/subject/test_overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/__init__.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/test_crinstance_for_periodadmin.py
+-rw-r--r--   0        0        0    11399 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/test_overview_for_periodadmin.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/test_subject_redirect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/__init__.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/anonymizationmode.py
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/crinstance_assignment.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/deadline_handling.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiner_selfassign.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/first_deadline.py
+-rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/gradingconfiguration.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/long_and_shortname.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/overview.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/projectgroups.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/publishing_time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/download_files/__init__.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/download_files/backends.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/download_files/batch_download_api.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/download_files/download_archive.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiners/__init__.py
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiners/add_groups_to_examiner.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiners/base_single_examinerview.py
+-rw-r--r--   0        0        0    24438 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiners/bulk_organize.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiners/examinerdetails.py
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiners/overview.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiners/remove_groups_from_examiner.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/__init__.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/overview.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_period.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_semester_manual.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/statistics/__init__.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/statistics/statistics_overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/__init__.py
+-rw-r--r--   0        0        0    18351 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/create_groups.py
+-rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/create_groups_accumulated_score.py
+-rw-r--r--   0        0        0    19774 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/delete_groups.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/groupdetails.py
+-rw-r--r--   0        0        0    11479 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/groupview_base.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/manage_deadlines.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/merge_groups.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/overview.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/replace_groups.py
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/split_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/common/__init__.py
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/common/bulkimport_users_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/__init__.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/createsubject.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/crinstance_dashboard.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/overview.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/__init__.py
+-rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/assignment_list.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/filters.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/student_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/period/__init__.py
+-rw-r--r--   0        0        0    11280 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/period/admins.py
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/period/all_results_generator.py
+-rw-r--r--   0        0        0    16100 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/period/createassignment.py
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/period/crinstance_period.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/period/edit.py
+-rw-r--r--   0        0        0    11244 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/period/examiners.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/period/overview.py
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/period/overview_all_results.py
+-rw-r--r--   0        0        0    12995 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/period/overview_all_results_collector.py
+-rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/period/students.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/period/manage_tags/__init__.py
+-rw-r--r--   0        0        0    24353 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/period/manage_tags/manage_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/subject/__init__.py
+-rw-r--r--   0        0        0    10432 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/subject/admins.py
+-rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/subject/createperiod.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/subject/crinstance_subject.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/subject/edit.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/subject/overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/subject_for_period_admin/__init__.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/subject_for_period_admin/crinstance_subject_for_periodadmin.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/subject_for_period_admin/overview_for_periodadmin.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_admin/views/subject_for_period_admin/subject_redirect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_authenticate/__init__.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_authenticate/allauth_adapter.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_authenticate/apps.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_authenticate/socialaccount_user_updaters.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_authenticate/urls.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/login.django.html
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/logout.django.html
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_authenticate/views/__init__.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_authenticate/views/allauth_views.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_authenticate/views/custom_login_view.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_bulkcreate_users/__init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_bulkcreate_users/create_users.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_bulkcreate_users/urls.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/confirm_bulkcreated_users.django.html
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/show_bulkcreated_users.django.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/submit_bulkcreate_users.django.html
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_bulkcreate_users/views/__init__.py
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_bulkcreate_users/views/submit_bulk_users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_changelog/__init__.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_changelog/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/__init__.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/admin.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/apps.py
+-rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/editor_widget.py
+-rw-r--r--   0        0        0    14740 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/models.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/api/__init__.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/api/preview_markdown.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/migrations/0001_initial.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/migrations/0002_auto_20160109_1210.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/migrations/0003_auto_20160109_1239.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/migrations/0004_commentfile_created_datetime.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/migrations/0005_auto_20160122_1709.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/migrations/0006_auto_20170621_1720.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/migrations/0007_auto_20170630_0309.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/migrations/0008_commentfile_v2_id.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/migrations/0009_auto_20180509_1528.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/migrations/0010_commentedithistory.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/migrations/0011_auto_20220421_1242.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/migrations/__init__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/templates/devilry_comment/devilry_markdown_editor.django.html
+-rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/tests/__init__.py
+-rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/tests/test_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/views/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_comment/views/markdown_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/__init__.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/abstract_batch_action.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/admin.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/apps.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/backend_registry.py
+-rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/backends/__init__.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/backends/backend_mock.py
+-rw-r--r--   0        0        0    14916 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/backends/backends_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/batchjob_mixins/__init__.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/batchjob_mixins/assignment_mixin.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/batchjob_mixins/feedbackset_mixin.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/migrations/0001_initial.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/migrations/0002_auto_20170119_1202.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/migrations/0003_auto_20170119_1648.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/migrations/0004_auto_20170120_1733.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/migrations/0005_compressedarchivemeta_created_by.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/migrations/0006_compressedarchivemeta_created_by_role.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/migrations/0007_auto_20181002_1053.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/tests/__init__.py
+-rw-r--r--   0        0        0    16151 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/tests/test_backend.py
+-rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/tests/test_model.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_compressionutil/tests/test_registry.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/__init__.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_acemarkdown.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_crinstance.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_crmenu.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_css_icon_map.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/assignment.py
+-rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/assignmentgroup.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/common.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_sidebar.py
+-rw-r--r--   0        0        0    22529 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_timeline.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/period.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/permissiongroup.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/permissiongroupuser.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/subject.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/user.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listfilter/__init__.py
+-rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listfilter/assignment.py
+-rw-r--r--   0        0        0    28185 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listfilter/assignmentgroup.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listfilter/user.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listfilter/utils.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_multiselect2/__init__.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_multiselect2/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_tablebuilder/__init__.py
+-rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_tablebuilder/base.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_tablebuilder/base_new.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/cradmin_legacy/standalone-base.django.html
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_acemarkdown.django.html
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/common/goforwardlinkitemframe.django.html
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/account-menuitem.django.html
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/breadcrumb-menuitem.django.html
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/menu.django.html
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignment/description.django.html
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/examiner-item-value.django.html
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/fully-anonymous-subjectadmin-group-item-value.django.html
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/item-value.django.html
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/minimal-item-value.django.html
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/minimal-unanonymized-selected-item.django.html
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-examiner-item-value.django.html
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-fully-anonymous-subjectadmin-group-item-value.django.html
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-item-value.django.html
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/selected-item-full.django.html
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/student-item-value.django.html
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/groupdetails.django.html
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/grouptitle.django.html
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/admin-itemvalue.django.html
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/student-itemvalue.django.html
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/permissiongroup/subjectorperiodpermissiongroup-itemvalue.django.html
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/subject/admin-itemvalue.django.html
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listfilter/utils/devilry_with_result_value_renderable.django.html
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/header_itemvalue.django.html
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/itemframe.django.html
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/itemvalue.django.html
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/row.django.html
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/table.django.html
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_cell.django.html
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_row.django.html
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_tablebuilder.django.html
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_confirmview.django.html
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_createview_with_backlink.django.html
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_updateview_with_backlink.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/__init__.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignment.py
+-rw-r--r--   0        0        0    73418 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignmentgroup.py
+-rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_sidebar.py
+-rw-r--r--   0        0        0    14121 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_timeline.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_period.py
+-rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroup.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroupuser.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listfilter/__init__.py
+-rw-r--r--   0        0        0    21241 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listfilter/test_assignmentgroup_listfilter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_multiselect2/__init__.py
+-rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_multiselect2/test_user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_tablebuilder/__init__.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_tablebuilder/test_table.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/viewhelpers/__init__.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_cradmin/viewhelpers/devilry_confirmview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dataporten_allauth/__init__.py
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dataporten_allauth/callback.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dataporten_allauth/models.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dataporten_allauth/provider.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dataporten_allauth/urls.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dataporten_allauth/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/__init__.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/admin.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/apps.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/bulk_create_queryset_mixin.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql.py
+-rw-r--r--   0        0        0     7900 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/models.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/general_purpose_functions.sql
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/assignment/triggers.sql
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/assignment_group/triggers.sql
+-rw-r--r--   0        0        0    17478 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/assignment_group_cached_data/rebuild.sql
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/candidate/triggers.sql
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/comment/triggers.sql
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/commentfile/helperfunctions.sql
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/commentfile/triggers.sql
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/examiner/triggers.sql
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/helperfunctions.sql
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/triggers.sql
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/validate.sql
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/groupcomment/triggers.sql
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/imageannotationcomment/triggers.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/devilry_dbcache_testapp/__init__.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/devilry_dbcache_testapp/models.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/migrations/0002_auto_20170108_0948.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/migrations/0003_auto_20170108_1341.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/migrations/0004_auto_20170108_1453.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/migrations/0005_auto_20170124_1504.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/tests/__init__.py
+-rw-r--r--   0        0        0    76816 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_assignment_group_cached_data_triggers.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_assignment_group_triggers.py
+-rw-r--r--   0        0        0    10410 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_bulk_create_queryset_mixin.py
+-rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_candidate_triggers.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_comment_triggers.py
+-rw-r--r--   0        0        0     7767 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_examiner_triggers.py
+-rw-r--r--   0        0        0    17528 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_feedbackset_triggers.py
+-rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_groupcomment_triggers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/__init__.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/cradmin_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/models.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/deadline-bulk-multiselect-filterlistview.django.html
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/manage-deadline.django.html
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline-item-value.django.html
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline.django.html
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/suggested-deadlines.django.html
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-base.django.html
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-excluded-groups-move-deadline.django.html
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-excluded-groups-new-attempt.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/tests/__init__.py
+-rw-r--r--   0        0        0    33071 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/tests/test_deadline_listview.py
+-rw-r--r--   0        0        0    33393 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_admin.py
+-rw-r--r--   0        0        0    87456 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_examiner.py
+-rw-r--r--   0        0        0    76838 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/tests/test_multiselect_groups.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/views/__init__.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/views/deadline_listview.py
+-rw-r--r--   0        0        0    20342 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/views/manage_deadline_view.py
+-rw-r--r--   0        0        0     8626 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/views/multiselect_groups_view.py
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/views/viewutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_detektor/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_detektor/models.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_detektor/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_detektor/migrations/0002_auto_20180119_1137.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_detektor/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_developemail/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_developemail/admin.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_developemail/email_backend.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_developemail/models.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_developemail/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_developemail/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/models.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/rq_backend.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/rq_jobs.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/comment_email/__init__.py
+-rw-r--r--   0        0        0    12475 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/comment_email/comment_email.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/deadline_email/__init__.py
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/deadline_email/deadline_email.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/feedback_email/__init__.py
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/feedback_email/feedback_email.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/groupinvite_email/__init__.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/groupinvite_email/groupinvite_email.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/management/commands/__init__.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/management/commands/devilry_send_testemail.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/templates/devilry_email/comment_email/comment.txt
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/templates/devilry_email/deadline_email/deadline_moved.txt
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/templates/devilry_email/deadline_email/new_attempt.txt
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/templates/devilry_email/feedback_email/assignment_feedback_student.txt
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/templates/devilry_email/groupinvite_email/accepted.txt
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/templates/devilry_email/groupinvite_email/invite.txt
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/templates/devilry_email/groupinvite_email/rejected.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/templatetags/__init__.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/templatetags/comment_email_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/tests/__init__.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/tests/test_bulk_feedback.py
+-rw-r--r--   0        0        0    72034 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/tests/test_comment_email.py
+-rw-r--r--   0        0        0    17611 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/tests/test_deadline_email.py
+-rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_email/tests/test_feedback_email.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_errortemplates/__init__.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_errortemplates/views.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_errortemplates/static/devilry_errortemplates/style.css
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_errortemplates/templates/devilry_errortemplates/404.django.html
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_errortemplates/templates/devilry_errortemplates/500.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/__init__.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/models.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tasks.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/cradminextensions/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/cradminextensions/devilry_crinstance_examiner.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/cradminextensions/devilry_crmenu_examiner.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_create_feedback.django.html
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_new_attempt.django.html
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/grouplist.django.html
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/includes/batchdownload_assignment.django.html
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/column_header_item.django.html
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/grade_cell_value.django.html
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/group_cell_value.django.html
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/simple_group_bulk_feedbackview.django.html
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/text_cell_value.django.html
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/dashboard/assignmentlist.django.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign-group-item-value.django.html
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templatetags/__init__.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/templatetags/devilry_examiner_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_assignment/__init__.py
+-rw-r--r--   0        0        0    31945 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_assignment/test_batchdownload_api.py
+-rw-r--r--   0        0        0    35476 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_assignment/test_batchframework_tasks.py
+-rw-r--r--   0        0        0    65831 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback.py
+-rw-r--r--   0        0        0    28101 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback_simple.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_assignment/test_crinstance_assignment.py
+-rw-r--r--   0        0        0   126915 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_assignment/test_grouplist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_cradminextensions/__init__.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_cradminextensions/test_devilry_crmenu_examiner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_dashboard/__init__.py
+-rw-r--r--   0        0        0    34779 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_dashboard/test_assignmentlist.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_dashboard/test_crinstance_dashboard.py
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_api.py
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_crinstance_selfassign.py
+-rw-r--r--   0        0        0    36880 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_grouplist.py
+-rw-r--r--   0        0        0    12281 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/__init__.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/crinstance_assignment.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/grouplist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/__init__.py
+-rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py
+-rw-r--r--   0        0        0    11506 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_manage_deadline.py
+-rw-r--r--   0        0        0    11298 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_operations_grouplist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/download_files/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/download_files/backends.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/download_files/batch_download_api.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/download_files/download_archive.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/dashboard/__init__.py
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/dashboard/assignmentlist.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/dashboard/crinstance_dashboard.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/selfassign/__init__.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/selfassign/api.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/selfassign/crinstance_selfassign.py
+-rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/selfassign/selfassign.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_examiner/views/selfassign/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/__init__.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/crinstance_frontpage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/cradminextensions/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/cradminextensions/devilry_crmenu_frontpage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/cradminextensions/listbuilder/__init__.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/cradminextensions/listbuilder/listbuilder_role.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/templates/devilry_frontpage/base.django.html
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/templates/devilry_frontpage/frontpage.django.html
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/tests/__init__.py
+-rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/tests/test_frontpage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/tests/test_cradminextensions/__init__.py
+-rw-r--r--   0        0        0    11517 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/tests/test_cradminextensions/test_listbuilder_role.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/views/__init__.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_frontpage/views/frontpage.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/models.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/urls.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/templates/devilry_gradeform/advanced.editable.gradeform.django.html
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/templates/devilry_gradeform/advanced.gradeform.django.html
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/templates/devilry_gradeform/base.django.html
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/templates/devilry_gradeform/create.gradeform.django.html
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/templates/devilry_gradeform/setup.gradeform.django.html
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/templatetags/__init__.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/templatetags/devilry_gradeform_tags.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/views/__init__.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/views/editable_gradeform.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/views/grade_form.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/views/points_grade_form.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/views/setup_create_gradeform.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/views/setup_gradeform.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradeform/views/viewable_gradeform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/__init__.py
+-rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/models.py
+-rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/pluginregistry.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/urls.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/migrations/0001_initial.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/migrations/0002_auto_20170108_0948.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/migrations/__init__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/bulkeditfeedbackbuttonbar.django.html
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/editfeedbackbuttonbar.django.html
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/editfeedbackbuttonbar_savedraftonly.django.html
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackbulkeditorbase.django.html
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_bulkpreview.django.html
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_preview.django.html
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackeditorbase.django.html
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/backandforward-bar.django.html
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/backbutton-bar.django.html
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/backward-button.django.html
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/base.django.html
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/currentprogress.django.html
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/forward-button.django.html
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/reconfigurebase.django.html
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/select_points_to_grade_mapper.django.html
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/selectplugin.django.html
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setmaxpoints.django.html
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setpassing_grade_min_points.django.html
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setup_custom_table.django.html
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/summary.django.html
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/use-this-button.django.html
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/editmarkdown.django.html
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/feedbackeditorfilewidget.django.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/__init__.py
+-rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/helpers.py
+-rw-r--r--   0        0        0    10027 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/test_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/__init__.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/test_download_feedbackdraftfile.py
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/test_feedbackdraft_preview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/__init__.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/base.py
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_select_points_to_grade_mapper.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_selectplugin.py
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_setmaxpoints.py
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_setpassing_grade_min_points.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_setup_custom_table.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_summary.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/__init__.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/download_feedbackdraftfile.py
+-rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/feedbackbulkeditorbase.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/feedbackdraft_bulkpreview.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/feedbackdraft_preview.py
+-rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/feedbackeditorbase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/__init__.py
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/base.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/select_points_to_grade_mapper.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/selectplugin.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/setmaxpoints.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/setpassing_grade_min_points.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/setup_custom_table.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/summary.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/widgets/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/widgets/editfeedbackbuttonbar.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/widgets/editmarkdown.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystem/widgets/filewidget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_approved/__init__.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_approved/apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_approved/models.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_approved/urls.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_approved/templates/devilry_gradingsystemplugin_approved/feedbackbulkeditor.django.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_approved/templates/devilry_gradingsystemplugin_approved/feedbackeditor.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_approved/views/__init__.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_approved/views/feedbackeditor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_points/__init__.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_points/apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_points/models.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_points/urls.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_points/templates/devilry_gradingsystemplugin_points/feedbackbulkeditor.django.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_points/templates/devilry_gradingsystemplugin_points/feedbackeditor.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_points/views/__init__.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_points/views/feedbackeditor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/__init__.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/admin.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/apps.py
+-rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/devilry_group_baker_factories.py
+-rw-r--r--   0        0        0    34983 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/models.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tasks.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/urls.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/cradmin_instances/__init__.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/cradmin_instances/crinstance_admin.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/cradmin_instances/crinstance_base.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/cradmin_instances/crinstance_examiner.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/cradmin_instances/crinstance_student.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/feedbackfeed_builder/__init__.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/feedbackfeed_builder/builder_base.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_sidebarbuilder.py
+-rw-r--r--   0        0        0    10659 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_timelinebuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/management/commands/__init__.py
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/management/commands/mock_data.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0001_initial.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0002_feedbackset_gradeform_json.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0003_auto_20160106_1418.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0004_auto_20160107_0918.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0005_auto_20160107_0958.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0006_auto_20160107_1000.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0007_auto_20160107_1031.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0008_auto_20160107_1053.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0009_auto_20160107_1100.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0010_auto_20160107_1106.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0011_auto_20160107_1111.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0012_auto_20160107_1129.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0013_auto_20160110_1621.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0014_feedbackset_grading_status.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0015_auto_20160111_1245.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0016_auto_20160114_2202.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0017_auto_20160122_1518.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0018_auto_20160122_1712.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0019_auto_20160822_1945.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0019_auto_20160912_1649.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0020_feedbackset_ignored_datetime.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0021_merge.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0022_auto_20170103_2308.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0023_auto_20170104_0551.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0024_auto_20170107_1838.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0025_auto_20170124_1504.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0026_datamigrate_update_for_no_none_values_in_feedbackset_deadline.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0027_auto_20170206_1146.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0027_auto_20170207_1951.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0028_auto_20170208_1344.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0029_merge.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0030_auto_20170621_1734.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0031_groupcomment_v2_id.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0032_auto_20180214_1654.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0033_feedbacksetgradingupdatehistory.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0034_feedbackset_last_updated_by.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/0035_groupcommentedithistory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/migrations/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/base.django.html
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed.django.html
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_guidelines.django.html
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/group_comment_edit_base.django.html
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_base.django.html
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_discuss.django.html
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_examiner_admin_discuss.django.html
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_base.django.html
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_delete_groupcomment.html
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_discuss.django.html
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_examiner_admin_discuss.django.html
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_feedback.django.html
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/group_comment_history/comment_history.django.html
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/group_comment_history/history_item_value.django.html
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/admin_commentform_discuss_examiner_headingtext.django.html
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/admin_commentform_discuss_public_headingtext.django.html
+-rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/batch_download_archive_script.django.html
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/buttonbar.django.html
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/comments_disabled.django.html
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/examiner.editlastdelivery.django.html
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/examiner_commentform_discuss_examiner_headingtext.django.html
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/examiner_commentform_discuss_public_headingtext.django.html
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/fileupload.django.html
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/groupcomment_edit_delete_option.html
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/student_commentform_headingtext.django.html
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/admin_groupcomment_item_value.django.html
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/base_event_item_value.django.html
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/base_groupcomment_item_value.django.html
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/deadline_expired_item_value.django.html
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/deadline_moved_item_value.django.html
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/examiner_groupcomment_item_value.django.html
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/feedbackset_info_item_value.django.html
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_item_value.django.html
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_updated_item_value.django.html
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/student_groupcomment_item_value.django.html
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/base_sidebar_file_item_value.django.html
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_comment_item_value.django.html
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_feedbackset_item_value.django.html
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_file_item_value.django.html
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_list.django.html
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/template_tags/devilry_group_comment_user_is_none.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templatetags/__init__.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/templatetags/devilry_group_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/__init__.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_devilry_group_mommy_factories.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_templatetags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_crinstance/__init__.py
+-rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_crinstance/test_crinstance_admin.py
+-rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_crinstance/test_crinstance_examiner.py
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_crinstance/test_crinstance_student.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_download/__init__.py
+-rw-r--r--   0        0        0    21694 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_download/test_batchdownload_api.py
+-rw-r--r--   0        0        0    10095 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_download/test_batchframework_compression.py
+-rw-r--r--   0        0        0    17151 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_download/test_feedbackfeed_bulkfiledownload.py
+-rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_download/test_feedbackfeed_filedownload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/admin/__init__.py
+-rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/admin/test_comment_edit_history.py
+-rw-r--r--   0        0        0    37226 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/admin/test_feedbackfeed_admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/__init__.py
+-rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_comment_edit_history.py
+-rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_delete_comment.py
+-rw-r--r--   0        0        0    50866 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_discuss.py
+-rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_comment.py
+-rw-r--r--   0        0        0    13104 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_grade.py
+-rw-r--r--   0        0        0    37037 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_feedback.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/__init__.py
+-rw-r--r--   0        0        0    30200 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_admin.py
+-rw-r--r--   0        0        0    25291 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_common.py
+-rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_examiner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/student/__init__.py
+-rw-r--r--   0        0        0    14087 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/student/test_comment_edit_history.py
+-rw-r--r--   0        0        0   109725 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/student/test_feedbackfeed_student.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed_builders/__init__.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_sidebarbuilder.py
+-rw-r--r--   0        0        0    21620 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_timeline_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_models/__init__.py
+-rw-r--r--   0        0        0    18792 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_models/test_feedback_set.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_models/test_feedbackfeed_model.py
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_models/test_feedbackset_passed_pervious_period.py
+-rw-r--r--   0        0        0    17503 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/tests/test_models/test_group_comment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/utils/__init__.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/utils/download_response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/__init__.py
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/cradmin_comment_history.py
+-rw-r--r--   0        0        0    24391 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/cradmin_feedbackfeed_base.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/group_comment_edit_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/admin/__init__.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/admin/feedbackfeed_admin.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/admin/group_comment_history.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/admin/manage_deadline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/download_files/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/download_files/backends.py
+-rw-r--r--   0        0        0    16091 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/download_files/batch_download_api.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/download_files/batch_download_files.py
+-rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/download_files/feedbackfeed_bulkfiledownload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/examiner/__init__.py
+-rw-r--r--   0        0        0    21303 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/examiner/feedbackfeed_examiner.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/examiner/group_comment_history.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/examiner/manage_deadline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/student/__init__.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/student/feedbackfeed_student.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_group/views/student/group_comment_history.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/models.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/urls.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/templates/devilry_header/about_me.django.html
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/templates/devilry_header/app.django.html
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/templates/devilry_header/header2_extjsinclude.django.html
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/templates/devilry_header/header2include.django.html
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/templates/devilry_header/includes/change_language.django.html
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/tests/__init__.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/tests/test_aboutme.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/tests/test_change_language.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/views/__init__.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/views/about_me.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_header/views/change_language.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_help/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_help/tests.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_help/urls.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_help/views.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_help/templates/devilry_help/help.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_i18n/__init__.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_i18n/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_i18n/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/__init__.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporter.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/models.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/management/commands/__init__.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/management/commands/devilry_import_v2_database.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/migrations/0001_initial.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/migrations/0002_auto_20190624_1238.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/migrations/0003_auto_20210427_1350.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/migrations/__init__.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/__init__.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/assignment_importer.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/assignmentgroup_importer.py
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/candidate_examiner_importer.py
+-rw-r--r--   0        0        0    13855 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/delivery_feedback_importers.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/feedbackset_importer.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/modelimporter_utils.py
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/node_importer.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/period_importer.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/pointrange_to_grade_importer.py
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/qualifiesforexam_importer.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/relateduser_importer.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/subject_importer.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/user_importer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/scripts/__init__.py
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/scripts/user_add_missing_data_from_json.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/__init__.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/importer_testcase_mixin.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentgroupimporter.py
+-rw-r--r--   0        0        0    11674 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentimporter.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_candidateimporter.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_commentfilecontentimporter.py
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_deliveryimporter.py
+-rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_examinerimporter.py
+-rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_feedbacksetimporter.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_filemetaimporter.py
+-rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_nodeimporter.py
+-rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_periodimporter.py
+-rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointrangetogradeimporter.py
+-rw-r--r--   0        0        0     7374 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointtogrademapimporter.py
+-rw-r--r--   0        0        0    14419 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_qualifiesforexam_importer.py
+-rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedexaminerimporter.py
+-rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedstudentimporter.py
+-rw-r--r--   0        0        0    22341 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_staticfeedbackimporter.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_subjectimporter.py
+-rw-r--r--   0        0        0     8108 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_userimporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_scripts/__init__.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_scripts/test_user_add_missing_data_from_json.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/__init__.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2assignment_directoryparser.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2assignmentgroup_directoryparser.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2candidate_directoryparser.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2deadline_directoryparser.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2delivery_directoryparser.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2examiner_directoryparser.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2filemeta_directoryparser.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2node_directoryparser.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2period_directoryparser.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2pointrangetograde_directoryparser.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2pointtogrademap_directoryparser.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2qualifiesforexam_finalexam_directoryparser.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2qualifiesforexam_status_directoryparser.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2relatedexaminer_directoryparser.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2relatedstudent_directoryparser.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2staticfeedback_directoryparser.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2subject_directoryparser.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2user_directoryparser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_markup/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_markup/models.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_markup/parse_markdown.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_markup/urls.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_markup/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_markup/markdown_extensions/__init__.py
+-rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_markup/markdown_extensions/code_diff.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_markup/markdown_extensions/latex_math.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_markup/templates/devilry_markup/code_diff.html
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_markup/templates/devilry_markup/latex_math.html
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_markup/templates/markup/load_latex_support.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/admin.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/migrations/0002_auto_20210427_1350.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/migrations/0003_alter_message_context_type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/migrations/__init__.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/models/__init__.py
+-rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/models/base.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/templates/devilry_message/for_test.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/tests/__init__.py
+-rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/tests/test_message.py
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/tests/test_message_receiver.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/utils/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_message/utils/subject_generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/__init__.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/admin.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/apps.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/cradmin_app.py
+-rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/models.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/pluginhelpers.py
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/plugintyperegistry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/listbuilder/__init__.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/listbuilder/assignment_listbuilder_list.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/listbuilder/plugin_listbuilder_list.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/migrations/0001_initial.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/migrations/0002_auto_20170223_1112.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/migrations/0003_auto_20170629_1914.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/migrations/0004_auto_20210427_1350.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/migrations/0005_deletedqualifiesforfinalexam.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/migrations/0006_status_plugin_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tablebuilder/__init__.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tablebuilder/tablebuilder.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/base.django.html
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/list_statuses.django.html
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/print_view.html
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/retract_status.django.html
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/selectplugin.django.html
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_preview.django.html
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_show.html
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/includes/qualification_table.django.html
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/assignment_item_value.django.html
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/description.django.html
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/plugin_item_value.django.html
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/tablebuilder/qualificationstatus_valueitem.django.html
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/tablebuilder/relatedstudent_valueitem.django.html
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/tablebuilder/tableheader_valueitem.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/__init__.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_list_statuses_view.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_models.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_plugin_listbuilder_list.py
+-rw-r--r--   0        0        0    16296 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_pluginhelpers.py
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_pluginselection_view.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_plugintyperegistry.py
+-rw-r--r--   0        0        0    17221 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_preview.py
+-rw-r--r--   0        0        0    22999 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_showstatus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/utils/__init__.py
+-rw-r--r--   0        0        0    21904 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/utils/groups_groupedby_relatedstudent_and_assignments.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/views/__init__.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/views/list_statuses_view.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/views/plugin_mixin.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/views/pluginselection_view.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/views/proxyview.py
+-rw-r--r--   0        0        0    14987 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/views/qualification_preview_view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/views/plugin_base_views/__init__.py
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/views/plugin_base_views/base_multiselect_view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/__init__.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/apps.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/models.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/plugin.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/resultscollector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/tests/__init__.py
+-rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/tests/test_resultscollector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/views/__init__.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/views/select_assignment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_points/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_points/apps.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_points/models.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_points/plugin.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_points/resultscollector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_points/tests/__init__.py
+-rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_points/tests/test_resultscollector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_points/views/__init__.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_points/views/select_assignment_and_points.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_students/__init__.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_students/apps.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_students/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_students/tests/__init__.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_students/tests/test_student_selection_view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_students/views/__init__.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_students/views/select_students.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/__init__.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/abstract_generator.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/admin.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/generator_registry.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/models.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/rq_task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/urls.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/migrations/0001_initial.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/migrations/0002_auto_20210427_1350.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/migrations/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/templates/devilry_report/download_report.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/tests/__init__.py
+-rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/tests/test_download_report_view.py
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/tests/test_generator_registry.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/tests/test_report_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/views/__init__.py
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_report/views/download_report.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_resetpassword/__init__.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_resetpassword/urls.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_rest/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_rest/__init__.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_rest/auth.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_rest/formfields.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_rest/models.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_rest/serializehelpers.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_rest/testclient.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_rest/tests/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_rest/tests/test_serializehelpers.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_sandbox/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_sandbox/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_sandbox/models.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_sandbox/sandbox.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_sandbox/urls.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_sandbox/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_sandbox/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_sandbox/management/commands/__init__.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_sandbox/management/commands/devilry_sandboxcreate.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_sandbox/templates/devilry_sandbox/createsubject.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_settings/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_settings/models.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_settings/urls.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_settings/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/__init__.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/api/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/api/assignment/__init__.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/api/assignment/api_utils.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/api/assignment/examiner_average_grading_points.py
+-rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/api/assignment/examiner_details.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/api/assignment/examiner_group_results.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/management/commands/__init__.py
+-rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/management/commands/devilry_create_test_course.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/management/commands/devilry_statistics_make_assignment_with_graded_groups.py
+-rw-r--r--   0        0        0   606439 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/static/devilry_statistics/6.3.0rc2/devilry_statistics_all.js
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/.babelrc
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/.editorconfig
+-rw-r--r--   0        0        0   475670 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/package-lock.json
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/package.json
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/webpack.config.js
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/devilry_statistics_all.js
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerAverageGradingPointsWidget.js
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerDetailsWidget.js
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerGroupResultWidget.js
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/registerAllWidgets.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/tests/__init__.py
+-rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/tests/test_api_examiner_average_grading_points.py
+-rw-r--r--   0        0        0    18649 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/tests/test_api_examiner_details.py
+-rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_statistics/tests/test_api_examiner_group_result.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/__init__.py
+-rw-r--r--   0        0        0     5154 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/models.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/cradminextensions/__init__.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/cradminextensions/columntypes.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/cradminextensions/devilry_crinstance_student.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/cradminextensions/devilry_crmenu_student.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/cradminextensions/studentobjecttable.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/migrations/__init__.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/add_delivery.django.html
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/contactapp/contact.django.html
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery-number-column.django.html
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery-status-column.django.html
+-rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_details.django.html
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_list.django.html
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/overviewapp/overview.django.html
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_delete.django.html
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond.django.html
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond_standalone.django.html
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/projectgroup_overview.django.html
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_period/assignmentsapp/assignmentgroup-list.django.html
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_period/assignmentsapp/statuscolumn.django.html
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_student/allperiods/allperiods.django.html
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_student/recentdeliveriesapp/delivery-summary-with-assignment-column.django.html
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_student/waitingfordeliveriesapp/last-deadline.django.html
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_student/waitingfordeliveriesapp/waiting-for-deliveries-list.django.html
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/delivery-summary-column.django.html
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/naturaltime-and-datetime-column.django.html
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/naturaltime-column.django.html
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/dashboard/dashboard.django.html
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/include/feedback-rendered-view.django.html
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/include/group_breadcrumb.django.html
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/period/overview.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templatetags/__init__.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/templatetags/devilry_student_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/tests/__init__.py
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/tests/test_models.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/tests/test_templatetags.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/tests/upload_testfile1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/tests/test_cradminextensions/__init__.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/tests/test_cradminextensions/test_devilry_crmenu_student.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/tests/test_dashboard/__init__.py
+-rw-r--r--   0        0        0    14380 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/tests/test_dashboard/test_allperiods.py
+-rw-r--r--   0        0        0    41388 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/tests/test_dashboard/test_dashboard.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/tests/test_group/__init__.py
+-rw-r--r--   0        0        0    88623 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/tests/test_group/test_projectgroupapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/tests/test_period/__init__.py
+-rw-r--r--   0        0        0    28524 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/tests/test_period/test_overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/views/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/views/show_delivery.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/views/dashboard/__init__.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/views/dashboard/allperiods.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/views/dashboard/crinstance_dashboard.py
+-rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/views/dashboard/dashboard.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/views/group/__init__.py
+-rw-r--r--   0        0        0    14862 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/views/group/projectgroupapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/views/period/__init__.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/views/period/crinstance_period.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_student/views/period/overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/models.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tasks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/delete_periods/__init__.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/delete_periods/period_delete.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/examples/relatedexaminers.json
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/examples/relatedstudents.json
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/examples/relatedstudents_email_instead_of_username.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_anonymize_database.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_clear_allauth_account_tables.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_compressed_archives.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_inactive_users.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_message_receivers.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_messages_without_receivers.py
+-rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_periods.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_fix_missing_first_feedbackset.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_mark_as_passed_in_previous_period.py
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodadd.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodadminadd.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodadminclear.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodsearch.py
+-rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedexaminers.py
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedstudents.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_permissiongroup_add_subject.py
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_qualifiedforfinalexam_delete_duplicates.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_rename_periodtag_prefix.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_resend_failed_messages.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_setup_dataporten_provider.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_setup_primary_domain.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_show_assignment_guidelines.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectadd.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectadminadd.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectadminclear.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectsearch.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_test_rq_task.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_useradd.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_useraddbulk.py
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_usermerge.py
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_usermod.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/__init__.py
+-rw-r--r--   0        0        0    14750 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_inactive_users.py
+-rw-r--r--   0        0        0    19826 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_periods.py
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminadd.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminclear.py
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_permissiongroup_add_subject.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_qualifiedforfinalexam_delete_duplicates.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadd.py
+-rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminadd.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminclear.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_useraddbulk.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_usermod.py
+-rw-r--r--   0        0        0     7755 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_resend_failed_messages.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/models.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/urls.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/views.py
+-rw-r--r--   0        0        0    40723 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/media/images/groovepaper.png
+-rw-r--r--   0        0        0    14235 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/media/images/favicons/apple-touch-icon.png
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/media/images/favicons/favicon.ico
+-rw-r--r--   0        0        0    65078 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/devilry_all.js
+-rw-r--r--   0        0        0   474892 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/devilry_all.js.map
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/LICENSE
+-rw-r--r--   0        0        0    23112 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/katex.min.css
+-rw-r--r--   0        0        0   598523 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/katex.mjs
+-rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/auto-render.js
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/auto-render.min.js
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/auto-render.mjs
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/copy-tex.css
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/copy-tex.js
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/copy-tex.min.css
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/copy-tex.min.js
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/copy-tex.mjs
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/mathtex-script-type.js
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/mathtex-script-type.min.js
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/mathtex-script-type.mjs
+-rw-r--r--   0        0        0    79571 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/mhchem.js
+-rw-r--r--   0        0        0    33776 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/mhchem.min.js
+-rw-r--r--   0        0        0    75577 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/mhchem.mjs
+-rw-r--r--   0        0        0    24069 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/render-a11y-string.js
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/render-a11y-string.min.js
+-rw-r--r--   0        0        0    20207 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/render-a11y-string.mjs
+-rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_AMS-Regular.ttf
+-rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_AMS-Regular.woff
+-rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_AMS-Regular.woff2
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Caligraphic-Bold.ttf
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Caligraphic-Bold.woff2
+-rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Caligraphic-Regular.ttf
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Caligraphic-Regular.woff2
+-rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Fraktur-Bold.ttf
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Fraktur-Bold.woff2
+-rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Fraktur-Regular.ttf
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Fraktur-Regular.woff2
+-rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Bold.ttf
+-rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Bold.woff2
+-rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-BoldItalic.ttf
+-rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-BoldItalic.woff2
+-rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Italic.ttf
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Italic.woff2
+-rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Regular.ttf
+-rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Regular.woff2
+-rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Math-BoldItalic.ttf
+-rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Math-BoldItalic.woff2
+-rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Math-Italic.ttf
+-rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Math-Italic.woff2
+-rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Bold.ttf
+-rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Bold.woff2
+-rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Italic.ttf
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Italic.woff2
+-rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Regular.ttf
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Regular.woff2
+-rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Script-Regular.ttf
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Script-Regular.woff2
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size1-Regular.ttf
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size1-Regular.woff2
+-rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size2-Regular.ttf
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size2-Regular.woff2
+-rw-r--r--   0        0        0     7588 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size3-Regular.ttf
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size3-Regular.woff2
+-rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size4-Regular.ttf
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size4-Regular.woff2
+-rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Typewriter-Regular.ttf
+-rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Typewriter-Regular.woff2
+-rw-r--r--   0        0        0    28426 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/commentEditor.js
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/cookie.js
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/examinerSelfAssignButton.js
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/feedbackfeedNavigationHandler.js
+-rw-r--r--   0        0        0    20380 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/fileupload.js
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/helloWorld.js
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/latex_math.js
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/webcomponent_utils.js
+-rw-r--r--   0        0        0   292259 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/styles/cradmin_theme_devilry_mainpages/theme.css
+-rw-r--r--   0        0        0   220567 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/styles/cradmin_theme_devilry_superuserui/theme.css
+-rw-r--r--   0        0        0    20335 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/vendor/fonts/glyphicons/glyphicons-halflings-regular.eot
+-rw-r--r--   0        0        0    62927 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/vendor/fonts/glyphicons/glyphicons-halflings-regular.svg
+-rw-r--r--   0        0        0    41280 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/vendor/fonts/glyphicons/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/vendor/fonts/glyphicons/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/templates/devilry_deploy/custom_css.django.css
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/templates/devilry_deploy/custom_css_base.django.html
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/templates/devilry_deploy/footer.django.html
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/templates/devilry_deploy/footer_base.django.html
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/templates/devilry_deploy/frontpage_footer.django.html
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/templates/devilry_deploy/login_footer.django.html
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/templates/devilry_theme3/favicons.django.html
+-rw-r--r--   0        0        0    25100 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/templates/devilry_theme3/wcag-debug.django.html
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/templates/devilry_theme3/include/devilry_all_js.django.html
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/templates/devilry_theme3/include/includetest.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/templatetags/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/devilry_theme3/templatetags/devilry_theme3_tags.py
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/django_decoupled_docs/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/django_decoupled_docs/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/django_decoupled_docs/models.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/django_decoupled_docs/registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/django_decoupled_docs/templatetags/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/django_decoupled_docs/templatetags/django_decoupled_docs_tags.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   267831 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/locale/en/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0   174762 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   374320 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/locale/nb/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/__init__.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/log.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/settingsproxy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/cradmin_legacy_settings.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/default_urls.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/devilry_test_runner.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/docproxies.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/http_error_handlers.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/i18n.py
+-rw-r--r--   0        0        0     9810 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/projectspecific_settings.py
+-rw-r--r--   0        0        0     8578 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/settings.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/templatecontext.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/formats/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/formats/en/__init__.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/formats/en/formats.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/formats/nb/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/formats/nb/formats.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/management/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/management/commands/__init__.py
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/common/management/commands/devilry_common_merge_candidates.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/__init__.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/dev_urls.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/fabrictasks.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/models.py
+-rw-r--r--   0        0        0   353927 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/dumps/old_default.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/management/commands/__init__.py
+-rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/management/commands/devilry_developer_create_deliveries_from_filesystemtree.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/management/commands/devilry_developer_delete_all_except_users.py
+-rw-r--r--   0        0        0    15531 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/management/commands/devilry_developer_performance_test_db.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/management/commands/devilry_developer_set_all_passwords_to_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/settings/__init__.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/settings/base.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/settings/codeship_test.py
+-rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/settings/develop.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/settings/docs.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/settings/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/testhelpers/__init__.py
+-rw-r--r--   0        0        0    22236 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/testhelpers/corebuilder.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/testhelpers/datebuilder.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/testhelpers/login.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/testhelpers/skip_rq_tests.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/develop/testhelpers/soupselect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/production/__init__.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/production/settings.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/production/urls.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/project/production/wsgi.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/GroupAssignments.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/GroupNodes.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/OrderedDictFallback.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/__init__.py
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/anonymize_database.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/command.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/create_absolute_url.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/custom_templates.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/datetimeutils.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/delay_middleware.py
+-rw-r--r--   0        0        0     8118 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/delivery_collection.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/devilry_djangoaggregate_functions.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/devilry_email.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/dictutils.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/filewrapperwithexplicitclose.py
+-rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/groups_groupedby_relatedstudent_and_assignment.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/importutils.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/logexceptionsmiddleware.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/management.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/migrationutils.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/models.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/module.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/nodenamesuggestor.py
+-rw-r--r--   0        0        0    11545 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/passed_in_previous_period.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/profile.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/rq_setup.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/setting_utils.py
+-rw-r--r--   0        0        0     7675 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/stream_archives.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/verify_unique_entries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/api/__init__.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/api/api_test_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/demodb/__init__.py
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/demodb/demousers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/graphviz/__init__.py
+-rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/graphviz/djangomodels.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/graphviz/dot.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/graphviz/sphinx.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/tests/delivery_collection_tests.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/tests/importutils.py
+-rwxr-xr-x   0        0        0     7534 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/tests/streamable_archive_tests.py
+-rw-r--r--   0        0        0    15352 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/tests/test_anonymize_db.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/tests/test_datetimeutils.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/tests/test_groups_groupedby_relatedstudent_and_assignment.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/tests/test_nodenamesuggestor.py
+-rw-r--r--   0        0        0    47879 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/tests/test_passed_in_previous_period.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/tests/test_setting_utils.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/devilry/utils/tests/test_url_datetime.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/LICENSE
+-rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/README.md
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    10953 2020-02-02 00:00:00.000000 devilry-6.3.0rc2/PKG-INFO
```

### Comparing `devilry-6.3.0rc1/devilry/.coveragerc` & `devilry-6.3.0rc2/devilry/.coveragerc`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/admin.py` & `devilry-6.3.0rc2/devilry/apps/core/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/baker_recipes.py` & `devilry-6.3.0rc2/devilry/apps/core/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/deliverystore.py` & `devilry-6.3.0rc2/devilry/apps/core/deliverystore.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/devilry_core_baker_factories.py` & `devilry-6.3.0rc2/devilry/apps/core/devilry_core_baker_factories.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/group_user_lookup.py` & `devilry-6.3.0rc2/devilry/apps/core/group_user_lookup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/testhelper.py` & `devilry-6.3.0rc2/devilry/apps/core/testhelper.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/testhelpers.py` & `devilry-6.3.0rc2/devilry/apps/core/testhelpers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/urls.py` & `devilry-6.3.0rc2/devilry/apps/core/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/api/applicationstate.py` & `devilry-6.3.0rc2/devilry/apps/core/api/applicationstate.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0002_auto_20150915_1127.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0002_auto_20150915_1127.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0003_auto_20150917_1537.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0003_auto_20150917_1537.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0009_assignmentgroup_batchoperation.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0009_assignmentgroup_batchoperation.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0010_assignment_anonymizationmode.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0010_assignment_anonymizationmode.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0011_datamigrate_anonymous_to_anonymizationmode.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0011_datamigrate_anonymous_to_anonymizationmode.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0013_auto_20160111_2021.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0013_auto_20160111_2021.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0015_assignment_uses_custom_candidate_ids.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0015_assignment_uses_custom_candidate_ids.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0017_candidate_relatedstudent_replaces_student_field.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0017_candidate_relatedstudent_replaces_student_field.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0018_auto_20160112_1923.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0018_auto_20160112_1923.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0019_auto_20160113_2037.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0019_auto_20160113_2037.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0021_examiner_relatedexaminer_replaces_user_field.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0021_examiner_relatedexaminer_replaces_user_field.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0027_auto_20160116_1843.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0027_auto_20160116_1843.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0029_assignmentgrouphistory.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0029_assignmentgrouphistory.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0030_auto_20170124_1504.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0030_auto_20170124_1504.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0031_auto_20170125_1601.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0031_auto_20170125_1601.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0032_datamigrate_update_for_no_none_values_in_assignment_firstdeadline.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0032_datamigrate_update_for_no_none_values_in_assignment_firstdeadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0033_auto_20170220_1330.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0033_auto_20170220_1330.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0034_auto_20170303_1308.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0034_auto_20170303_1308.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0037_auto_20170620_1515.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0037_auto_20170620_1515.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0038_auto_20170621_1720.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0038_auto_20170621_1720.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0040_auto_20180214_1654.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0040_auto_20180214_1654.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0041_auto_20180220_0651.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0041_auto_20180220_0651.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0042_candidateassignmentgrouphistory_examinerassignmentgrouphistory.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0042_candidateassignmentgrouphistory_examinerassignmentgrouphistory.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0043_auto_20180302_1139.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0043_auto_20180302_1139.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0044_auto_20190624_1238.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0044_auto_20190624_1238.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/migrations/0046_auto_20220519_1043.py` & `devilry-6.3.0rc2/devilry/apps/core/migrations/0046_auto_20220519_1043.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/__init__.py` & `devilry-6.3.0rc2/devilry/apps/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/abstract_applicationkeyvalue.py` & `devilry-6.3.0rc2/devilry/apps/core/models/abstract_applicationkeyvalue.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/abstract_is_candidate.py` & `devilry-6.3.0rc2/devilry/apps/core/models/abstract_is_candidate.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/abstract_is_examiner.py` & `devilry-6.3.0rc2/devilry/apps/core/models/abstract_is_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/assignment.py` & `devilry-6.3.0rc2/devilry/apps/core/models/assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/assignment_group.py` & `devilry-6.3.0rc2/devilry/apps/core/models/assignment_group.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/assignment_group_history.py` & `devilry-6.3.0rc2/devilry/apps/core/models/assignment_group_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/basenode.py` & `devilry-6.3.0rc2/devilry/apps/core/models/basenode.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/candidate.py` & `devilry-6.3.0rc2/devilry/apps/core/models/candidate.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/custom_db_fields.py` & `devilry-6.3.0rc2/devilry/apps/core/models/custom_db_fields.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/deadline.py` & `devilry-6.3.0rc2/devilry/apps/core/models/deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/delivery.py` & `devilry-6.3.0rc2/devilry/apps/core/models/delivery.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/devilryuserprofile.py` & `devilry-6.3.0rc2/devilry/apps/core/models/devilryuserprofile.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/examiner.py` & `devilry-6.3.0rc2/devilry/apps/core/models/examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/examiner_candidate_group_history.py` & `devilry-6.3.0rc2/devilry/apps/core/models/examiner_candidate_group_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/filemeta.py` & `devilry-6.3.0rc2/devilry/apps/core/models/filemeta.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/groupinvite.py` & `devilry-6.3.0rc2/devilry/apps/core/models/groupinvite.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/model_utils.py` & `devilry-6.3.0rc2/devilry/apps/core/models/model_utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/period.py` & `devilry-6.3.0rc2/devilry/apps/core/models/period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/period_tag.py` & `devilry-6.3.0rc2/devilry/apps/core/models/period_tag.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/pointrange_to_grade.py` & `devilry-6.3.0rc2/devilry/apps/core/models/pointrange_to_grade.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/relateduser.py` & `devilry-6.3.0rc2/devilry/apps/core/models/relateduser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/save_interface.py` & `devilry-6.3.0rc2/devilry/apps/core/models/save_interface.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/static_feedback.py` & `devilry-6.3.0rc2/devilry/apps/core/models/static_feedback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/models/subject.py` & `devilry-6.3.0rc2/devilry/apps/core/models/subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/comment-summary.django.html` & `devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/comment-summary.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-full-plain.django.html` & `devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-full-plain.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-full.django.html` & `devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-full.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/groupstatus.django.html` & `devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/groupstatus.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/relatedexaminers-on-period-tag.django.html` & `devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/relatedexaminers-on-period-tag.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/templates/devilry_core/templatetags/relatedstudents-on-period-tag.django.html` & `devilry-6.3.0rc2/devilry/apps/core/templates/devilry_core/templatetags/relatedstudents-on-period-tag.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/templates/search/indexes/core/assignmentgroup_text.txt` & `devilry-6.3.0rc2/devilry/apps/core/templates/search/indexes/core/assignmentgroup_text.txt`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/templatetags/devilry_core_tags.py` & `devilry-6.3.0rc2/devilry/apps/core/templatetags/devilry_core_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_assignment.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_assignment_group.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_assignment_group.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_assignment_group_history.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_assignment_group_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_candidate.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_candidate.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_deadline.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_devilry_core_tags.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_devilry_core_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_examiner.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_group_user_lookup.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_group_user_lookup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_groupinvite.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_groupinvite.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_period.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_period_tags.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_period_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_pointrange_to_grade.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_pointrange_to_grade.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_relateduser.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_relateduser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/tests/test_subject.py` & `devilry-6.3.0rc2/devilry/apps/core/tests/test_subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/apps/core/views/download_staticfeedbackfileattachment.py` & `devilry-6.3.0rc2/devilry/apps/core/views/download_staticfeedbackfileattachment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/coreutils/utils.py` & `devilry-6.3.0rc2/devilry/coreutils/utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/admin.py` & `devilry-6.3.0rc2/devilry/devilry_account/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/apps.py` & `devilry-6.3.0rc2/devilry/devilry_account/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/crinstance_account.py` & `devilry-6.3.0rc2/devilry/devilry_account/crinstance_account.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/middleware.py` & `devilry-6.3.0rc2/devilry/devilry_account/middleware.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/models.py` & `devilry-6.3.0rc2/devilry/devilry_account/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/user_merger.py` & `devilry-6.3.0rc2/devilry/devilry_account/user_merger.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/authbackend/default.py` & `devilry-6.3.0rc2/devilry/devilry_account/authbackend/default.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/authbackend/ldap.py` & `devilry-6.3.0rc2/devilry/devilry_account/authbackend/ldap.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/cradminextensions/devilry_crmenu_account.py` & `devilry-6.3.0rc2/devilry/devilry_account/cradminextensions/devilry_crmenu_account.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/crapps/account/index.py` & `devilry-6.3.0rc2/devilry/devilry_account/crapps/account/index.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/crapps/account/select_language.py` & `devilry-6.3.0rc2/devilry/devilry_account/crapps/account/select_language.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/devilry_account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/migrations/0002_auto_20150917_1731.py` & `devilry-6.3.0rc2/devilry/devilry_account/migrations/0002_auto_20150917_1731.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/migrations/0003_datamigrate-admins-into-permissiongroups.py` & `devilry-6.3.0rc2/devilry/devilry_account/migrations/0003_datamigrate-admins-into-permissiongroups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/migrations/0004_auto_20151222_1955.py` & `devilry-6.3.0rc2/devilry/devilry_account/migrations/0004_auto_20151222_1955.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/migrations/0005_auto_20160113_2037.py` & `devilry-6.3.0rc2/devilry/devilry_account/migrations/0005_auto_20160113_2037.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/migrations/0006_auto_20160120_0424.py` & `devilry-6.3.0rc2/devilry/devilry_account/migrations/0006_auto_20160120_0424.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/migrations/0007_auto_20210427_1350.py` & `devilry-6.3.0rc2/devilry/devilry_account/migrations/0007_auto_20210427_1350.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/migrations/0008_auto_20220510_1307.py` & `devilry-6.3.0rc2/devilry/devilry_account/migrations/0008_auto_20220510_1307.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/migrations/0009_mergeduser.py` & `devilry-6.3.0rc2/devilry/devilry_account/migrations/0009_mergeduser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html` & `devilry-6.3.0rc2/devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/templates/devilry_account/crapps/account/select_language.django.html` & `devilry-6.3.0rc2/devilry/devilry_account/templates/devilry_account/crapps/account/select_language.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/templatetags/devilry_account_tags.py` & `devilry-6.3.0rc2/devilry/devilry_account/templatetags/devilry_account_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/tests/test_devilry_account_tags.py` & `devilry-6.3.0rc2/devilry/devilry_account/tests/test_devilry_account_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/tests/test_middleware.py` & `devilry-6.3.0rc2/devilry/devilry_account/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/tests/test_models.py` & `devilry-6.3.0rc2/devilry/devilry_account/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/tests/test_user_merger.py` & `devilry-6.3.0rc2/devilry/devilry_account/tests/test_user_merger.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/tests/authbackend/test_default.py` & `devilry-6.3.0rc2/devilry/devilry_account/tests/authbackend/test_default.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/tests/test_crapps/test_account/test_index.py` & `devilry-6.3.0rc2/devilry/devilry_account/tests/test_crapps/test_account/test_index.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_account/tests/test_crapps/test_account/test_select_language.py` & `devilry-6.3.0rc2/devilry/devilry_account/tests/test_crapps/test_account/test_select_language.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/apps.py` & `devilry-6.3.0rc2/devilry/devilry_admin/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tasks.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tasks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/urls.py` & `devilry-6.3.0rc2/devilry/devilry_admin/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/devilry_crmenu_admin.py` & `devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/devilry_crmenu_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_assignmentgroup.py` & `devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_assignmentgroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedexaminer.py` & `devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedexaminer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedstudent.py` & `devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedstudent.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listfilter/listfilter_assignmentgroup.py` & `devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listfilter/listfilter_assignmentgroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py` & `devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/listfilter/listfilter_tags.py` & `devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/listfilter/listfilter_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/cradminextensions/multiselect2/multiselect2_relatedstudent.py` & `devilry-6.3.0rc2/devilry/devilry_admin/cradminextensions/multiselect2/multiselect2_relatedstudent.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/add_groups_to_examiner.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/add_groups_to_examiner.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/examinerdetails.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/examinerdetails.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/remove_groups_from_examiner.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/remove_groups_from_examiner.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-add.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-add.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-replace.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-replace.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag-item-value.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/random.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/random.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/select_method.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/select_method.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/custom-table.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/custom-table.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/gradingconfiguration-update.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/gradingconfiguration-update.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/examiners.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/examiners.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/gradingconfiguration.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/gradingconfiguration.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/published.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/published.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/settings.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/settings.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/statistics.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/statistics.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/students.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/students.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/utilities.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/utilities.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/includes/batchdownload_assignment.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/includes/batchdownload_assignment.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-item-value.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/candidate-item-value.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/candidate-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/confirm-view.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/confirm-view.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select-period-view.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select-period-view.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select_groups_to_pass.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select_groups_to_pass.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/statistics/overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/statistics/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/merge_groups.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/merge_groups.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/split_groups.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/split_groups.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-accumulated-score.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-accumulated-score.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-assignment-item-value.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-assignment-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-method.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-method.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-period-item-value.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-period-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/confirm.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/confirm.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/manual-select-students.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/manual-select-students.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/preview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/preview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/select-assignments.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/select-assignments.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-method.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-method.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-period-item-value.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-period-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/confirm.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/confirm.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupdetails/view.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupdetails/view.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/common/abstract-type-in-users.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/common/abstract-type-in-users.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/common/admin-list-view.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/common/admin-list-view.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/common/admins-explained.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/common/admins-explained.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/group_by_assignment.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/group_by_assignment.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_groups.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_groups.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_users.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_users.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/listbuilder/assignmentgroup_listbuilder/value.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/listbuilder/assignmentgroup_listbuilder/value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/listbuilder/listbuilder_relatedexaminer/onassignment-itemvalue.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/listbuilder/listbuilder_relatedexaminer/onassignment-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/admins/add.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/admins/add.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/admins/overview-itemvalue.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/admins/overview-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/admins/overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/admins/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/devilry_all_results_overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/devilry_all_results_overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/result_cell_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/result_cell_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/createassignment.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/createassignment.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/helpbox.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/helpbox.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/success_message.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/success_message.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/suggested_deadlines.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/suggested_deadlines.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/edit/updateview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/edit/updateview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/examiners/add.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/examiners/add.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview-itemvalue.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/add-tag.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/add-tag.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/base-multiselect-view.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/base-multiselect-view.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/crud.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/crud.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/delete.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/delete.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/manage-tags-list-view.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/manage-tags-list-view.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/tag-item-value.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/tag-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/relatedusers/select-method.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/relatedusers/select-method.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/add.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/add.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/overview-itemvalue.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/overview-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/overview_for_period_admins.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/overview_for_period_admins.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/admins/add.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/admins/add.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview-itemvalue.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/edit/updateview.django.html` & `devilry-6.3.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/edit/updateview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_anonymizationmode.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_anonymizationmode.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_batchframework_tasks.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_batchframework_tasks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_crinstance_assignment.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_crinstance_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_deadline_handling.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_deadline_handling.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_examiner_selfassign.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_examiner_selfassign.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_examiner_statistics.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_examiner_statistics.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_first_deadline.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_first_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_grading_configuration.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_grading_configuration.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_long_and_shortname.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_long_and_shortname.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_projectgroups.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_projectgroups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_publishing_time.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_publishing_time.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_add_groups_to_examiner.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_add_groups_to_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_bulk_organize.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_bulk_organize.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_examinerdetails.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_examinerdetails.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_remove_groups_from_examiner.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_remove_groups_from_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period_manual.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period_manual.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_create_groups.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_create_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_create_groups_accumulated_score.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_create_groups_accumulated_score.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_delete_groups.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_delete_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupdetails.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupdetails.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_merge_groups.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_merge_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_replace_groups.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_replace_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_split_group.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_split_group.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_baseinforview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_baseinforview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_basemultiselectview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_basemultiselectview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_groupviewmixin.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_groupviewmixin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/assignment/test_download_files/test_batchdownload_api.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/assignment/test_download_files/test_batchdownload_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/common/admins_common_testmixins.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/common/admins_common_testmixins.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/common/test_bulkimport_users_common.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/common/test_bulkimport_users_common.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/cradminextensions/test_devilry_crmenu_admin.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/cradminextensions/test_devilry_crmenu_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedexaminer.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedexaminer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedstudent.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedstudent.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/cradminextensions/test_multiselect2/test_multiselect2_relatedstudent.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/cradminextensions/test_multiselect2/test_multiselect2_relatedstudent.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/dashboard/test_createsubject.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/dashboard/test_createsubject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/dashboard/test_overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/dashboard/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_assignment_listview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_assignment_listview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_student_listview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_student_listview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_admins.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_admins.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_createassignment.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_createassignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_crinstance_period.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_crinstance_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_edit.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_edit.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_examiners.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_examiners.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_overview_all_results.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_overview_all_results.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_period_all_results_collector.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_period_all_results_collector.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_students.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_students.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags_relatedusers.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags_relatedusers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/period/test_report/test_all_results_generator.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/period/test_report/test_all_results_generator.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/subject/test_admins.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/subject/test_admins.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/subject/test_createperiod.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/subject/test_createperiod.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/subject/test_crinstance_subject.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/subject/test_crinstance_subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/subject/test_edit.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/subject/test_edit.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/subject/test_overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/subject/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/test_crinstance_for_periodadmin.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/test_crinstance_for_periodadmin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/test_overview_for_periodadmin.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/test_overview_for_periodadmin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/test_subject_redirect.py` & `devilry-6.3.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/test_subject_redirect.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/anonymizationmode.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/anonymizationmode.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/crinstance_assignment.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/crinstance_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/deadline_handling.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/deadline_handling.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiner_selfassign.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiner_selfassign.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/first_deadline.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/first_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/gradingconfiguration.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/gradingconfiguration.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/projectgroups.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/projectgroups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/publishing_time.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/publishing_time.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/download_files/backends.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/download_files/backends.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/download_files/batch_download_api.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/download_files/batch_download_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/download_files/download_archive.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/download_files/download_archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
         filewrapper = zip_backend.get_archive()
         content_type = 'application/octet-stream'
 
         response = http.StreamingHttpResponse(
             filewrapper,
             content_type=content_type
         )
+        response.set_cookie('zipdownload', 'start', max_age=10)
+
         response['content-disposition'] = 'attachment; filename={}'.format(
             archive_name.encode('ascii', 'replace').decode()
         )
         if zip_backend.archive_size() > 0:
             response['content-length'] = zip_backend.archive_size()
 
         return response
```

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiners/add_groups_to_examiner.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiners/add_groups_to_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiners/base_single_examinerview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiners/base_single_examinerview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiners/bulk_organize.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiners/bulk_organize.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiners/examinerdetails.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiners/examinerdetails.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiners/overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiners/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/examiners/remove_groups_from_examiner.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/examiners/remove_groups_from_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/__init__.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/__init__.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_period.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_semester_manual.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_semester_manual.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/statistics/statistics_overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/statistics/statistics_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/create_groups.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/create_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/create_groups_accumulated_score.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/create_groups_accumulated_score.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/delete_groups.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/delete_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/groupdetails.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/groupdetails.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/groupview_base.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/groupview_base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/manage_deadlines.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/manage_deadlines.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/merge_groups.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/merge_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/replace_groups.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/replace_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/assignment/students/split_group.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/assignment/students/split_group.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/common/bulkimport_users_common.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/common/bulkimport_users_common.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/createsubject.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/createsubject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/crinstance_dashboard.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/crinstance_dashboard.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/__init__.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/assignment_list.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/assignment_list.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/filters.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/filters.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/student_list.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/student_list.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/period/admins.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/period/admins.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/period/all_results_generator.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/period/all_results_generator.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/period/createassignment.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/period/createassignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/period/crinstance_period.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/period/crinstance_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/period/edit.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/period/edit.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/period/examiners.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/period/examiners.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/period/overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/period/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/period/overview_all_results.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/period/overview_all_results.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/period/overview_all_results_collector.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/period/overview_all_results_collector.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/period/students.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/period/students.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/period/manage_tags/manage_tags.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/period/manage_tags/manage_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/subject/admins.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/subject/admins.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/subject/createperiod.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/subject/createperiod.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/subject/crinstance_subject.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/subject/crinstance_subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/subject/edit.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/subject/edit.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/subject/overview.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/subject/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/subject_for_period_admin/crinstance_subject_for_periodadmin.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/subject_for_period_admin/crinstance_subject_for_periodadmin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/subject_for_period_admin/overview_for_periodadmin.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/subject_for_period_admin/overview_for_periodadmin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_admin/views/subject_for_period_admin/subject_redirect.py` & `devilry-6.3.0rc2/devilry/devilry_admin/views/subject_for_period_admin/subject_redirect.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_authenticate/allauth_adapter.py` & `devilry-6.3.0rc2/devilry/devilry_authenticate/allauth_adapter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_authenticate/apps.py` & `devilry-6.3.0rc2/devilry/devilry_authenticate/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_authenticate/socialaccount_user_updaters.py` & `devilry-6.3.0rc2/devilry/devilry_authenticate/socialaccount_user_updaters.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_authenticate/urls.py` & `devilry-6.3.0rc2/devilry/devilry_authenticate/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/login.django.html` & `devilry-6.3.0rc2/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/login.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/logout.django.html` & `devilry-6.3.0rc2/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/logout.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_authenticate/views/allauth_views.py` & `devilry-6.3.0rc2/devilry/devilry_authenticate/views/allauth_views.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_authenticate/views/custom_login_view.py` & `devilry-6.3.0rc2/devilry/devilry_authenticate/views/custom_login_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_bulkcreate_users/create_users.py` & `devilry-6.3.0rc2/devilry/devilry_bulkcreate_users/create_users.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_bulkcreate_users/urls.py` & `devilry-6.3.0rc2/devilry/devilry_bulkcreate_users/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/confirm_bulkcreated_users.django.html` & `devilry-6.3.0rc2/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/confirm_bulkcreated_users.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/show_bulkcreated_users.django.html` & `devilry-6.3.0rc2/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/show_bulkcreated_users.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_bulkcreate_users/views/submit_bulk_users.py` & `devilry-6.3.0rc2/devilry/devilry_bulkcreate_users/views/submit_bulk_users.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_changelog/models.py` & `devilry-6.3.0rc2/devilry/devilry_changelog/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_comment/editor_widget.py` & `devilry-6.3.0rc2/devilry/devilry_comment/editor_widget.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_comment/models.py` & `devilry-6.3.0rc2/devilry/devilry_comment/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_comment/api/preview_markdown.py` & `devilry-6.3.0rc2/devilry/devilry_comment/api/preview_markdown.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_comment/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/devilry_comment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_comment/migrations/0002_auto_20160109_1210.py` & `devilry-6.3.0rc2/devilry/devilry_comment/migrations/0002_auto_20160109_1210.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_comment/migrations/0003_auto_20160109_1239.py` & `devilry-6.3.0rc2/devilry/devilry_comment/migrations/0003_auto_20160109_1239.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_comment/migrations/0006_auto_20170621_1720.py` & `devilry-6.3.0rc2/devilry/devilry_comment/migrations/0006_auto_20170621_1720.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_comment/migrations/0010_commentedithistory.py` & `devilry-6.3.0rc2/devilry/devilry_comment/migrations/0010_commentedithistory.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_comment/migrations/0011_auto_20220421_1242.py` & `devilry-6.3.0rc2/devilry/devilry_comment/migrations/0011_auto_20220421_1242.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html` & `devilry-6.3.0rc2/devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_comment/tests/test_models.py` & `devilry-6.3.0rc2/devilry/devilry_comment/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/abstract_batch_action.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/abstract_batch_action.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/admin.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/backend_registry.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/backend_registry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/models.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/backends/backend_mock.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/backends/backend_mock.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/backends/backends_base.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/backends/backends_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Python imports
 import os
 import io
 import zipfile
 import tarfile
 import shutil
 from stat import S_IFREG
-from stream_zip import ZIP_64, stream_zip
+from stream_zip import ZIP_AUTO, stream_zip
 from to_file_like_obj import to_file_like_obj
 
 # Django imports
 from django.conf import settings
 from django.utils import timezone
 
 
@@ -169,16 +169,15 @@
         self.zipped_chunks = None
         self.save_to_disk = save_to_disk
         self.__add_path_extension()
         self._create_path_if_not_exists()
         if chunk_size:
             self.chunk_size = chunk_size
         else:
-            # Default 200MB chunk size
-            self.chunk_size = 1024 * 1024 * 200
+            self.chunk_size = int(0x8000)
 
     def __add_path_extension(self):
         """
         Sets :obj:`~.PythonZipFileBackend.archive_path` to full path by prepending the backend storage location
         to the archive_path. Also adds .zip extension
         """
         self.archive_path = os.path.join(self.get_storage_location(), self.archive_path)
@@ -237,31 +236,32 @@
     def _prep_files(self):
         """
         Prepares the files for Zip creation
         """
         now = timezone.now()
         mode = S_IFREG | 0o600
 
-        def contents(filelike_obj):
-            while chunk := filelike_obj.read(65536):
+        def contents(file_object):
+            filelike_obj = file_object.file
+            while chunk := filelike_obj.read(self.chunk_size):
                 yield chunk
 
         return (
-            (path, now, mode, ZIP_64, contents(filelike_obj))
+            (path, now, mode, ZIP_AUTO(filelike_obj.file.size), contents(filelike_obj))
             for (path, filelike_obj) in self.files
         )
 
     def close(self):
         """
         Must be invoked in order to process the files into an iterable yielding the bytes of the ZIP file.
 
         Readmode is set to True
         """
         prepped_files = self._prep_files()
-        self.zipped_chunks = stream_zip(prepped_files)
+        self.zipped_chunks = stream_zip(prepped_files, chunk_size=self.chunk_size)
         self.readmode = True
 
         if self.save_to_disk:
             self.archive = open(self.archive_path, 'wb')
             for chunk in self.zipped_chunks:
                 self.archive.write(chunk)
```

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/batchjob_mixins/assignment_mixin.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/batchjob_mixins/assignment_mixin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 
 import os
 
 from django.template import defaultfilters
+from django.db.models import Prefetch
 
 from devilry.devilry_compressionutil.batchjob_mixins import feedbackset_mixin
 
 
 class AssignmentBatchMixin(feedbackset_mixin.FeedbackSetBatchMixin):
     """
     Mixin for adding FeedbackSet files to zipfile for all AssignmentGroups in the Assignment the user has access to.
@@ -28,16 +29,26 @@
 
         Returns:
             QuerySet: AssignmentGroup queryset.
         """
         raise NotImplementedError()
 
     def add_assignment_groups(self, user, zipfile_backend, assignment):
-        for group in self.get_assignment_group_queryset(assignment=assignment, user=user):
+        group_queryset = self.get_assignment_group_queryset(assignment=assignment, user=user)
+        group_queryset = group_queryset.prefetch_related(
+            Prefetch(
+                'feedbackset_set',
+                queryset=self.get_feedbackset_queryset()
+            ),
+            'candidates__relatedstudent__user',
+        )
+
+        for group in group_queryset:
             group_path = '{}'.format(group.get_short_displayname())
             for feedback_set in group.feedbackset_set.all():
-                feedback_set_path = 'deadline-{}'.format(defaultfilters.date(feedback_set.current_deadline(), 'Y-m-d-Hi'))
+                feedback_set_path = 'deadline-{}' \
+                    .format(defaultfilters.date(feedback_set.deadline_datetime, 'Y-m-d-Hi'))
                 self.zipfile_add_feedbackset(
                     zipfile_backend=zipfile_backend,
                     feedback_set=feedback_set,
                     sub_path=os.path.join(group_path, feedback_set_path)
                 )
```

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/migrations/0002_auto_20170119_1202.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/migrations/0002_auto_20170119_1202.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/migrations/0003_auto_20170119_1648.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/migrations/0003_auto_20170119_1648.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/migrations/0005_compressedarchivemeta_created_by.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/migrations/0005_compressedarchivemeta_created_by.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/migrations/0006_compressedarchivemeta_created_by_role.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/migrations/0006_compressedarchivemeta_created_by_role.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/tests/test_backend.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/tests/test_model.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_compressionutil/tests/test_registry.py` & `devilry-6.3.0rc2/devilry/devilry_compressionutil/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_acemarkdown.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_acemarkdown.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_crinstance.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_crinstance.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_crmenu.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_crmenu.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/assignment.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/assignmentgroup.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/assignmentgroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_sidebar.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_sidebar.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_timeline.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_timeline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/period.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/permissiongroup.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/permissiongroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/permissiongroupuser.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/permissiongroupuser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listbuilder/subject.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listbuilder/subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listfilter/assignment.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listfilter/assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listfilter/assignmentgroup.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listfilter/assignmentgroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listfilter/user.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listfilter/user.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_listfilter/utils.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_listfilter/utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_multiselect2/user.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_multiselect2/user.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_tablebuilder/base.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_tablebuilder/base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/devilry_tablebuilder/base_new.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/devilry_tablebuilder/base_new.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/cradmin_legacy/standalone-base.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/cradmin_legacy/standalone-base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_acemarkdown.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_acemarkdown.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/account-menuitem.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/account-menuitem.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/examiner-item-value.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/examiner-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-examiner-item-value.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-examiner-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/groupdetails.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/groupdetails.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/admin-itemvalue.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/admin-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/student-itemvalue.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/student-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/permissiongroup/subjectorperiodpermissiongroup-itemvalue.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/permissiongroup/subjectorperiodpermissiongroup-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listfilter/utils/devilry_with_result_value_renderable.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listfilter/utils/devilry_with_result_value_renderable.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/row.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/row.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/table.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/table.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_tablebuilder.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_tablebuilder.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_confirmview.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_confirmview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_createview_with_backlink.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_createview_with_backlink.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_updateview_with_backlink.django.html` & `devilry-6.3.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_updateview_with_backlink.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignment.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignmentgroup.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignmentgroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_sidebar.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_sidebar.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_timeline.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_timeline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_period.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroup.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroupuser.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroupuser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_user.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_user.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_listfilter/test_assignmentgroup_listfilter.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_listfilter/test_assignmentgroup_listfilter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_devilry_multiselect2/test_user.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_devilry_multiselect2/test_user.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/tests/test_tablebuilder/test_table.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/tests/test_tablebuilder/test_table.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_cradmin/viewhelpers/devilry_confirmview.py` & `devilry-6.3.0rc2/devilry/devilry_cradmin/viewhelpers/devilry_confirmview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dataporten_allauth/callback.py` & `devilry-6.3.0rc2/devilry/devilry_dataporten_allauth/callback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dataporten_allauth/views.py` & `devilry-6.3.0rc2/devilry/devilry_dataporten_allauth/views.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/admin.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/bulk_create_queryset_mixin.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/bulk_create_queryset_mixin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/models.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/assignment/triggers.sql` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/assignment/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/assignment_group/triggers.sql` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/assignment_group/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/assignment_group_cached_data/rebuild.sql` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/assignment_group_cached_data/rebuild.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/candidate/triggers.sql` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/candidate/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/comment/triggers.sql` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/comment/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/commentfile/helperfunctions.sql` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/commentfile/helperfunctions.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/commentfile/triggers.sql` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/commentfile/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/examiner/triggers.sql` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/examiner/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/helperfunctions.sql` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/helperfunctions.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/triggers.sql` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/validate.sql` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/validate.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/groupcomment/triggers.sql` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/groupcomment/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/customsql_sqlcode/imageannotationcomment/triggers.sql` & `devilry-6.3.0rc2/devilry/devilry_dbcache/customsql_sqlcode/imageannotationcomment/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/migrations/0002_auto_20170108_0948.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/migrations/0002_auto_20170108_0948.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/migrations/0003_auto_20170108_1341.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/migrations/0003_auto_20170108_1341.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/migrations/0004_auto_20170108_1453.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/migrations/0004_auto_20170108_1453.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/migrations/0005_auto_20170124_1504.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/migrations/0005_auto_20170124_1504.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_assignment_group_cached_data_triggers.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_assignment_group_cached_data_triggers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_benchmarks.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_bulk_create_queryset_mixin.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_bulk_create_queryset_mixin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_candidate_triggers.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_candidate_triggers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_comment_triggers.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_comment_triggers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_examiner_triggers.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_examiner_triggers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_feedbackset_triggers.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_feedbackset_triggers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_dbcache/tests/test_groupcomment_triggers.py` & `devilry-6.3.0rc2/devilry/devilry_dbcache/tests/test_groupcomment_triggers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/cradmin_app.py` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/cradmin_app.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/deadline-bulk-multiselect-filterlistview.django.html` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/deadline-bulk-multiselect-filterlistview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/manage-deadline.django.html` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/manage-deadline.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline-item-value.django.html` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline.django.html` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/suggested-deadlines.django.html` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/suggested-deadlines.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-base.django.html` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/tests/test_deadline_listview.py` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/tests/test_deadline_listview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_admin.py` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_examiner.py` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/tests/test_multiselect_groups.py` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/tests/test_multiselect_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/views/deadline_listview.py` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/views/deadline_listview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/views/manage_deadline_view.py` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/views/manage_deadline_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/views/multiselect_groups_view.py` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/views/multiselect_groups_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_deadlinemanagement/views/viewutils.py` & `devilry-6.3.0rc2/devilry/devilry_deadlinemanagement/views/viewutils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_detektor/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/devilry_detektor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_detektor/migrations/0002_auto_20180119_1137.py` & `devilry-6.3.0rc2/devilry/devilry_detektor/migrations/0002_auto_20180119_1137.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_developemail/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/devilry_developemail/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/utils.py` & `devilry-6.3.0rc2/devilry/devilry_email/utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/comment_email/comment_email.py` & `devilry-6.3.0rc2/devilry/devilry_email/comment_email/comment_email.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/deadline_email/deadline_email.py` & `devilry-6.3.0rc2/devilry/devilry_email/deadline_email/deadline_email.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/feedback_email/feedback_email.py` & `devilry-6.3.0rc2/devilry/devilry_email/feedback_email/feedback_email.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/groupinvite_email/groupinvite_email.py` & `devilry-6.3.0rc2/devilry/devilry_email/groupinvite_email/groupinvite_email.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/management/commands/devilry_send_testemail.py` & `devilry-6.3.0rc2/devilry/devilry_email/management/commands/devilry_send_testemail.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/templates/devilry_email/comment_email/comment.txt` & `devilry-6.3.0rc2/devilry/devilry_email/templates/devilry_email/comment_email/comment.txt`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/templates/devilry_email/deadline_email/deadline_moved.txt` & `devilry-6.3.0rc2/devilry/devilry_email/templates/devilry_email/deadline_email/deadline_moved.txt`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/templates/devilry_email/deadline_email/new_attempt.txt` & `devilry-6.3.0rc2/devilry/devilry_email/templates/devilry_email/deadline_email/new_attempt.txt`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/templates/devilry_email/feedback_email/assignment_feedback_student.txt` & `devilry-6.3.0rc2/devilry/devilry_email/templates/devilry_email/feedback_email/assignment_feedback_student.txt`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/templatetags/comment_email_tags.py` & `devilry-6.3.0rc2/devilry/devilry_email/templatetags/comment_email_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/tests/test_bulk_feedback.py` & `devilry-6.3.0rc2/devilry/devilry_email/tests/test_bulk_feedback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/tests/test_comment_email.py` & `devilry-6.3.0rc2/devilry/devilry_email/tests/test_comment_email.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/tests/test_deadline_email.py` & `devilry-6.3.0rc2/devilry/devilry_email/tests/test_deadline_email.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_email/tests/test_feedback_email.py` & `devilry-6.3.0rc2/devilry/devilry_email/tests/test_feedback_email.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/apps.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tasks.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tasks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/urls.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/cradminextensions/devilry_crmenu_examiner.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/cradminextensions/devilry_crmenu_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_create_feedback.django.html` & `devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_create_feedback.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_new_attempt.django.html` & `devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_new_attempt.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/grouplist.django.html` & `devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/grouplist.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/includes/batchdownload_assignment.django.html` & `devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/includes/batchdownload_assignment.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/grade_cell_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/grade_cell_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/simple_group_bulk_feedbackview.django.html` & `devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/simple_group_bulk_feedbackview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/dashboard/assignmentlist.django.html` & `devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/dashboard/assignmentlist.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign-group-item-value.django.html` & `devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign-group-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign.django.html` & `devilry-6.3.0rc2/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/templatetags/devilry_examiner_tags.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/templatetags/devilry_examiner_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_assignment/test_batchdownload_api.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_assignment/test_batchdownload_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_assignment/test_batchframework_tasks.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_assignment/test_batchframework_tasks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback_simple.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback_simple.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_assignment/test_crinstance_assignment.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_assignment/test_crinstance_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_assignment/test_grouplist.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_assignment/test_grouplist.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_cradminextensions/test_devilry_crmenu_examiner.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_cradminextensions/test_devilry_crmenu_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_dashboard/test_assignmentlist.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_dashboard/test_assignmentlist.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_dashboard/test_crinstance_dashboard.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_dashboard/test_crinstance_dashboard.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_api.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_crinstance_selfassign.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_crinstance_selfassign.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_grouplist.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_grouplist.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_utils.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/crinstance_assignment.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/crinstance_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/grouplist.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/grouplist.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_manage_deadline.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_manage_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_operations_grouplist.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_operations_grouplist.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/download_files/batch_download_api.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/download_files/batch_download_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/assignment/download_files/download_archive.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/assignment/download_files/download_archive.py`

 * *Files 17% similar despite different names*

```diff
@@ -50,20 +50,22 @@
         if not zip_backend:
             raise Http404()
 
         self.add_assignment_groups(self.request.user, zip_backend, assignment)
         zip_backend.close()
 
         filewrapper = zip_backend.get_archive()
-        content_type = 'application/octet-stream'
+        content_type = 'application/zip'
 
         response = http.StreamingHttpResponse(
             filewrapper,
             content_type=content_type
         )
+        response.set_cookie('zipdownload', 'start', max_age=10)
+
         response['content-disposition'] = 'attachment; filename={}'.format(
             archive_name.encode('ascii', 'replace').decode()
         )
         if zip_backend.archive_size() > 0:
             response['content-length'] = zip_backend.archive_size()
 
         return response
```

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/dashboard/assignmentlist.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/dashboard/assignmentlist.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/dashboard/crinstance_dashboard.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/dashboard/crinstance_dashboard.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/selfassign/api.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/selfassign/api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/selfassign/crinstance_selfassign.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/selfassign/crinstance_selfassign.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/selfassign/selfassign.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/selfassign/selfassign.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_examiner/views/selfassign/utils.py` & `devilry-6.3.0rc2/devilry/devilry_examiner/views/selfassign/utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_frontpage/crinstance_frontpage.py` & `devilry-6.3.0rc2/devilry/devilry_frontpage/crinstance_frontpage.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_frontpage/cradminextensions/listbuilder/listbuilder_role.py` & `devilry-6.3.0rc2/devilry/devilry_frontpage/cradminextensions/listbuilder/listbuilder_role.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_frontpage/templates/devilry_frontpage/frontpage.django.html` & `devilry-6.3.0rc2/devilry/devilry_frontpage/templates/devilry_frontpage/frontpage.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_frontpage/tests/test_frontpage.py` & `devilry-6.3.0rc2/devilry/devilry_frontpage/tests/test_frontpage.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_frontpage/tests/test_cradminextensions/test_listbuilder_role.py` & `devilry-6.3.0rc2/devilry/devilry_frontpage/tests/test_cradminextensions/test_listbuilder_role.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_frontpage/views/frontpage.py` & `devilry-6.3.0rc2/devilry/devilry_frontpage/views/frontpage.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradeform/templates/devilry_gradeform/setup.gradeform.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradeform/templates/devilry_gradeform/setup.gradeform.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradeform/views/editable_gradeform.py` & `devilry-6.3.0rc2/devilry/devilry_gradeform/views/editable_gradeform.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradeform/views/grade_form.py` & `devilry-6.3.0rc2/devilry/devilry_gradeform/views/grade_form.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradeform/views/setup_create_gradeform.py` & `devilry-6.3.0rc2/devilry/devilry_gradeform/views/setup_create_gradeform.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradeform/views/setup_gradeform.py` & `devilry-6.3.0rc2/devilry/devilry_gradeform/views/setup_gradeform.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradeform/views/viewable_gradeform.py` & `devilry-6.3.0rc2/devilry/devilry_gradeform/views/viewable_gradeform.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/models.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/pluginregistry.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/pluginregistry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/urls.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/migrations/0002_auto_20170108_0948.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/migrations/0002_auto_20170108_0948.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/bulkeditfeedbackbuttonbar.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/bulkeditfeedbackbuttonbar.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/editfeedbackbuttonbar.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/editfeedbackbuttonbar.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackbulkeditorbase.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackbulkeditorbase.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_bulkpreview.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_bulkpreview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_preview.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_preview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/base.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/currentprogress.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/currentprogress.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/select_points_to_grade_mapper.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/select_points_to_grade_mapper.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/selectplugin.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/selectplugin.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setmaxpoints.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setmaxpoints.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setpassing_grade_min_points.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setpassing_grade_min_points.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setup_custom_table.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setup_custom_table.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/summary.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/summary.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/editmarkdown.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/editmarkdown.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/feedbackeditorfilewidget.django.html` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/feedbackeditorfilewidget.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/helpers.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/test_models.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/test_download_feedbackdraftfile.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/test_download_feedbackdraftfile.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/test_feedbackdraft_preview.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/test_feedbackdraft_preview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/base.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_select_points_to_grade_mapper.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_select_points_to_grade_mapper.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_selectplugin.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_selectplugin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_setmaxpoints.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_setmaxpoints.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_setpassing_grade_min_points.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_setpassing_grade_min_points.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_setup_custom_table.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_setup_custom_table.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_summary.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_summary.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/download_feedbackdraftfile.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/download_feedbackdraftfile.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/feedbackbulkeditorbase.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/feedbackbulkeditorbase.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/feedbackdraft_bulkpreview.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/feedbackdraft_bulkpreview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/feedbackdraft_preview.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/feedbackdraft_preview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/feedbackeditorbase.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/feedbackeditorbase.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/base.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/select_points_to_grade_mapper.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/select_points_to_grade_mapper.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/selectplugin.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/selectplugin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/setmaxpoints.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/setmaxpoints.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/setpassing_grade_min_points.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/setpassing_grade_min_points.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/setup_custom_table.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/setup_custom_table.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/views/admin/summary.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/views/admin/summary.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/widgets/editmarkdown.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/widgets/editmarkdown.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystem/widgets/filewidget.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystem/widgets/filewidget.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_approved/apps.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_approved/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_approved/views/feedbackeditor.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_approved/views/feedbackeditor.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_points/apps.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_points/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_gradingsystemplugin_points/views/feedbackeditor.py` & `devilry-6.3.0rc2/devilry/devilry_gradingsystemplugin_points/views/feedbackeditor.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/admin.py` & `devilry-6.3.0rc2/devilry/devilry_group/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/apps.py` & `devilry-6.3.0rc2/devilry/devilry_group/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/devilry_group_baker_factories.py` & `devilry-6.3.0rc2/devilry/devilry_group/devilry_group_baker_factories.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/models.py` & `devilry-6.3.0rc2/devilry/devilry_group/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tasks.py` & `devilry-6.3.0rc2/devilry/devilry_group/tasks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/urls.py` & `devilry-6.3.0rc2/devilry/devilry_group/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/cradmin_instances/crinstance_admin.py` & `devilry-6.3.0rc2/devilry/devilry_group/cradmin_instances/crinstance_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/cradmin_instances/crinstance_base.py` & `devilry-6.3.0rc2/devilry/devilry_group/cradmin_instances/crinstance_base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/cradmin_instances/crinstance_examiner.py` & `devilry-6.3.0rc2/devilry/devilry_group/cradmin_instances/crinstance_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/cradmin_instances/crinstance_student.py` & `devilry-6.3.0rc2/devilry/devilry_group/cradmin_instances/crinstance_student.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/feedbackfeed_builder/builder_base.py` & `devilry-6.3.0rc2/devilry/devilry_group/feedbackfeed_builder/builder_base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_sidebarbuilder.py` & `devilry-6.3.0rc2/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_sidebarbuilder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_timelinebuilder.py` & `devilry-6.3.0rc2/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_timelinebuilder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0003_auto_20160106_1418.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0003_auto_20160106_1418.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0004_auto_20160107_0918.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0004_auto_20160107_0918.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0007_auto_20160107_1031.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0007_auto_20160107_1031.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0008_auto_20160107_1053.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0008_auto_20160107_1053.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0009_auto_20160107_1100.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0009_auto_20160107_1100.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0010_auto_20160107_1106.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0010_auto_20160107_1106.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0011_auto_20160107_1111.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0011_auto_20160107_1111.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0012_auto_20160107_1129.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0012_auto_20160107_1129.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0013_auto_20160110_1621.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0013_auto_20160110_1621.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0014_feedbackset_grading_status.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0014_feedbackset_grading_status.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0015_auto_20160111_1245.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0015_auto_20160111_1245.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0016_auto_20160114_2202.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0016_auto_20160114_2202.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0017_auto_20160122_1518.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0017_auto_20160122_1518.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0019_auto_20160822_1945.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0019_auto_20160822_1945.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0019_auto_20160912_1649.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0019_auto_20160912_1649.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0023_auto_20170104_0551.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0023_auto_20170104_0551.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0024_auto_20170107_1838.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0024_auto_20170107_1838.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0025_auto_20170124_1504.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0025_auto_20170124_1504.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0026_datamigrate_update_for_no_none_values_in_feedbackset_deadline.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0026_datamigrate_update_for_no_none_values_in_feedbackset_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0027_auto_20170206_1146.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0027_auto_20170206_1146.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0027_auto_20170207_1951.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0027_auto_20170207_1951.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0030_auto_20170621_1734.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0030_auto_20170621_1734.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0032_auto_20180214_1654.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0032_auto_20180214_1654.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0033_feedbacksetgradingupdatehistory.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0033_feedbacksetgradingupdatehistory.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0034_feedbackset_last_updated_by.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0034_feedbackset_last_updated_by.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/migrations/0035_groupcommentedithistory.py` & `devilry-6.3.0rc2/devilry/devilry_group/migrations/0035_groupcommentedithistory.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_guidelines.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_guidelines.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/group_comment_edit_base.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/group_comment_edit_base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_base.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_base.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/group_comment_history/comment_history.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/group_comment_history/comment_history.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/group_comment_history/history_item_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/group_comment_history/history_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/batch_download_archive_script.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/batch_download_archive_script.django.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 {% load devilry_group_tags %}
 {% load cradmin_legacy_tags %}
 {% load i18n %}
 
 <script type="module">
-    class CSRFToken {
+    class Cookies {
         constructor () {
             this.csrftoken = this._getCookie('csrftoken');
+            this.zipdownload = this._getCookie('zipdownload');
         }
 
         _getCookie(name) {
             let cookieValue = null;
             if (document.cookie && document.cookie !== '') {
                 const cookies = document.cookie.split(';');
                 for (let i = 0; i < cookies.length; i++) {
@@ -111,27 +112,27 @@
                     <p>ERROR</p>
                 </div>
             `, 'text/html').body.firstChild;
             this._removeCurrentDownloadElementNode();
             this.appendChild(errorWarning);
         }
 
-        _handleArchiveNotCreated () {            
+        _handleArchiveNotCreated () {
             const button = new DOMParser().parseFromString(`
                 <button id=${this.rootElementId} class="btn btn-default" type="button" aria-label="${this.ariaLabelArchiveBuildStart}">
                     ${this.startDownloadText}
                 </button>
             `, 'text/html').body.firstChild;
 
             button.addEventListener('click', (e) => {
                 fetch(this.apiUrl, {
                     method: 'POST',
                     headers: {
                         'Content-Type': 'application/json',
-                        'X-CSRFToken': new CSRFToken().csrftoken
+                        'X-CSRFToken': new Cookies().csrftoken
                     }
                 })
                 .then(response => response.json())
                 .then((responseData) => {
                     this.finishedWithinSameSession = true;
                     this._handleApiResponse(responseData);
                 })
@@ -155,23 +156,44 @@
             `, 'text/html').body.firstChild;
             this._removeCurrentDownloadElementNode();
             this.appendChild(progressNodeElement);
         }
 
         _handleArchiveReadyForDownload (downloadUrl) {
             const downloadLink = new DOMParser().parseFromString(`
-                <a 
+                <a
                     id="${this.rootElementId}"
-                    href="${downloadUrl}"
                     aria-label="${this.finishedWithinSameSession ? this.ariaLabelArchiveBuildCompleted : this.ariaLabelArchiveBuildDownload}"
                     class="btn btn-default"
                 >
-                    ${this.downloadArchiveText}
+                    <span id="${this.rootElementId}_text">
+                        ${this.downloadArchiveText}
+                    </span>
+                    <span id="${this.rootElementId}_spinner" class="hidden fa fa-spinner fa-spin" aria-hidden="true"></span>
                 </a>
             `, 'text/html').body.firstChild;
+            downloadLink.addEventListener('click', (e) => {
+                const text = document.getElementById(this.rootElementId + "_text")
+                const spinner = document.getElementById(this.rootElementId + "_spinner")
+                text.classList.add('hidden');
+                spinner.classList.remove('hidden');
+                var downloadTimeout;
+                var checkDownloadCookie = function() {
+                    if (new Cookies().zipdownload) {
+                        text.classList.remove('hidden');
+                        spinner.classList.add('hidden');
+                    } else {
+                        downloadTimeout = window.setTimeout(checkDownloadCookie, 1000); //Re-run this function in 1 second.
+                    }
+                };
+                const dl = document.createElement('a');
+                dl.setAttribute('href', downloadUrl);
+                dl.click();
+                window.setTimeout(checkDownloadCookie, 1000);
+            });
             this._removeCurrentDownloadElementNode();
             this.appendChild(downloadLink);
         }
     }
 
     window.customElements.define('group-feedbackfeed-archivedownload', GroupFeedbackFeedArchiveDownload);
 </script>
```

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/buttonbar.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/buttonbar.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/examiner.editlastdelivery.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/examiner.editlastdelivery.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/groupcomment_edit_delete_option.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/groupcomment_edit_delete_option.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/include/student_commentform_headingtext.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/include/student_commentform_headingtext.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/admin_groupcomment_item_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/admin_groupcomment_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/base_groupcomment_item_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/base_groupcomment_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/deadline_moved_item_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/deadline_moved_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/examiner_groupcomment_item_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/examiner_groupcomment_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/feedbackset_info_item_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/feedbackset_info_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_item_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_updated_item_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_updated_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/student_groupcomment_item_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/student_groupcomment_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_comment_item_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_comment_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_feedbackset_item_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_feedbackset_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_file_item_value.django.html` & `devilry-6.3.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_file_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/templatetags/devilry_group_tags.py` & `devilry-6.3.0rc2/devilry/devilry_group/templatetags/devilry_group_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_devilry_group_mommy_factories.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_devilry_group_mommy_factories.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_templatetags.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_crinstance/test_crinstance_admin.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_crinstance/test_crinstance_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_crinstance/test_crinstance_examiner.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_crinstance/test_crinstance_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_crinstance/test_crinstance_student.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_crinstance/test_crinstance_student.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_download/test_batchdownload_api.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_download/test_batchdownload_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_download/test_batchframework_compression.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_download/test_batchframework_compression.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_download/test_feedbackfeed_bulkfiledownload.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_download/test_feedbackfeed_bulkfiledownload.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_download/test_feedbackfeed_filedownload.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_download/test_feedbackfeed_filedownload.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/admin/test_comment_edit_history.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/admin/test_comment_edit_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/admin/test_feedbackfeed_admin.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/admin/test_feedbackfeed_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_comment_edit_history.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_comment_edit_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_delete_comment.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_delete_comment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_discuss.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_discuss.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_comment.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_comment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_grade.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_grade.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_feedback.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_feedback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_admin.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_common.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_common.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_examiner.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/student/test_comment_edit_history.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/student/test_comment_edit_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed/student/test_feedbackfeed_student.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed/student/test_feedbackfeed_student.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_sidebarbuilder.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_sidebarbuilder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_timeline_builder.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_timeline_builder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_models/test_feedback_set.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_models/test_feedback_set.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_models/test_feedbackfeed_model.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_models/test_feedbackfeed_model.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_models/test_feedbackset_passed_pervious_period.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_models/test_feedbackset_passed_pervious_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/tests/test_models/test_group_comment.py` & `devilry-6.3.0rc2/devilry/devilry_group/tests/test_models/test_group_comment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/utils/download_response.py` & `devilry-6.3.0rc2/devilry/devilry_group/utils/download_response.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/cradmin_comment_history.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/cradmin_comment_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/cradmin_feedbackfeed_base.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/cradmin_feedbackfeed_base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/group_comment_edit_base.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/group_comment_edit_base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/admin/feedbackfeed_admin.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/admin/feedbackfeed_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/admin/group_comment_history.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/admin/group_comment_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/admin/manage_deadline.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/admin/manage_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/download_files/backends.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/download_files/backends.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/download_files/batch_download_api.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/download_files/batch_download_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/download_files/batch_download_files.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/download_files/batch_download_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # -*- coding: utf-8 -*-
 from wsgiref.util import FileWrapper
 import re
 import os
 
 from django import http
-from django.contrib.contenttypes.models import ContentType
-from django.http import Http404, HttpResponse
+from django.http import Http404
 from django.shortcuts import get_object_or_404
 from django.views import generic
 from cradmin_legacy import crapp
 
 from devilry.devilry_comment import models as comment_models
-from devilry.devilry_compressionutil import models as archivemodels
 from devilry.devilry_group import models as group_models
-from devilry.devilry_group.utils import download_response
 from devilry.devilry_group.views.download_files.batch_download_api import BatchCompressionAPIFeedbackSetView
 from devilry.devilry_compressionutil.backend_registry import Registry
 from devilry.devilry_compressionutil.batchjob_mixins.feedbackset_mixin import FeedbackSetBatchMixin
 
 
 
 
@@ -73,15 +70,16 @@
 
         Returns:
             Response: redirects to wait-for-download view,
                 see :class:`~devilry.devilry_group.views.download_files.feedbackfeed_downloadviews.WaitForDownload`, or
                 returns the content, see `~devilry.devilry_group.utils.download_response`.
         """
         feedbackset_id = kwargs.get('feedbackset_id')
-        feedbackset = get_object_or_404(group_models.FeedbackSet, id=feedbackset_id)
+
+        feedbackset = get_object_or_404(self.get_feedbackset_queryset(), id=feedbackset_id)
 
         # Check that the cradmin role and the AssignmentGroup is the same.
         if feedbackset.group.id != request.cradmin_role.id:
             raise Http404()
 
         from django.utils import timezone
         archive_name = 'feedbackset-{}-{}-delivery.zip'.format(
@@ -102,20 +100,22 @@
         if not zip_backend:
             raise Http404()
 
         self.zipfile_add_feedbackset(zipfile_backend=zip_backend, feedback_set=feedbackset)
         zip_backend.close()
 
         filewrapper = zip_backend.get_archive()
-        content_type = 'application/octet-stream'
+        content_type = 'application/zip'
 
         response = http.StreamingHttpResponse(
             filewrapper,
             content_type=content_type
         )
+        response.set_cookie('zipdownload', 'start', max_age=10)
+
         response['content-disposition'] = 'attachment; filename={}'.format(
             archive_name.encode('ascii', 'replace').decode()
         )
         if zip_backend.archive_size() > 0:
             response['content-length'] = zip_backend.archive_size()
 
         return response
```

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/download_files/feedbackfeed_bulkfiledownload.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/download_files/feedbackfeed_bulkfiledownload.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/examiner/feedbackfeed_examiner.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/examiner/feedbackfeed_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/examiner/group_comment_history.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/examiner/group_comment_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/examiner/manage_deadline.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/examiner/manage_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/student/feedbackfeed_student.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/student/feedbackfeed_student.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_group/views/student/group_comment_history.py` & `devilry-6.3.0rc2/devilry/devilry_group/views/student/group_comment_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_header/templates/devilry_header/about_me.django.html` & `devilry-6.3.0rc2/devilry/devilry_header/templates/devilry_header/about_me.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_header/templates/devilry_header/header2include.django.html` & `devilry-6.3.0rc2/devilry/devilry_header/templates/devilry_header/header2include.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_header/templates/devilry_header/includes/change_language.django.html` & `devilry-6.3.0rc2/devilry/devilry_header/templates/devilry_header/includes/change_language.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_header/tests/test_aboutme.py` & `devilry-6.3.0rc2/devilry/devilry_header/tests/test_aboutme.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_header/tests/test_change_language.py` & `devilry-6.3.0rc2/devilry/devilry_header/tests/test_change_language.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_header/views/about_me.py` & `devilry-6.3.0rc2/devilry/devilry_header/views/about_me.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_header/views/change_language.py` & `devilry-6.3.0rc2/devilry/devilry_header/views/change_language.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_help/tests.py` & `devilry-6.3.0rc2/devilry/devilry_help/tests.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_help/views.py` & `devilry-6.3.0rc2/devilry/devilry_help/views.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_help/templates/devilry_help/help.django.html` & `devilry-6.3.0rc2/devilry/devilry_help/templates/devilry_help/help.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_i18n/middleware.py` & `devilry-6.3.0rc2/devilry/devilry_i18n/middleware.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/models.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparser.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/management/commands/devilry_import_v2_database.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/management/commands/devilry_import_v2_database.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/__init__.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/__init__.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/assignment_importer.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/assignment_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/assignmentgroup_importer.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/assignmentgroup_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/candidate_examiner_importer.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/candidate_examiner_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/delivery_feedback_importers.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/delivery_feedback_importers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/feedbackset_importer.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/feedbackset_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/modelimporter_utils.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/modelimporter_utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/node_importer.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/node_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/period_importer.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/period_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/pointrange_to_grade_importer.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/pointrange_to_grade_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/qualifiesforexam_importer.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/qualifiesforexam_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/relateduser_importer.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/relateduser_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/subject_importer.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/subject_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/modelimporters/user_importer.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/modelimporters/user_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/scripts/user_add_missing_data_from_json.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/scripts/user_add_missing_data_from_json.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/importer_testcase_mixin.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/importer_testcase_mixin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentgroupimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentgroupimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_candidateimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_candidateimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_commentfilecontentimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_commentfilecontentimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_deliveryimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_deliveryimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_examinerimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_examinerimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_feedbacksetimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_feedbacksetimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_filemetaimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_filemetaimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_nodeimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_nodeimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_periodimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_periodimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointrangetogradeimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointrangetogradeimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointtogrademapimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointtogrademapimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_qualifiesforexam_importer.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_qualifiesforexam_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedexaminerimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedexaminerimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedstudentimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedstudentimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_staticfeedbackimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_staticfeedbackimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_subjectimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_subjectimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_userimporter.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_userimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/tests/test_scripts/test_user_add_missing_data_from_json.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/tests/test_scripts/test_user_add_missing_data_from_json.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/__init__.py` & `devilry-6.3.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/__init__.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_markup/parse_markdown.py` & `devilry-6.3.0rc2/devilry/devilry_markup/parse_markdown.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_markup/views.py` & `devilry-6.3.0rc2/devilry/devilry_markup/views.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_markup/markdown_extensions/code_diff.py` & `devilry-6.3.0rc2/devilry/devilry_markup/markdown_extensions/code_diff.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_markup/markdown_extensions/latex_math.py` & `devilry-6.3.0rc2/devilry/devilry_markup/markdown_extensions/latex_math.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_markup/templates/devilry_markup/code_diff.html` & `devilry-6.3.0rc2/devilry/devilry_markup/templates/devilry_markup/code_diff.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_message/admin.py` & `devilry-6.3.0rc2/devilry/devilry_message/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_message/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/devilry_message/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_message/migrations/0002_auto_20210427_1350.py` & `devilry-6.3.0rc2/devilry/devilry_message/migrations/0002_auto_20210427_1350.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_message/migrations/0003_alter_message_context_type.py` & `devilry-6.3.0rc2/devilry/devilry_message/migrations/0003_alter_message_context_type.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_message/models/base.py` & `devilry-6.3.0rc2/devilry/devilry_message/models/base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_message/tests/test_message.py` & `devilry-6.3.0rc2/devilry/devilry_message/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_message/tests/test_message_receiver.py` & `devilry-6.3.0rc2/devilry/devilry_message/tests/test_message_receiver.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/admin.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/apps.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/cradmin_app.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/cradmin_app.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/models.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/pluginhelpers.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/pluginhelpers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/plugintyperegistry.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/plugintyperegistry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/listbuilder/assignment_listbuilder_list.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/listbuilder/assignment_listbuilder_list.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/listbuilder/plugin_listbuilder_list.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/listbuilder/plugin_listbuilder_list.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/migrations/0002_auto_20170223_1112.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/migrations/0002_auto_20170223_1112.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/migrations/0005_deletedqualifiesforfinalexam.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/migrations/0005_deletedqualifiesforfinalexam.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tablebuilder/tablebuilder.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tablebuilder/tablebuilder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/base.django.html` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/list_statuses.django.html` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/list_statuses.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/print_view.html` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/print_view.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/retract_status.django.html` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/retract_status.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/selectplugin.django.html` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/selectplugin.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_preview.django.html` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_preview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_show.html` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_show.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/includes/qualification_table.django.html` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/includes/qualification_table.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/description.django.html` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/description.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_list_statuses_view.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_list_statuses_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_models.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_plugin_listbuilder_list.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_plugin_listbuilder_list.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_pluginhelpers.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_pluginhelpers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_pluginselection_view.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_pluginselection_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_plugintyperegistry.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_plugintyperegistry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_preview.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_preview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/tests/test_showstatus.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/tests/test_showstatus.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/utils/groups_groupedby_relatedstudent_and_assignments.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/utils/groups_groupedby_relatedstudent_and_assignments.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/views/list_statuses_view.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/views/list_statuses_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/views/pluginselection_view.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/views/pluginselection_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/views/proxyview.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/views/proxyview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/views/qualification_preview_view.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/views/qualification_preview_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam/views/plugin_base_views/base_multiselect_view.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam/views/plugin_base_views/base_multiselect_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/plugin.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/plugin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/resultscollector.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/resultscollector.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/tests/test_resultscollector.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/tests/test_resultscollector.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/views/select_assignment.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/views/select_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_points/plugin.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_points/plugin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_points/resultscollector.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_points/resultscollector.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_points/tests/test_resultscollector.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_points/tests/test_resultscollector.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_points/views/select_assignment_and_points.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_points/views/select_assignment_and_points.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_students/plugin.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_students/plugin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_students/tests/test_student_selection_view.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_students/tests/test_student_selection_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_qualifiesforexam_plugin_students/views/select_students.py` & `devilry-6.3.0rc2/devilry/devilry_qualifiesforexam_plugin_students/views/select_students.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_report/abstract_generator.py` & `devilry-6.3.0rc2/devilry/devilry_report/abstract_generator.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_report/admin.py` & `devilry-6.3.0rc2/devilry/devilry_report/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_report/generator_registry.py` & `devilry-6.3.0rc2/devilry/devilry_report/generator_registry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_report/models.py` & `devilry-6.3.0rc2/devilry/devilry_report/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_report/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/devilry_report/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_report/migrations/0002_auto_20210427_1350.py` & `devilry-6.3.0rc2/devilry/devilry_report/migrations/0002_auto_20210427_1350.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_report/templates/devilry_report/download_report.django.html` & `devilry-6.3.0rc2/devilry/devilry_report/templates/devilry_report/download_report.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_report/tests/test_download_report_view.py` & `devilry-6.3.0rc2/devilry/devilry_report/tests/test_download_report_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_report/tests/test_generator_registry.py` & `devilry-6.3.0rc2/devilry/devilry_report/tests/test_generator_registry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_report/tests/test_report_model.py` & `devilry-6.3.0rc2/devilry/devilry_report/tests/test_report_model.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_report/views/download_report.py` & `devilry-6.3.0rc2/devilry/devilry_report/views/download_report.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_resetpassword/urls.py` & `devilry-6.3.0rc2/devilry/devilry_resetpassword/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_rest/auth.py` & `devilry-6.3.0rc2/devilry/devilry_rest/auth.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_rest/formfields.py` & `devilry-6.3.0rc2/devilry/devilry_rest/formfields.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_rest/serializehelpers.py` & `devilry-6.3.0rc2/devilry/devilry_rest/serializehelpers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_rest/testclient.py` & `devilry-6.3.0rc2/devilry/devilry_rest/testclient.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_rest/tests/test_serializehelpers.py` & `devilry-6.3.0rc2/devilry/devilry_rest/tests/test_serializehelpers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_sandbox/sandbox.py` & `devilry-6.3.0rc2/devilry/devilry_sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_sandbox/urls.py` & `devilry-6.3.0rc2/devilry/devilry_sandbox/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_sandbox/views.py` & `devilry-6.3.0rc2/devilry/devilry_sandbox/views.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_sandbox/management/commands/devilry_sandboxcreate.py` & `devilry-6.3.0rc2/devilry/devilry_sandbox/management/commands/devilry_sandboxcreate.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_sandbox/templates/devilry_sandbox/createsubject.django.html` & `devilry-6.3.0rc2/devilry/devilry_sandbox/templates/devilry_sandbox/createsubject.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_settings/views.py` & `devilry-6.3.0rc2/devilry/devilry_settings/views.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/urls.py` & `devilry-6.3.0rc2/devilry/devilry_statistics/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/api/assignment/api_utils.py` & `devilry-6.3.0rc2/devilry/devilry_statistics/api/assignment/api_utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/api/assignment/examiner_average_grading_points.py` & `devilry-6.3.0rc2/devilry/devilry_statistics/api/assignment/examiner_average_grading_points.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/api/assignment/examiner_details.py` & `devilry-6.3.0rc2/devilry/devilry_statistics/api/assignment/examiner_details.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/api/assignment/examiner_group_results.py` & `devilry-6.3.0rc2/devilry/devilry_statistics/api/assignment/examiner_group_results.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/management/commands/devilry_create_test_course.py` & `devilry-6.3.0rc2/devilry/devilry_statistics/management/commands/devilry_create_test_course.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/management/commands/devilry_statistics_make_assignment_with_graded_groups.py` & `devilry-6.3.0rc2/devilry/devilry_statistics/management/commands/devilry_statistics_make_assignment_with_graded_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/static/devilry_statistics/6.3.0rc1/devilry_statistics_all.js` & `devilry-6.3.0rc2/devilry/devilry_statistics/static/devilry_statistics/6.3.0rc2/devilry_statistics_all.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/package-lock.json` & `devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/package-lock.json`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/package.json` & `devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/package.json`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/devilry_statistics_all.js` & `devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/devilry_statistics_all.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerAverageGradingPointsWidget.js` & `devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerAverageGradingPointsWidget.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerDetailsWidget.js` & `devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerDetailsWidget.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerGroupResultWidget.js` & `devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerGroupResultWidget.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/registerAllWidgets.js` & `devilry-6.3.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/registerAllWidgets.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/tests/test_api_examiner_average_grading_points.py` & `devilry-6.3.0rc2/devilry/devilry_statistics/tests/test_api_examiner_average_grading_points.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/tests/test_api_examiner_details.py` & `devilry-6.3.0rc2/devilry/devilry_statistics/tests/test_api_examiner_details.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_statistics/tests/test_api_examiner_group_result.py` & `devilry-6.3.0rc2/devilry/devilry_statistics/tests/test_api_examiner_group_result.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/models.py` & `devilry-6.3.0rc2/devilry/devilry_student/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/urls.py` & `devilry-6.3.0rc2/devilry/devilry_student/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/cradminextensions/columntypes.py` & `devilry-6.3.0rc2/devilry/devilry_student/cradminextensions/columntypes.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/cradminextensions/devilry_crmenu_student.py` & `devilry-6.3.0rc2/devilry/devilry_student/cradminextensions/devilry_crmenu_student.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/migrations/0001_initial.py` & `devilry-6.3.0rc2/devilry/devilry_student/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html` & `devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/add_delivery.django.html` & `devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/add_delivery.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/contactapp/contact.django.html` & `devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/contactapp/contact.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery-status-column.django.html` & `devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery-status-column.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_details.django.html` & `devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_details.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_list.django.html` & `devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_list.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/overviewapp/overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/overviewapp/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_delete.django.html` & `devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_delete.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond.django.html` & `devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond_standalone.django.html` & `devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond_standalone.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/projectgroup_overview.django.html` & `devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/projectgroup_overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/delivery-summary-column.django.html` & `devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/delivery-summary-column.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templates/devilry_student/dashboard/dashboard.django.html` & `devilry-6.3.0rc2/devilry/devilry_student/templates/devilry_student/dashboard/dashboard.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/templatetags/devilry_student_tags.py` & `devilry-6.3.0rc2/devilry/devilry_student/templatetags/devilry_student_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/tests/test_models.py` & `devilry-6.3.0rc2/devilry/devilry_student/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/tests/test_templatetags.py` & `devilry-6.3.0rc2/devilry/devilry_student/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/tests/test_cradminextensions/test_devilry_crmenu_student.py` & `devilry-6.3.0rc2/devilry/devilry_student/tests/test_cradminextensions/test_devilry_crmenu_student.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/tests/test_dashboard/test_allperiods.py` & `devilry-6.3.0rc2/devilry/devilry_student/tests/test_dashboard/test_allperiods.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/tests/test_dashboard/test_dashboard.py` & `devilry-6.3.0rc2/devilry/devilry_student/tests/test_dashboard/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/tests/test_group/test_projectgroupapp.py` & `devilry-6.3.0rc2/devilry/devilry_student/tests/test_group/test_projectgroupapp.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/tests/test_period/test_overview.py` & `devilry-6.3.0rc2/devilry/devilry_student/tests/test_period/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/views/show_delivery.py` & `devilry-6.3.0rc2/devilry/devilry_student/views/show_delivery.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/views/dashboard/allperiods.py` & `devilry-6.3.0rc2/devilry/devilry_student/views/dashboard/allperiods.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/views/dashboard/crinstance_dashboard.py` & `devilry-6.3.0rc2/devilry/devilry_student/views/dashboard/crinstance_dashboard.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/views/dashboard/dashboard.py` & `devilry-6.3.0rc2/devilry/devilry_student/views/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/views/group/projectgroupapp.py` & `devilry-6.3.0rc2/devilry/devilry_student/views/group/projectgroupapp.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/views/period/crinstance_period.py` & `devilry-6.3.0rc2/devilry/devilry_student/views/period/crinstance_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_student/views/period/overview.py` & `devilry-6.3.0rc2/devilry/devilry_student/views/period/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/delete_periods/period_delete.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/delete_periods/period_delete.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/examples/relatedstudents_email_instead_of_username.json` & `devilry-6.3.0rc2/devilry/devilry_superadmin/examples/relatedstudents_email_instead_of_username.json`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_anonymize_database.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_anonymize_database.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_compressed_archives.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_compressed_archives.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_inactive_users.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_inactive_users.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_message_receivers.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_message_receivers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_messages_without_receivers.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_messages_without_receivers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_periods.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_periods.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_fix_missing_first_feedbackset.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_fix_missing_first_feedbackset.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_mark_as_passed_in_previous_period.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_mark_as_passed_in_previous_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodadd.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodadminadd.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodadminadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodadminclear.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodadminclear.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodsearch.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodsearch.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedexaminers.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedexaminers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedstudents.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedstudents.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_permissiongroup_add_subject.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_permissiongroup_add_subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_qualifiedforfinalexam_delete_duplicates.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_qualifiedforfinalexam_delete_duplicates.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_rename_periodtag_prefix.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_rename_periodtag_prefix.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_resend_failed_messages.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_resend_failed_messages.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_setup_dataporten_provider.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_setup_dataporten_provider.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_setup_primary_domain.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_setup_primary_domain.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_show_assignment_guidelines.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_show_assignment_guidelines.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectadd.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectadminadd.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectadminadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectadminclear.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectadminclear.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectsearch.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectsearch.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_test_rq_task.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_test_rq_task.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_useradd.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_useradd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_useraddbulk.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_useraddbulk.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_usermerge.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_usermerge.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/management/commands/devilry_usermod.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/management/commands/devilry_usermod.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_inactive_users.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_inactive_users.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_periods.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_periods.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminadd.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminclear.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminclear.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_permissiongroup_add_subject.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_permissiongroup_add_subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_qualifiedforfinalexam_delete_duplicates.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_qualifiedforfinalexam_delete_duplicates.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadd.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminadd.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminclear.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminclear.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_useraddbulk.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_useraddbulk.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_usermod.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_usermod.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_resend_failed_messages.py` & `devilry-6.3.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_resend_failed_messages.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/media/images/groovepaper.png` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/media/images/groovepaper.png`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/media/images/favicons/apple-touch-icon.png` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/media/images/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/media/images/favicons/favicon.ico` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/media/images/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/devilry_all.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/devilry_all.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/devilry_all.js.map` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/devilry_all.js.map`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/LICENSE` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/LICENSE`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/katex.min.css` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/katex.min.css`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/katex.mjs` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/katex.mjs`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/auto-render.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/auto-render.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/auto-render.min.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/auto-render.min.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/auto-render.mjs` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/auto-render.mjs`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/copy-tex.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/copy-tex.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/copy-tex.min.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/copy-tex.min.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/copy-tex.mjs` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/copy-tex.mjs`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/mathtex-script-type.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/mathtex-script-type.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/mathtex-script-type.min.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/mathtex-script-type.min.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/mathtex-script-type.mjs` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/mathtex-script-type.mjs`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/mhchem.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/mhchem.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/mhchem.min.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/mhchem.min.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/mhchem.mjs` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/mhchem.mjs`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/render-a11y-string.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/render-a11y-string.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/render-a11y-string.min.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/render-a11y-string.min.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/contrib/render-a11y-string.mjs` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/contrib/render-a11y-string.mjs`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_AMS-Regular.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_AMS-Regular.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_AMS-Regular.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_AMS-Regular.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_AMS-Regular.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Caligraphic-Bold.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Caligraphic-Bold.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Caligraphic-Bold.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Caligraphic-Bold.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Caligraphic-Regular.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Caligraphic-Regular.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Caligraphic-Regular.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Caligraphic-Regular.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Fraktur-Bold.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Fraktur-Bold.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Fraktur-Bold.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Fraktur-Bold.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Fraktur-Regular.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Fraktur-Regular.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Fraktur-Regular.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Fraktur-Regular.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Bold.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Bold.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Bold.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Bold.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-BoldItalic.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-BoldItalic.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-BoldItalic.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Italic.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Italic.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Italic.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Italic.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Regular.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Regular.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Regular.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Main-Regular.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Math-BoldItalic.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Math-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Math-BoldItalic.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Math-BoldItalic.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Math-Italic.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Math-Italic.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Math-Italic.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Math-Italic.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Bold.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Bold.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Bold.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Bold.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Italic.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Italic.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Italic.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Italic.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Regular.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Regular.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Regular.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_SansSerif-Regular.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Script-Regular.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Script-Regular.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Script-Regular.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Script-Regular.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size1-Regular.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size1-Regular.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size1-Regular.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size1-Regular.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size2-Regular.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size2-Regular.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size2-Regular.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size2-Regular.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size3-Regular.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size3-Regular.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size3-Regular.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size3-Regular.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size4-Regular.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size4-Regular.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size4-Regular.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Size4-Regular.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Typewriter-Regular.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Typewriter-Regular.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Typewriter-Regular.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/katex/fonts/KaTeX_Typewriter-Regular.woff2` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/katex/fonts/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/commentEditor.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/commentEditor.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/cookie.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/cookie.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/examinerSelfAssignButton.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/examinerSelfAssignButton.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/feedbackfeedNavigationHandler.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/feedbackfeedNavigationHandler.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/fileupload.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/fileupload.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/scripts/plain_es6/latex_math.js` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/scripts/plain_es6/latex_math.js`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/styles/cradmin_theme_devilry_mainpages/theme.css` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/styles/cradmin_theme_devilry_mainpages/theme.css`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/styles/cradmin_theme_devilry_superuserui/theme.css` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/styles/cradmin_theme_devilry_superuserui/theme.css`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/vendor/fonts/glyphicons/glyphicons-halflings-regular.eot` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/vendor/fonts/glyphicons/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/vendor/fonts/glyphicons/glyphicons-halflings-regular.svg` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/vendor/fonts/glyphicons/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/vendor/fonts/glyphicons/glyphicons-halflings-regular.ttf` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/vendor/fonts/glyphicons/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc1/vendor/fonts/glyphicons/glyphicons-halflings-regular.woff` & `devilry-6.3.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.3.0rc2/vendor/fonts/glyphicons/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/templates/devilry_theme3/wcag-debug.django.html` & `devilry-6.3.0rc2/devilry/devilry_theme3/templates/devilry_theme3/wcag-debug.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/devilry_theme3/templatetags/devilry_theme3_tags.py` & `devilry-6.3.0rc2/devilry/devilry_theme3/templatetags/devilry_theme3_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/django_decoupled_docs/README.rst` & `devilry-6.3.0rc2/devilry/django_decoupled_docs/README.rst`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/django_decoupled_docs/registry.py` & `devilry-6.3.0rc2/devilry/django_decoupled_docs/registry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/locale/en/LC_MESSAGES/django.po` & `devilry-6.3.0rc2/devilry/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/locale/en/LC_MESSAGES/djangojs.po` & `devilry-6.3.0rc2/devilry/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/locale/nb/LC_MESSAGES/django.mo` & `devilry-6.3.0rc2/devilry/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/locale/nb/LC_MESSAGES/django.po` & `devilry-6.3.0rc2/devilry/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/locale/nb/LC_MESSAGES/djangojs.po` & `devilry-6.3.0rc2/devilry/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/log.py` & `devilry-6.3.0rc2/devilry/project/log.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/settingsproxy.py` & `devilry-6.3.0rc2/devilry/project/settingsproxy.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/common/cradmin_legacy_settings.py` & `devilry-6.3.0rc2/devilry/project/common/cradmin_legacy_settings.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/common/default_urls.py` & `devilry-6.3.0rc2/devilry/project/common/default_urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/common/projectspecific_settings.py` & `devilry-6.3.0rc2/devilry/project/common/projectspecific_settings.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/common/settings.py` & `devilry-6.3.0rc2/devilry/project/common/settings.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/common/templatecontext.py` & `devilry-6.3.0rc2/devilry/project/common/templatecontext.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/common/management/commands/devilry_common_merge_candidates.py` & `devilry-6.3.0rc2/devilry/project/common/management/commands/devilry_common_merge_candidates.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/develop/dev_urls.py` & `devilry-6.3.0rc2/devilry/project/develop/dev_urls.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from devilry.project.common.default_urls import devilry_urls
 from devilry.project.common.http_error_handlers import *  # noqa
 
 
 urlpatterns = [
     # path('devilry_sandbox/', include('devilry.devilry_sandbox.urls')),
     path('devilry_theme/', include('devilry.devilry_theme3.urls')),
+    path('silk/', include('silk.urls', namespace='silk'))
 ]
 
 if settings.DEBUG:
     import debug_toolbar
     urlpatterns = [
         path('__debug__/', include(debug_toolbar.urls))
     ] + urlpatterns
```

### Comparing `devilry-6.3.0rc1/devilry/project/develop/fabrictasks.py` & `devilry-6.3.0rc2/devilry/project/develop/fabrictasks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/develop/middleware.py` & `devilry-6.3.0rc2/devilry/project/develop/middleware.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/develop/dumps/old_default.sql` & `devilry-6.3.0rc2/devilry/project/develop/dumps/old_default.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/develop/management/commands/devilry_developer_create_deliveries_from_filesystemtree.py` & `devilry-6.3.0rc2/devilry/project/develop/management/commands/devilry_developer_create_deliveries_from_filesystemtree.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/develop/management/commands/devilry_developer_delete_all_except_users.py` & `devilry-6.3.0rc2/devilry/project/develop/management/commands/devilry_developer_delete_all_except_users.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/develop/management/commands/devilry_developer_performance_test_db.py` & `devilry-6.3.0rc2/devilry/project/develop/management/commands/devilry_developer_performance_test_db.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/develop/settings/base.py` & `devilry-6.3.0rc2/devilry/project/develop/settings/base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/develop/settings/develop.py` & `devilry-6.3.0rc2/devilry/project/develop/settings/develop.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if profiler_middleware:
     MIDDLEWARE = MIDDLEWARE + [
         'devilry.utils.profile.ProfilerMiddleware', # Enable profiling. Just add ?prof=yes to any url to see a profile report
     ]
 
 MIDDLEWARE = MIDDLEWARE + [
     'debug_toolbar.middleware.DebugToolbarMiddleware',
+    'silk.middleware.SilkyMiddleware',
 #    "whitenoise.middleware.WhiteNoiseMiddleware",
 ]
 
 # DELAY_MIDDLEWARE_TIME = (80, 120) # Wait for randint(*DELAY_MIDDLEWARE_TIME)/100.0 before responding to each request when using DelayMiddleware
 # delay_middleware = True
 # if delay_middleware:
 #     MIDDLEWARE = MIDDLEWARE + [
@@ -31,15 +32,16 @@
 
 ######################
 #
 # Django Debug Toolbar
 #
 ######################
 INSTALLED_APPS += [
-    'debug_toolbar'
+    'debug_toolbar',
+    'silk'
 ]
 
 
 #######################################################
 #
 # Django allauth with Dataporten provider
 #
@@ -283,7 +285,13 @@
 
 # STORAGES = {
 #    # ...
 #    "staticfiles": {
 #        "BACKEND": "whitenoise.storage.CompressedManifestStaticFilesStorage",
 #    },
 # }
+
+
+SILKY_PYTHON_PROFILER = True
+SILKY_PYTHON_PROFILER_BINARY = True
+SILKY_META = True
+SILKY_ANALYZE_QUERIES = True
```

### Comparing `devilry-6.3.0rc1/devilry/project/develop/settings/test.py` & `devilry-6.3.0rc2/devilry/project/develop/settings/test.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/develop/testhelpers/corebuilder.py` & `devilry-6.3.0rc2/devilry/project/develop/testhelpers/corebuilder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/develop/testhelpers/datebuilder.py` & `devilry-6.3.0rc2/devilry/project/develop/testhelpers/datebuilder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/develop/testhelpers/login.py` & `devilry-6.3.0rc2/devilry/project/develop/testhelpers/login.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/project/develop/testhelpers/soupselect.py` & `devilry-6.3.0rc2/devilry/project/develop/testhelpers/soupselect.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/GroupAssignments.py` & `devilry-6.3.0rc2/devilry/utils/GroupAssignments.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/GroupNodes.py` & `devilry-6.3.0rc2/devilry/utils/GroupNodes.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/OrderedDictFallback.py` & `devilry-6.3.0rc2/devilry/utils/OrderedDictFallback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/anonymize_database.py` & `devilry-6.3.0rc2/devilry/utils/anonymize_database.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/datetimeutils.py` & `devilry-6.3.0rc2/devilry/utils/datetimeutils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/delivery_collection.py` & `devilry-6.3.0rc2/devilry/utils/delivery_collection.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/devilry_djangoaggregate_functions.py` & `devilry-6.3.0rc2/devilry/utils/devilry_djangoaggregate_functions.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/devilry_email.py` & `devilry-6.3.0rc2/devilry/utils/devilry_email.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/filewrapperwithexplicitclose.py` & `devilry-6.3.0rc2/devilry/utils/filewrapperwithexplicitclose.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/groups_groupedby_relatedstudent_and_assignment.py` & `devilry-6.3.0rc2/devilry/utils/groups_groupedby_relatedstudent_and_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/importutils.py` & `devilry-6.3.0rc2/devilry/utils/importutils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/management.py` & `devilry-6.3.0rc2/devilry/utils/management.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/migrationutils.py` & `devilry-6.3.0rc2/devilry/utils/migrationutils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/nodenamesuggestor.py` & `devilry-6.3.0rc2/devilry/utils/nodenamesuggestor.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/passed_in_previous_period.py` & `devilry-6.3.0rc2/devilry/utils/passed_in_previous_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/profile.py` & `devilry-6.3.0rc2/devilry/utils/profile.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/rq_setup.py` & `devilry-6.3.0rc2/devilry/utils/rq_setup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/setting_utils.py` & `devilry-6.3.0rc2/devilry/utils/setting_utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/stream_archives.py` & `devilry-6.3.0rc2/devilry/utils/stream_archives.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/api/api_test_mixin.py` & `devilry-6.3.0rc2/devilry/utils/api/api_test_mixin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/demodb/demousers.py` & `devilry-6.3.0rc2/devilry/utils/demodb/demousers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/graphviz/djangomodels.py` & `devilry-6.3.0rc2/devilry/utils/graphviz/djangomodels.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/graphviz/dot.py` & `devilry-6.3.0rc2/devilry/utils/graphviz/dot.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/tests/delivery_collection_tests.py` & `devilry-6.3.0rc2/devilry/utils/tests/delivery_collection_tests.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/tests/importutils.py` & `devilry-6.3.0rc2/devilry/utils/tests/importutils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/tests/streamable_archive_tests.py` & `devilry-6.3.0rc2/devilry/utils/tests/streamable_archive_tests.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/tests/test_anonymize_db.py` & `devilry-6.3.0rc2/devilry/utils/tests/test_anonymize_db.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/tests/test_datetimeutils.py` & `devilry-6.3.0rc2/devilry/utils/tests/test_datetimeutils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/tests/test_groups_groupedby_relatedstudent_and_assignment.py` & `devilry-6.3.0rc2/devilry/utils/tests/test_groups_groupedby_relatedstudent_and_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/tests/test_nodenamesuggestor.py` & `devilry-6.3.0rc2/devilry/utils/tests/test_nodenamesuggestor.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/tests/test_passed_in_previous_period.py` & `devilry-6.3.0rc2/devilry/utils/tests/test_passed_in_previous_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/tests/test_setting_utils.py` & `devilry-6.3.0rc2/devilry/utils/tests/test_setting_utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/devilry/utils/tests/test_url_datetime.py` & `devilry-6.3.0rc2/devilry/utils/tests/test_url_datetime.py`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/.gitignore` & `devilry-6.3.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/LICENSE` & `devilry-6.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/README.md` & `devilry-6.3.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `devilry-6.3.0rc1/pyproject.toml` & `devilry-6.3.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     "pyflakes==0.8.1",
     "Fabric3==1.14.post1",
     "doc2dash==3.0.0",
     "django-storages==1.1.5",
     "boto==2.32.1",
     "django-auth-ldap",
     "pip-tools",
+    "django-silk",
 ]
 test = [
     "htmls",
     "pytest",
     "pytest-django",
     "pytest-env",
     "model-bakery",
@@ -114,11 +115,11 @@
     "node_modules",
     "/devilry/devilry_theme3/staticsources",
     "/devilry/project/develop/dumps/default.sql",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "6.3.0rc1"
+version = "6.3.0rc2"
 version_files = ["devilry/__init__.py:__version__"]
 tag_format = "$version"
 update_changelog_on_bump = true
```

### Comparing `devilry-6.3.0rc1/PKG-INFO` & `devilry-6.3.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devilry
-Version: 6.3.0rc1
+Version: 6.3.0rc2
 Summary: A system for handling electronic deliveries. See https://github.com/devilry/devilry-django.
 Author: Tor Johansen, Bendik Opstad, Vegard Angell, Magne Westlie, Ilya Kostolomov, Christian Tryti, Rebekka Mørken, Stian Julseth
 Author-email: Espen Angell Kristiansen <post@appresso.no>
 License: Copyright (c) 2010, Devilry contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -80,14 +80,15 @@
 Requires-Dist: urlobject<2.5.0,>=2.4.0
 Requires-Dist: xlsxwriter<1.2.0,>=1.1.0
 Provides-Extra: dev
 Requires-Dist: beautifulsoup4==4.7.1; extra == 'dev'
 Requires-Dist: boto==2.32.1; extra == 'dev'
 Requires-Dist: django-auth-ldap; extra == 'dev'
 Requires-Dist: django-debug-toolbar; extra == 'dev'
+Requires-Dist: django-silk; extra == 'dev'
 Requires-Dist: django-storages==1.1.5; extra == 'dev'
 Requires-Dist: doc2dash==3.0.0; extra == 'dev'
 Requires-Dist: fabric3==1.14.post1; extra == 'dev'
 Requires-Dist: flake8==2.2.2; extra == 'dev'
 Requires-Dist: htmls==1.0.0; extra == 'dev'
 Requires-Dist: model-bakery; extra == 'dev'
 Requires-Dist: pip-tools; extra == 'dev'
```

