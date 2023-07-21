# Comparing `tmp/devilry-6.0.0rc1.tar.gz` & `tmp/devilry-6.0.0rc2.tar.gz`

## Comparing `devilry-6.0.0rc1.tar` & `devilry-6.0.0rc2.tar`

### file list

```diff
@@ -1,1581 +1,1586 @@
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/.coveragerc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/__init__.py
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/admin.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/apps.py
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/baker_recipes.py
--rw-r--r--   0        0        0    10440 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/deliverystore.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/devilry_core_baker_factories.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/group_user_lookup.py
--rw-r--r--   0        0        0    39763 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/testhelper.py
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/testhelpers.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/urls.py
--rw-r--r--   0        0        0    34188 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0001_initial.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0002_auto_20150915_1127.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0003_auto_20150917_1537.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0004_examiner_relatedexaminer.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0005_relatedexaminer_automatic_anonymous_id.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0006_auto_20151112_1851.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0007_assignment_gradeform_setup_json.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0008_auto_20151222_1955.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0009_assignmentgroup_batchoperation.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0010_assignment_anonymizationmode.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0011_datamigrate_anonymous_to_anonymizationmode.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0012_auto_20160111_2019.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0013_auto_20160111_2021.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0014_auto_20160112_1052.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0015_assignment_uses_custom_candidate_ids.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0016_auto_20160112_1831.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0017_candidate_relatedstudent_replaces_student_field.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0018_auto_20160112_1923.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0019_auto_20160113_2037.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0020_relatedexaminer_active.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0021_examiner_relatedexaminer_replaces_user_field.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0022_auto_20160114_1520.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0023_auto_20160114_1522.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0024_auto_20160114_1524.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0025_auto_20160114_1525.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0026_auto_20160114_1528.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0027_auto_20160116_1843.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0028_auto_20160119_0337.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0029_assignmentgrouphistory.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0030_auto_20170124_1504.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0031_auto_20170125_1601.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0032_datamigrate_update_for_no_none_values_in_assignment_firstdeadline.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0033_auto_20170220_1330.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0034_auto_20170303_1308.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0035_auto_20170523_1747.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0036_auto_20170523_1748.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0037_auto_20170620_1515.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0038_auto_20170621_1720.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0039_assignmentgroup_internal_is_being_deleted.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0040_auto_20180214_1654.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0041_auto_20180220_0651.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0042_candidateassignmentgrouphistory_examinerassignmentgrouphistory.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0043_auto_20180302_1139.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0044_auto_20190624_1238.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0045_auto_20210427_1350.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/0046_auto_20220519_1043.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/migrations/__init__.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/__init__.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/abstract_applicationkeyvalue.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/abstract_is_admin.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/abstract_is_candidate.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/abstract_is_examiner.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/administrators.py
--rw-r--r--   0        0        0    50913 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/assignment.py
--rw-r--r--   0        0        0    76482 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/assignment_group.py
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/assignment_group_history.py
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/basenode.py
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/candidate.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/custom_db_fields.py
--rw-r--r--   0        0        0    16062 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/deadline.py
--rw-r--r--   0        0        0    13166 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/delivery.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/deliverytypes.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/devilryuserprofile.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/examiner.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/examiner_candidate_group_history.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/filemeta.py
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/groupinvite.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/model_utils.py
--rw-r--r--   0        0        0    10652 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/period.py
--rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/period_tag.py
--rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/pointrange_to_grade.py
--rw-r--r--   0        0        0    19027 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/relateduser.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/save_interface.py
--rw-r--r--   0        0        0    10883 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/static_feedback.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/models/subject.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/groupinvite_accepted.django.txt
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/groupinvite_invite.django.txt
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/groupinvite_rejected.django.txt
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/comment-summary.django.html
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-base-plain.django.html
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-base.django.html
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-full-plain.django.html
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-full.django.html
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-short.django.html
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/groupstatus.django.html
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/multiple-candidates-long-displayname.django.html
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/multiple-candidates-short-displayname.django.html
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/multiple-examiners-long-displayname.django.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/multiple-examiners-short-displayname.django.html
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/period-tags-on-period.django.html
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/relatedexaminers-on-period-tag.django.html
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/relatedstudents-on-period-tag.django.html
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/relatedusers-on-period-tag.django.html
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/single-candidate-long-displayname.django.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/single-candidate-short-displayname.django.html
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/single-examiner-long-displayname-plain.django.html
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/single-examiner-long-displayname.django.html
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/single-examiner-short-displayname.django.html
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/search/indexes/core/assignment_text.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/search/indexes/core/assignmentgroup_candidates.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/search/indexes/core/assignmentgroup_examiners.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/search/indexes/core/assignmentgroup_tags.txt
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/search/indexes/core/assignmentgroup_text.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/search/indexes/core/basenode_text.txt
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/search/indexes/core/format_user.django.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/search/indexes/core/node_text.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/search/indexes/core/period_text.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templates/search/indexes/core/subject_text.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templatetags/__init__.py
--rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/templatetags/devilry_core_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/__init__.py
--rw-r--r--   0        0        0    79383 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_assignment.py
--rw-r--r--   0        0        0   180651 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_assignment_group.py
--rw-r--r--   0        0        0     8857 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_assignment_group_history.py
--rw-r--r--   0        0        0     8276 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_candidate.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_deadline.py
--rw-r--r--   0        0        0    78327 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_devilry_core_tags.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_examiner.py
--rw-r--r--   0        0        0    30450 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_group_user_lookup.py
--rw-r--r--   0        0        0    24874 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_groupinvite.py
--rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_period.py
--rw-r--r--   0        0        0    12030 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_period_tags.py
--rw-r--r--   0        0        0    20085 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_pointrange_to_grade.py
--rw-r--r--   0        0        0    38546 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_relateduser.py
--rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/tests/test_subject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/views/__init__.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/apps/core/views/download_staticfeedbackfileattachment.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/coreutils/__init__.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/coreutils/utils.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/defaults/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/defaults/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/__init__.py
--rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/admin.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/apps.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/baker_recipes.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/crinstance_account.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/exceptions.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/middleware.py
--rw-r--r--   0        0        0    52183 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/models.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/urls.py
--rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/user_merger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/authbackend/__init__.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/authbackend/default.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/authbackend/ldap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/cradminextensions/__init__.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/cradminextensions/devilry_crmenu_account.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/crapps/__init__.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/crapps/account/__init__.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/crapps/account/index.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/crapps/account/select_language.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/crapps/account/utils.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/migrations/0001_initial.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/migrations/0002_auto_20150917_1731.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/migrations/0003_datamigrate-admins-into-permissiongroups.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/migrations/0004_auto_20151222_1955.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/migrations/0005_auto_20160113_2037.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/migrations/0006_auto_20160120_0424.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/migrations/0007_auto_20210427_1350.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/migrations/0008_auto_20220510_1307.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/migrations/0009_mergeduser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/migrations/__init__.py
--rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/templates/devilry_account/crapps/account/select_language.django.html
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/templates/devilry_account/templatetags/multiple-users-verbose-inline.django.html
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/templates/devilry_account/templatetags/user-verbose-inline-plain.django.html
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/templates/devilry_account/templatetags/user-verbose-inline.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/templatetags/__init__.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/templatetags/devilry_account_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/tests/__init__.py
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/tests/test_devilry_account_tags.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/tests/test_middleware.py
--rw-r--r--   0        0        0    46608 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/tests/test_models.py
--rw-r--r--   0        0        0    16979 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/tests/test_user_merger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/tests/authbackend/__init__.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/tests/authbackend/test_default.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/tests/test_crapps/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/tests/test_crapps/test_account/__init__.py
--rw-r--r--   0        0        0    18890 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/tests/test_crapps/test_account/test_index.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_account/tests/test_crapps/test_account/test_select_language.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/__init__.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/models.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tasks.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/__init__.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/devilry_crinstance_admin.py
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/devilry_crmenu_admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_assignmentgroup.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedexaminer.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedstudent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listfilter/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listfilter/listfilter_assignmentgroup.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listfilter/listfilter_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/multiselect2/__init__.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/multiselect2/multiselect2_relatedstudent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/listbuilder/__init__.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/listbuilder/admindashboard_subject_listbuilder.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/overview.django.html
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/add_groups_to_examiner.django.html
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/examinerdetails.django.html
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/overview.django.html
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/remove_groups_from_examiner.django.html
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-add.django.html
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-replace.django.html
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag-item-value.django.html
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag.django.html
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/random.django.html
--rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/select_method.django.html
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/custom-table.django.html
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/gradingconfiguration-update.django.html
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/examiners.django.html
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/gradingconfiguration.django.html
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/published.django.html
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/settings.django.html
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/statistics.django.html
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/students.django.html
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/utilities.django.html
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/includes/batchdownload_assignment.django.html
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-item-value.django.html
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-overview.django.html
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/candidate-item-value.django.html
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/confirm-view.django.html
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/overview.django.html
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select-period-view.django.html
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select_groups_to_pass.django.html
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/statistics/overview.django.html
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups.django.html
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/merge_groups.django.html
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/overview.django.html
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/split_groups.django.html
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-accumulated-score.django.html
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-assignment-item-value.django.html
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-method.django.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-period-item-value.django.html
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/confirm.django.html
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/manual-select-students.django.html
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/preview-relatedstudent-item-value.django.html
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/preview.django.html
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/select-assignments.django.html
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/selectable-assignment-item-value.django.html
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/selected-assignment-item-value.django.html
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/includes/select-assignment-item-value-description.django.html
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-assignment-item-value.django.html
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-method.django.html
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-period-item-value.django.html
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/confirm.django.html
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupdetails/details-renderable.django.html
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupdetails/view.django.html
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupview_base/base-info-view.django.html
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupview_base/base-multiselect-view.django.html
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupview_base/include/no-items-message.django.html
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/common/abstract-type-in-users.django.html
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/common/admin-list-view.django.html
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/common/admins-explained.django.html
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/overview.django.html
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/group_by_assignment.django.html
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_groups.django.html
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_users.django.html
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/listbuilder/admindashboard_subject_listbuilder/value.django.html
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/listbuilder/assignmentgroup_listbuilder/value.django.html
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/listbuilder/listbuilder_relatedexaminer/onassignment-itemvalue.django.html
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/listbuilder/listbuilder_relatedstudent/readonly-itemvalue.django.html
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/multiselect2/multiselect2_relatedstudent/itemvalue.django.html
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/multiselect2/multiselect2_relatedstudent/selecteditem.django.html
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/overview.django.html
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/admins/add.django.html
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/admins/overview-itemvalue.django.html
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/admins/overview.django.html
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/column_header_item.django.html
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/devilry_admin_all_results_overview_table.django.html
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/devilry_all_results_overview.django.html
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/result_cell_value.django.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/student_cell_value.django.html
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/createassignment.django.html
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/helpbox.django.html
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/success_message.django.html
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/suggested_deadlines.django.html
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/edit/updateview.django.html
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/examiners/add.django.html
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview-itemvalue.django.html
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview.django.html
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/add-tag.django.html
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/base-multiselect-view.django.html
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/crud.django.html
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/delete.django.html
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/manage-tags-list-view.django.html
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/tag-item-value.django.html
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/relatedusers/select-method.django.html
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/qualifiedforfinalexams/statuslistview-info-column.django.html
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/qualifiedforfinalexams/userlistview-info-column.django.html
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/add.django.html
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/overview-itemvalue.django.html
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/overview.django.html
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/students-not-added-to-assignments-warning.django.html
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/userselectview-no-searchresults-message.django.html
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/overview.django.html
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/overview_for_period_admins.html
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/admins/add.django.html
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview-itemvalue.django.html
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview.django.html
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/edit/updateview.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/__init__.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_anonymizationmode.py
--rw-r--r--   0        0        0    44944 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_batchframework_tasks.py
--rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_crinstance_assignment.py
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_deadline_handling.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_examiner_selfassign.py
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_examiner_statistics.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_first_deadline.py
--rw-r--r--   0        0        0    12214 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_grading_configuration.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_long_and_shortname.py
--rw-r--r--   0        0        0    48383 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_overview.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_projectgroups.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_publishing_time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/examiners/__init__.py
--rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_add_groups_to_examiner.py
--rw-r--r--   0        0        0    63295 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_bulk_organize.py
--rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_examinerdetails.py
--rw-r--r--   0        0        0    12880 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_overview.py
--rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_remove_groups_from_examiner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/__init__.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_overview.py
--rw-r--r--   0        0        0    51914 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period.py
--rw-r--r--   0        0        0    10256 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period_manual.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/__init__.py
--rw-r--r--   0        0        0    44849 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_create_groups.py
--rw-r--r--   0        0        0    45703 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_create_groups_accumulated_score.py
--rw-r--r--   0        0        0    46531 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_delete_groups.py
--rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupdetails.py
--rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_merge_groups.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_overview.py
--rw-r--r--   0        0        0    50909 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_replace_groups.py
--rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_split_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/__init__.py
--rw-r--r--   0        0        0    19748 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_baseinforview.py
--rw-r--r--   0        0        0    19777 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_basemultiselectview.py
--rw-r--r--   0        0        0    77200 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_groupviewmixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_download_files/__init__.py
--rw-r--r--   0        0        0    33016 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_download_files/test_batchdownload_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/common/__init__.py
--rw-r--r--   0        0        0    16683 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/common/admins_common_testmixins.py
--rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/common/test_bulkimport_users_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/cradminextensions/__init__.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/cradminextensions/test_devilry_crmenu_admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/__init__.py
--rw-r--r--   0        0        0     8928 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedexaminer.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedstudent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/cradminextensions/test_multiselect2/__init__.py
--rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/cradminextensions/test_multiselect2/test_multiselect2_relatedstudent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/dashboard/__init__.py
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/dashboard/test_createsubject.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/dashboard/test_crinstance_dashboard.py
--rw-r--r--   0        0        0    18818 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/dashboard/test_overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/__init__.py
--rw-r--r--   0        0        0    29261 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_assignment_listview.py
--rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_student_listview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/__init__.py
--rw-r--r--   0        0        0    29781 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_admins.py
--rw-r--r--   0        0        0    40873 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_createassignment.py
--rw-r--r--   0        0        0    15268 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_crinstance_period.py
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_edit.py
--rw-r--r--   0        0        0    34091 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_examiners.py
--rw-r--r--   0        0        0    19450 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_overview.py
--rw-r--r--   0        0        0    10863 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_overview_all_results.py
--rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_period_all_results_collector.py
--rw-r--r--   0        0        0    34017 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_students.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_manage_tags/__init__.py
--rw-r--r--   0        0        0    53319 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags.py
--rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags_relatedusers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_report/__init__.py
--rw-r--r--   0        0        0    42098 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_report/test_all_results_generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/subject/__init__.py
--rw-r--r--   0        0        0    26747 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/subject/test_admins.py
--rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/subject/test_createperiod.py
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/subject/test_crinstance_subject.py
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/subject/test_edit.py
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/subject/test_overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/__init__.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/test_crinstance_for_periodadmin.py
--rw-r--r--   0        0        0    11399 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/test_overview_for_periodadmin.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/test_subject_redirect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/__init__.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/anonymizationmode.py
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/crinstance_assignment.py
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/deadline_handling.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiner_selfassign.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/first_deadline.py
--rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/gradingconfiguration.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/long_and_shortname.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/overview.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/projectgroups.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/publishing_time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/download_files/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/download_files/backends.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/download_files/batch_download_api.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/download_files/download_archive.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiners/__init__.py
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiners/add_groups_to_examiner.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiners/base_single_examinerview.py
--rw-r--r--   0        0        0    24438 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiners/bulk_organize.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiners/examinerdetails.py
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiners/overview.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiners/remove_groups_from_examiner.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/__init__.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/overview.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_period.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_semester_manual.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/statistics/__init__.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/statistics/statistics_overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/__init__.py
--rw-r--r--   0        0        0    18351 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/create_groups.py
--rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/create_groups_accumulated_score.py
--rw-r--r--   0        0        0    19774 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/delete_groups.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/groupdetails.py
--rw-r--r--   0        0        0    11479 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/groupview_base.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/manage_deadlines.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/merge_groups.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/overview.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/replace_groups.py
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/split_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/common/__init__.py
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/common/bulkimport_users_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/__init__.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/createsubject.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/crinstance_dashboard.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/overview.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/__init__.py
--rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/assignment_list.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/filters.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/student_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/period/__init__.py
--rw-r--r--   0        0        0    11280 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/period/admins.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/period/all_results_generator.py
--rw-r--r--   0        0        0    16100 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/period/createassignment.py
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/period/crinstance_period.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/period/edit.py
--rw-r--r--   0        0        0    11244 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/period/examiners.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/period/overview.py
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/period/overview_all_results.py
--rw-r--r--   0        0        0    12995 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/period/overview_all_results_collector.py
--rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/period/students.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/period/manage_tags/__init__.py
--rw-r--r--   0        0        0    24353 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/period/manage_tags/manage_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/subject/__init__.py
--rw-r--r--   0        0        0    10432 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/subject/admins.py
--rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/subject/createperiod.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/subject/crinstance_subject.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/subject/edit.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/subject/overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/subject_for_period_admin/__init__.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/subject_for_period_admin/crinstance_subject_for_periodadmin.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/subject_for_period_admin/overview_for_periodadmin.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_admin/views/subject_for_period_admin/subject_redirect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_authenticate/__init__.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_authenticate/allauth_adapter.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_authenticate/apps.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_authenticate/socialaccount_user_updaters.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_authenticate/urls.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/login.django.html
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/logout.django.html
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_authenticate/views/__init__.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_authenticate/views/allauth_views.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_authenticate/views/custom_login_view.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_bulkcreate_users/__init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_bulkcreate_users/create_users.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_bulkcreate_users/urls.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/confirm_bulkcreated_users.django.html
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/show_bulkcreated_users.django.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/submit_bulkcreate_users.django.html
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_bulkcreate_users/views/__init__.py
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_bulkcreate_users/views/submit_bulk_users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_changelog/__init__.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_changelog/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/__init__.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/admin.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/apps.py
--rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/editor_widget.py
--rw-r--r--   0        0        0    14740 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/models.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/api/__init__.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/api/preview_markdown.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/migrations/0001_initial.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/migrations/0002_auto_20160109_1210.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/migrations/0003_auto_20160109_1239.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/migrations/0004_commentfile_created_datetime.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/migrations/0005_auto_20160122_1709.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/migrations/0006_auto_20170621_1720.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/migrations/0007_auto_20170630_0309.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/migrations/0008_commentfile_v2_id.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/migrations/0009_auto_20180509_1528.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/migrations/0010_commentedithistory.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/migrations/0011_auto_20220421_1242.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/migrations/__init__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/templates/devilry_comment/devilry_markdown_editor.django.html
--rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/tests/__init__.py
--rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/tests/test_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/views/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_comment/views/markdown_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/__init__.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/abstract_batch_action.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/admin.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/apps.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/backend_registry.py
--rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/backends/__init__.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/backends/backend_mock.py
--rw-r--r--   0        0        0    10827 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/backends/backends_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/batchjob_mixins/__init__.py
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/batchjob_mixins/assignment_mixin.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/batchjob_mixins/feedbackset_mixin.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/migrations/0001_initial.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/migrations/0002_auto_20170119_1202.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/migrations/0003_auto_20170119_1648.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/migrations/0004_auto_20170120_1733.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/migrations/0005_compressedarchivemeta_created_by.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/migrations/0006_compressedarchivemeta_created_by_role.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/migrations/0007_auto_20181002_1053.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/tests/__init__.py
--rw-r--r--   0        0        0    14906 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/tests/test_backend.py
--rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/tests/test_model.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_compressionutil/tests/test_registry.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/__init__.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_acemarkdown.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_crinstance.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_crmenu.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_css_icon_map.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/assignment.py
--rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/assignmentgroup.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/common.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_sidebar.py
--rw-r--r--   0        0        0    22529 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_timeline.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/period.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/permissiongroup.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/permissiongroupuser.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/subject.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/user.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listfilter/__init__.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listfilter/assignment.py
--rw-r--r--   0        0        0    26535 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listfilter/assignmentgroup.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listfilter/user.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listfilter/utils.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_multiselect2/__init__.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_multiselect2/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_tablebuilder/__init__.py
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_tablebuilder/base.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_tablebuilder/base_new.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/cradmin_legacy/standalone-base.django.html
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_acemarkdown.django.html
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/common/goforwardlinkitemframe.django.html
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/account-menuitem.django.html
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/breadcrumb-menuitem.django.html
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/menu.django.html
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignment/description.django.html
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/examiner-item-value.django.html
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/fully-anonymous-subjectadmin-group-item-value.django.html
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/item-value.django.html
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/minimal-item-value.django.html
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/minimal-unanonymized-selected-item.django.html
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-examiner-item-value.django.html
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-fully-anonymous-subjectadmin-group-item-value.django.html
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-item-value.django.html
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/selected-item-full.django.html
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/student-item-value.django.html
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/groupdetails.django.html
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/grouptitle.django.html
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/admin-itemvalue.django.html
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/student-itemvalue.django.html
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/permissiongroup/subjectorperiodpermissiongroup-itemvalue.django.html
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/subject/admin-itemvalue.django.html
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listfilter/utils/devilry_with_result_value_renderable.django.html
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/header_itemvalue.django.html
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/itemframe.django.html
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/itemvalue.django.html
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/row.django.html
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/table.django.html
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_cell.django.html
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_row.django.html
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_tablebuilder.django.html
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_confirmview.django.html
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_createview_with_backlink.django.html
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_updateview_with_backlink.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/__init__.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignment.py
--rw-r--r--   0        0        0    73418 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignmentgroup.py
--rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_sidebar.py
--rw-r--r--   0        0        0    14121 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_timeline.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_period.py
--rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroup.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroupuser.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listfilter/__init__.py
--rw-r--r--   0        0        0    21241 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listfilter/test_assignmentgroup_listfilter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_multiselect2/__init__.py
--rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_multiselect2/test_user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_tablebuilder/__init__.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_tablebuilder/test_table.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/viewhelpers/__init__.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_cradmin/viewhelpers/devilry_confirmview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dataporten_allauth/__init__.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dataporten_allauth/callback.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dataporten_allauth/models.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dataporten_allauth/provider.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dataporten_allauth/urls.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dataporten_allauth/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/__init__.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/admin.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/apps.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/bulk_create_queryset_mixin.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql.py
--rw-r--r--   0        0        0     7900 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/models.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/general_purpose_functions.sql
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/assignment/triggers.sql
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/assignment_group/triggers.sql
--rw-r--r--   0        0        0    17478 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/assignment_group_cached_data/rebuild.sql
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/candidate/triggers.sql
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/comment/triggers.sql
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/commentfile/helperfunctions.sql
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/commentfile/triggers.sql
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/examiner/triggers.sql
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/helperfunctions.sql
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/triggers.sql
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/validate.sql
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/groupcomment/triggers.sql
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/imageannotationcomment/triggers.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/devilry_dbcache_testapp/__init__.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/devilry_dbcache_testapp/models.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/migrations/0001_initial.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/migrations/0002_auto_20170108_0948.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/migrations/0003_auto_20170108_1341.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/migrations/0004_auto_20170108_1453.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/migrations/0005_auto_20170124_1504.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/tests/__init__.py
--rw-r--r--   0        0        0    76816 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_assignment_group_cached_data_triggers.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_assignment_group_triggers.py
--rw-r--r--   0        0        0    10410 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_benchmarks.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_bulk_create_queryset_mixin.py
--rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_candidate_triggers.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_comment_triggers.py
--rw-r--r--   0        0        0     7767 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_examiner_triggers.py
--rw-r--r--   0        0        0    17528 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_feedbackset_triggers.py
--rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_groupcomment_triggers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/__init__.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/cradmin_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/models.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/deadline-bulk-multiselect-filterlistview.django.html
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/manage-deadline.django.html
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline-item-value.django.html
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline.django.html
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/suggested-deadlines.django.html
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-base.django.html
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-excluded-groups-move-deadline.django.html
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-excluded-groups-new-attempt.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/tests/__init__.py
--rw-r--r--   0        0        0    33071 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/tests/test_deadline_listview.py
--rw-r--r--   0        0        0    33393 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_admin.py
--rw-r--r--   0        0        0    87456 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_examiner.py
--rw-r--r--   0        0        0    76838 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/tests/test_multiselect_groups.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/views/__init__.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/views/deadline_listview.py
--rw-r--r--   0        0        0    20342 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/views/manage_deadline_view.py
--rw-r--r--   0        0        0     8626 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/views/multiselect_groups_view.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/views/viewutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_detektor/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_detektor/models.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_detektor/migrations/0001_initial.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_detektor/migrations/0002_auto_20180119_1137.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_detektor/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_developemail/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_developemail/admin.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_developemail/email_backend.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_developemail/models.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_developemail/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_developemail/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/models.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/rq_backend.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/rq_jobs.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/comment_email/__init__.py
--rw-r--r--   0        0        0    12531 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/comment_email/comment_email.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/deadline_email/__init__.py
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/deadline_email/deadline_email.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/feedback_email/__init__.py
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/feedback_email/feedback_email.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/management/commands/__init__.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/management/commands/devilry_send_testemail.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/templates/devilry_email/comment_email/comment.txt
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/templates/devilry_email/deadline_email/deadline_moved.txt
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/templates/devilry_email/deadline_email/new_attempt.txt
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/templates/devilry_email/feedback_email/assignment_feedback_student.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/templatetags/__init__.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/templatetags/comment_email_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/tests/__init__.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/tests/test_bulk_feedback.py
--rw-r--r--   0        0        0    67083 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/tests/test_comment_email.py
--rw-r--r--   0        0        0    17611 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/tests/test_deadline_email.py
--rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_email/tests/test_feedback_email.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_errortemplates/__init__.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_errortemplates/views.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_errortemplates/static/devilry_errortemplates/style.css
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_errortemplates/templates/devilry_errortemplates/404.django.html
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_errortemplates/templates/devilry_errortemplates/500.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/__init__.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/models.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tasks.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/cradminextensions/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/cradminextensions/devilry_crinstance_examiner.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/cradminextensions/devilry_crmenu_examiner.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_create_feedback.django.html
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_new_attempt.django.html
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/grouplist.django.html
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/includes/batchdownload_assignment.django.html
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/column_header_item.django.html
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/grade_cell_value.django.html
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/group_cell_value.django.html
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/simple_group_bulk_feedbackview.django.html
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/text_cell_value.django.html
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/dashboard/assignmentlist.django.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign-group-item-value.django.html
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templatetags/__init__.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/templatetags/devilry_examiner_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_assignment/__init__.py
--rw-r--r--   0        0        0    31945 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_assignment/test_batchdownload_api.py
--rw-r--r--   0        0        0    35476 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_assignment/test_batchframework_tasks.py
--rw-r--r--   0        0        0    65831 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback.py
--rw-r--r--   0        0        0    28101 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback_simple.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_assignment/test_crinstance_assignment.py
--rw-r--r--   0        0        0   126915 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_assignment/test_grouplist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_cradminextensions/__init__.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_cradminextensions/test_devilry_crmenu_examiner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_dashboard/__init__.py
--rw-r--r--   0        0        0    34779 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_dashboard/test_assignmentlist.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_dashboard/test_crinstance_dashboard.py
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_api.py
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_crinstance_selfassign.py
--rw-r--r--   0        0        0    36880 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_grouplist.py
--rw-r--r--   0        0        0    12281 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/__init__.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/crinstance_assignment.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/grouplist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/__init__.py
--rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py
--rw-r--r--   0        0        0    11506 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_manage_deadline.py
--rw-r--r--   0        0        0    11298 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_operations_grouplist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/download_files/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/download_files/backends.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/download_files/batch_download_api.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/download_files/download_archive.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/dashboard/__init__.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/dashboard/assignmentlist.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/dashboard/crinstance_dashboard.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/selfassign/__init__.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/selfassign/api.py
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/selfassign/crinstance_selfassign.py
--rw-r--r--   0        0        0    10002 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/selfassign/selfassign.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_examiner/views/selfassign/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/__init__.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/crinstance_frontpage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/cradminextensions/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/cradminextensions/devilry_crmenu_frontpage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/cradminextensions/listbuilder/__init__.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/cradminextensions/listbuilder/listbuilder_role.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/templates/devilry_frontpage/base.django.html
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/templates/devilry_frontpage/frontpage.django.html
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/tests/__init__.py
--rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/tests/test_frontpage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/tests/test_cradminextensions/__init__.py
--rw-r--r--   0        0        0    11517 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/tests/test_cradminextensions/test_listbuilder_role.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/views/__init__.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_frontpage/views/frontpage.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/models.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/urls.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/templates/devilry_gradeform/advanced.editable.gradeform.django.html
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/templates/devilry_gradeform/advanced.gradeform.django.html
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/templates/devilry_gradeform/base.django.html
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/templates/devilry_gradeform/create.gradeform.django.html
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/templates/devilry_gradeform/setup.gradeform.django.html
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/templatetags/__init__.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/templatetags/devilry_gradeform_tags.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/views/__init__.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/views/editable_gradeform.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/views/grade_form.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/views/points_grade_form.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/views/setup_create_gradeform.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/views/setup_gradeform.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradeform/views/viewable_gradeform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/__init__.py
--rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/models.py
--rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/pluginregistry.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/urls.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/migrations/0001_initial.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/migrations/0002_auto_20170108_0948.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/migrations/__init__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/bulkeditfeedbackbuttonbar.django.html
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/editfeedbackbuttonbar.django.html
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/editfeedbackbuttonbar_savedraftonly.django.html
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackbulkeditorbase.django.html
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_bulkpreview.django.html
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_preview.django.html
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackeditorbase.django.html
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/backandforward-bar.django.html
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/backbutton-bar.django.html
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/backward-button.django.html
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/base.django.html
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/currentprogress.django.html
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/forward-button.django.html
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/reconfigurebase.django.html
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/select_points_to_grade_mapper.django.html
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/selectplugin.django.html
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setmaxpoints.django.html
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setpassing_grade_min_points.django.html
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setup_custom_table.django.html
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/summary.django.html
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/use-this-button.django.html
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/editmarkdown.django.html
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/feedbackeditorfilewidget.django.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/__init__.py
--rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/helpers.py
--rw-r--r--   0        0        0    10027 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/test_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/__init__.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/test_download_feedbackdraftfile.py
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/test_feedbackdraft_preview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/__init__.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/base.py
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_select_points_to_grade_mapper.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_selectplugin.py
--rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_setmaxpoints.py
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_setpassing_grade_min_points.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_setup_custom_table.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_summary.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/__init__.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/download_feedbackdraftfile.py
--rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/feedbackbulkeditorbase.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/feedbackdraft_bulkpreview.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/feedbackdraft_preview.py
--rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/feedbackeditorbase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/__init__.py
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/base.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/select_points_to_grade_mapper.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/selectplugin.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/setmaxpoints.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/setpassing_grade_min_points.py
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/setup_custom_table.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/summary.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/widgets/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/widgets/editfeedbackbuttonbar.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/widgets/editmarkdown.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystem/widgets/filewidget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_approved/__init__.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_approved/apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_approved/models.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_approved/urls.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_approved/templates/devilry_gradingsystemplugin_approved/feedbackbulkeditor.django.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_approved/templates/devilry_gradingsystemplugin_approved/feedbackeditor.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_approved/views/__init__.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_approved/views/feedbackeditor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_points/__init__.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_points/apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_points/models.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_points/urls.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_points/templates/devilry_gradingsystemplugin_points/feedbackbulkeditor.django.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_points/templates/devilry_gradingsystemplugin_points/feedbackeditor.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_points/views/__init__.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_points/views/feedbackeditor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/__init__.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/admin.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/apps.py
--rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/devilry_group_baker_factories.py
--rw-r--r--   0        0        0    34983 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/models.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tasks.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/urls.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/cradmin_instances/__init__.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/cradmin_instances/crinstance_admin.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/cradmin_instances/crinstance_base.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/cradmin_instances/crinstance_examiner.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/cradmin_instances/crinstance_student.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/feedbackfeed_builder/__init__.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/feedbackfeed_builder/builder_base.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_sidebarbuilder.py
--rw-r--r--   0        0        0    10659 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_timelinebuilder.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0001_initial.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0002_feedbackset_gradeform_json.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0003_auto_20160106_1418.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0004_auto_20160107_0918.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0005_auto_20160107_0958.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0006_auto_20160107_1000.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0007_auto_20160107_1031.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0008_auto_20160107_1053.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0009_auto_20160107_1100.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0010_auto_20160107_1106.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0011_auto_20160107_1111.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0012_auto_20160107_1129.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0013_auto_20160110_1621.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0014_feedbackset_grading_status.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0015_auto_20160111_1245.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0016_auto_20160114_2202.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0017_auto_20160122_1518.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0018_auto_20160122_1712.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0019_auto_20160822_1945.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0019_auto_20160912_1649.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0020_feedbackset_ignored_datetime.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0021_merge.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0022_auto_20170103_2308.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0023_auto_20170104_0551.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0024_auto_20170107_1838.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0025_auto_20170124_1504.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0026_datamigrate_update_for_no_none_values_in_feedbackset_deadline.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0027_auto_20170206_1146.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0027_auto_20170207_1951.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0028_auto_20170208_1344.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0029_merge.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0030_auto_20170621_1734.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0031_groupcomment_v2_id.py
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0032_auto_20180214_1654.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0033_feedbacksetgradingupdatehistory.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0034_feedbackset_last_updated_by.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/0035_groupcommentedithistory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/migrations/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/base.django.html
--rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed.django.html
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_guidelines.django.html
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/group_comment_edit_base.django.html
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_base.django.html
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_discuss.django.html
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_examiner_admin_discuss.django.html
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_base.django.html
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_delete_groupcomment.html
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_discuss.django.html
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_examiner_admin_discuss.django.html
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_feedback.django.html
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/group_comment_history/comment_history.django.html
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/group_comment_history/history_item_value.django.html
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/admin_commentform_discuss_examiner_headingtext.django.html
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/admin_commentform_discuss_public_headingtext.django.html
--rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/batch_download_archive_script.django.html
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/buttonbar.django.html
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/comments_disabled.django.html
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/examiner.editlastdelivery.django.html
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/examiner_commentform_discuss_examiner_headingtext.django.html
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/examiner_commentform_discuss_public_headingtext.django.html
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/fileupload.django.html
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/groupcomment_edit_delete_option.html
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/student_commentform_headingtext.django.html
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/admin_groupcomment_item_value.django.html
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/base_event_item_value.django.html
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/base_groupcomment_item_value.django.html
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/deadline_expired_item_value.django.html
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/deadline_moved_item_value.django.html
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/examiner_groupcomment_item_value.django.html
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/feedbackset_info_item_value.django.html
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_item_value.django.html
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_updated_item_value.django.html
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/student_groupcomment_item_value.django.html
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/base_sidebar_file_item_value.django.html
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_comment_item_value.django.html
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_feedbackset_item_value.django.html
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_file_item_value.django.html
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_list.django.html
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/template_tags/devilry_group_comment_user_is_none.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templatetags/__init__.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/templatetags/devilry_group_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/__init__.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_devilry_group_mommy_factories.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_templatetags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_crinstance/__init__.py
--rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_crinstance/test_crinstance_admin.py
--rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_crinstance/test_crinstance_examiner.py
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_crinstance/test_crinstance_student.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_download/__init__.py
--rw-r--r--   0        0        0    21694 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_download/test_batchdownload_api.py
--rw-r--r--   0        0        0    10095 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_download/test_batchframework_compression.py
--rw-r--r--   0        0        0    17151 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_download/test_feedbackfeed_bulkfiledownload.py
--rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_download/test_feedbackfeed_filedownload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/admin/__init__.py
--rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/admin/test_comment_edit_history.py
--rw-r--r--   0        0        0    37226 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/admin/test_feedbackfeed_admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/__init__.py
--rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_comment_edit_history.py
--rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_delete_comment.py
--rw-r--r--   0        0        0    50866 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_discuss.py
--rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_comment.py
--rw-r--r--   0        0        0    13104 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_grade.py
--rw-r--r--   0        0        0    37037 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_feedback.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/__init__.py
--rw-r--r--   0        0        0    30200 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_admin.py
--rw-r--r--   0        0        0    25291 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_common.py
--rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_examiner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/student/__init__.py
--rw-r--r--   0        0        0    14087 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/student/test_comment_edit_history.py
--rw-r--r--   0        0        0   109725 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/student/test_feedbackfeed_student.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed_builders/__init__.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_sidebarbuilder.py
--rw-r--r--   0        0        0    21620 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_timeline_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_models/__init__.py
--rw-r--r--   0        0        0    18792 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_models/test_feedback_set.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_models/test_feedbackfeed_model.py
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_models/test_feedbackset_passed_pervious_period.py
--rw-r--r--   0        0        0    17503 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/tests/test_models/test_group_comment.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/utils/__init__.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/utils/download_response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/__init__.py
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/cradmin_comment_history.py
--rw-r--r--   0        0        0    24391 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/cradmin_feedbackfeed_base.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/group_comment_edit_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/admin/__init__.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/admin/feedbackfeed_admin.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/admin/group_comment_history.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/admin/manage_deadline.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/download_files/__init__.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/download_files/backends.py
--rw-r--r--   0        0        0    15946 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/download_files/batch_download_api.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/download_files/batch_download_files.py
--rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/download_files/feedbackfeed_bulkfiledownload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/examiner/__init__.py
--rw-r--r--   0        0        0    21527 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/examiner/feedbackfeed_examiner.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/examiner/group_comment_history.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/examiner/manage_deadline.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/student/__init__.py
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/student/feedbackfeed_student.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_group/views/student/group_comment_history.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/models.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/urls.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/templates/devilry_header/about_me.django.html
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/templates/devilry_header/app.django.html
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/templates/devilry_header/header2_extjsinclude.django.html
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/templates/devilry_header/header2include.django.html
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/templates/devilry_header/includes/change_language.django.html
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/tests/__init__.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/tests/test_aboutme.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/tests/test_change_language.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/views/__init__.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/views/about_me.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_header/views/change_language.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_help/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_help/tests.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_help/urls.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_help/views.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_help/templates/devilry_help/help.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_i18n/__init__.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_i18n/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_i18n/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/__init__.py
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporter.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/models.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/management/commands/__init__.py
--rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/management/commands/devilry_import_v2_database.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/migrations/0001_initial.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/migrations/0002_auto_20190624_1238.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/migrations/0003_auto_20210427_1350.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/migrations/__init__.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/__init__.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/assignment_importer.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/assignmentgroup_importer.py
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/candidate_examiner_importer.py
--rw-r--r--   0        0        0    13855 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/delivery_feedback_importers.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/feedbackset_importer.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/modelimporter_utils.py
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/node_importer.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/period_importer.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/pointrange_to_grade_importer.py
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/qualifiesforexam_importer.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/relateduser_importer.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/subject_importer.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/user_importer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/scripts/__init__.py
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/scripts/user_add_missing_data_from_json.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/__init__.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/importer_testcase_mixin.py
--rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentgroupimporter.py
--rw-r--r--   0        0        0    12575 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentimporter.py
--rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_candidateimporter.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_commentfilecontentimporter.py
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_deliveryimporter.py
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_examinerimporter.py
--rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_feedbacksetimporter.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_filemetaimporter.py
--rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_nodeimporter.py
--rw-r--r--   0        0        0     9128 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_periodimporter.py
--rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointrangetogradeimporter.py
--rw-r--r--   0        0        0     7374 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointtogrademapimporter.py
--rw-r--r--   0        0        0    14419 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_qualifiesforexam_importer.py
--rw-r--r--   0        0        0     9054 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedexaminerimporter.py
--rw-r--r--   0        0        0     8955 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedstudentimporter.py
--rw-r--r--   0        0        0    22341 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_staticfeedbackimporter.py
--rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_subjectimporter.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_userimporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_scripts/__init__.py
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_scripts/test_user_add_missing_data_from_json.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/__init__.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2assignment_directoryparser.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2assignmentgroup_directoryparser.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2candidate_directoryparser.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2deadline_directoryparser.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2delivery_directoryparser.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2examiner_directoryparser.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2filemeta_directoryparser.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2node_directoryparser.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2period_directoryparser.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2pointrangetograde_directoryparser.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2pointtogrademap_directoryparser.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2qualifiesforexam_finalexam_directoryparser.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2qualifiesforexam_status_directoryparser.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2relatedexaminer_directoryparser.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2relatedstudent_directoryparser.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2staticfeedback_directoryparser.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2subject_directoryparser.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/v2user_directoryparser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_markup/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_markup/models.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_markup/parse_markdown.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_markup/urls.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_markup/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_markup/markdown_extensions/__init__.py
--rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_markup/markdown_extensions/code_diff.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_markup/markdown_extensions/latex_math.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_markup/templates/devilry_markup/code_diff.html
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_markup/templates/devilry_markup/latex_math.html
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_markup/templates/markup/load_latex_support.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/admin.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/migrations/0001_initial.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/migrations/0002_auto_20210427_1350.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/migrations/__init__.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/models/__init__.py
--rw-r--r--   0        0        0    20293 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/models/base.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/templates/devilry_message/for_test.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/tests/__init__.py
--rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/tests/test_message.py
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/tests/test_message_receiver.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/utils/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_message/utils/subject_generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/__init__.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/admin.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/apps.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/cradmin_app.py
--rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/models.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/pluginhelpers.py
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/plugintyperegistry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/listbuilder/__init__.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/listbuilder/plugin_listbuilder_list.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/migrations/0001_initial.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/migrations/0002_auto_20170223_1112.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/migrations/0003_auto_20170629_1914.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/migrations/0004_auto_20210427_1350.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/migrations/0005_deletedqualifiesforfinalexam.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tablebuilder/__init__.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tablebuilder/tablebuilder.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/base.django.html
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/list_statuses.django.html
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/print_view.html
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/retract_status.django.html
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/selectplugin.django.html
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_preview.django.html
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_show.html
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/includes/qualification_table.django.html
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/description.django.html
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/plugin_item_value.django.html
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/tablebuilder/qualificationstatus_valueitem.django.html
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/tablebuilder/relatedstudent_valueitem.django.html
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/tablebuilder/tableheader_valueitem.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/__init__.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_list_statuses_view.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_models.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_plugin_listbuilder_list.py
--rw-r--r--   0        0        0    16296 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_pluginhelpers.py
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_pluginselection_view.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_plugintyperegistry.py
--rw-r--r--   0        0        0    17221 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_preview.py
--rw-r--r--   0        0        0    22999 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_showstatus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/utils/__init__.py
--rw-r--r--   0        0        0    21904 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/utils/groups_groupedby_relatedstudent_and_assignments.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/views/__init__.py
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/views/list_statuses_view.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/views/plugin_mixin.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/views/pluginselection_view.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/views/proxyview.py
--rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/views/qualification_preview_view.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/views/plugin_base_views/__init__.py
--rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/views/plugin_base_views/base_multiselect_view.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/apps.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/models.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/plugin.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/resultscollector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/tests/__init__.py
--rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/tests/test_resultscollector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/views/__init__.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/views/select_assignment.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_points/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_points/apps.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_points/models.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_points/plugin.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_points/resultscollector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_points/tests/__init__.py
--rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_points/tests/test_resultscollector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_points/views/__init__.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_points/views/select_assignment_and_points.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_students/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_students/apps.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_students/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_students/tests/__init__.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_students/tests/test_student_selection_view.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_students/views/__init__.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_students/views/select_students.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/__init__.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/abstract_generator.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/admin.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/generator_registry.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/models.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/rq_task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/urls.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/migrations/0001_initial.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/migrations/0002_auto_20210427_1350.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/migrations/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/templates/devilry_report/download_report.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/tests/__init__.py
--rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/tests/test_download_report_view.py
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/tests/test_generator_registry.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/tests/test_report_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/views/__init__.py
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_report/views/download_report.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_resetpassword/__init__.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_resetpassword/urls.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_rest/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_rest/__init__.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_rest/auth.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_rest/formfields.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_rest/models.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_rest/serializehelpers.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_rest/testclient.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_rest/tests/__init__.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_rest/tests/test_serializehelpers.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_sandbox/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_sandbox/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_sandbox/models.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_sandbox/sandbox.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_sandbox/urls.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_sandbox/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_sandbox/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_sandbox/management/commands/__init__.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_sandbox/management/commands/devilry_sandboxcreate.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_sandbox/templates/devilry_sandbox/createsubject.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_settings/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_settings/models.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_settings/urls.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_settings/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/__init__.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/api/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/api/assignment/__init__.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/api/assignment/api_utils.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/api/assignment/examiner_average_grading_points.py
--rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/api/assignment/examiner_details.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/api/assignment/examiner_group_results.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/management/commands/__init__.py
--rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/management/commands/devilry_create_test_course.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/management/commands/devilry_statistics_make_assignment_with_graded_groups.py
--rw-r--r--   0        0        0   606439 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/static/devilry_statistics/6.0.0rc1/devilry_statistics_all.js
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/.babelrc
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/.editorconfig
--rw-r--r--   0        0        0   475670 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/package-lock.json
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/package.json
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/webpack.config.js
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/devilry_statistics_all.js
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerAverageGradingPointsWidget.js
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerDetailsWidget.js
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerGroupResultWidget.js
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/registerAllWidgets.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/tests/__init__.py
--rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/tests/test_api_examiner_average_grading_points.py
--rw-r--r--   0        0        0    18649 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/tests/test_api_examiner_details.py
--rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_statistics/tests/test_api_examiner_group_result.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/__init__.py
--rw-r--r--   0        0        0     5154 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/models.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/cradminextensions/__init__.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/cradminextensions/columntypes.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/cradminextensions/devilry_crinstance_student.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/cradminextensions/devilry_crmenu_student.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/cradminextensions/studentobjecttable.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/migrations/__init__.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/add_delivery.django.html
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/contactapp/contact.django.html
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery-number-column.django.html
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery-status-column.django.html
--rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_details.django.html
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_list.django.html
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/overviewapp/overview.django.html
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_delete.django.html
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond.django.html
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond_standalone.django.html
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/projectgroup_overview.django.html
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_period/assignmentsapp/assignmentgroup-list.django.html
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_period/assignmentsapp/statuscolumn.django.html
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_student/allperiods/allperiods.django.html
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_student/recentdeliveriesapp/delivery-summary-with-assignment-column.django.html
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_student/waitingfordeliveriesapp/last-deadline.django.html
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_student/waitingfordeliveriesapp/waiting-for-deliveries-list.django.html
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/delivery-summary-column.django.html
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/naturaltime-and-datetime-column.django.html
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/naturaltime-column.django.html
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/dashboard/dashboard.django.html
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/include/feedback-rendered-view.django.html
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/include/group_breadcrumb.django.html
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/period/overview.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templatetags/__init__.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/templatetags/devilry_student_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/tests/__init__.py
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/tests/test_models.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/tests/test_templatetags.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/tests/upload_testfile1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/tests/test_cradminextensions/__init__.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/tests/test_cradminextensions/test_devilry_crmenu_student.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/tests/test_dashboard/__init__.py
--rw-r--r--   0        0        0    14380 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/tests/test_dashboard/test_allperiods.py
--rw-r--r--   0        0        0    41388 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/tests/test_dashboard/test_dashboard.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/tests/test_group/__init__.py
--rw-r--r--   0        0        0    88623 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/tests/test_group/test_projectgroupapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/tests/test_period/__init__.py
--rw-r--r--   0        0        0    28524 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/tests/test_period/test_overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/views/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/views/show_delivery.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/views/dashboard/__init__.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/views/dashboard/allperiods.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/views/dashboard/crinstance_dashboard.py
--rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/views/dashboard/dashboard.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/views/group/__init__.py
--rw-r--r--   0        0        0    14862 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/views/group/projectgroupapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/views/period/__init__.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/views/period/crinstance_period.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_student/views/period/overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/models.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tasks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/delete_periods/__init__.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/delete_periods/period_delete.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/examples/relatedexaminers.json
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/examples/relatedstudents.json
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/examples/relatedstudents_email_instead_of_username.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_anonymize_database.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_clear_allauth_account_tables.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_compressed_archives.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_inactive_users.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_message_receivers.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_messages_without_receivers.py
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_periods.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_fix_missing_first_feedbackset.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_mark_as_passed_in_previous_period.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodadd.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodadminadd.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodadminclear.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodsearch.py
--rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedexaminers.py
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedstudents.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_permissiongroup_add_subject.py
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_qualifiedforfinalexam_delete_duplicates.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_rename_periodtag_prefix.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_resend_failed_messages.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_setup_dataporten_provider.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_setup_primary_domain.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_show_assignment_guidelines.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectadd.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectadminadd.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectadminclear.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectsearch.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_test_rq_task.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_useradd.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_useraddbulk.py
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_usermerge.py
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_usermod.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/__init__.py
--rw-r--r--   0        0        0    14750 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_inactive_users.py
--rw-r--r--   0        0        0    19826 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_periods.py
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminadd.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminclear.py
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_permissiongroup_add_subject.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_qualifiedforfinalexam_delete_duplicates.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadd.py
--rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminadd.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminclear.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_useraddbulk.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_usermod.py
--rw-r--r--   0        0        0     7755 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_resend_failed_messages.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/models.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/urls.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/views.py
--rw-r--r--   0        0        0    40723 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/media/images/groovepaper.png
--rw-r--r--   0        0        0    14235 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/media/images/favicons/apple-touch-icon.png
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/media/images/favicons/favicon.ico
--rw-r--r--   0        0        0    65078 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/devilry_all.js
--rw-r--r--   0        0        0   474892 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/devilry_all.js.map
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/katex/LICENSE
--rw-r--r--   0        0        0    23112 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/katex/katex.min.css
--rw-r--r--   0        0        0   598523 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/katex/katex.mjs
--rw-r--r--   0        0        0    27456 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/commentEditor.js
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/cookie.js
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/examinerSelfAssignButton.js
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/feedbackfeedNavigationHandler.js
--rw-r--r--   0        0        0    20380 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/fileupload.js
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/helloWorld.js
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/latex_math.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/webcomponent_utils.js
--rw-r--r--   0        0        0   292191 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/styles/cradmin_theme_devilry_mainpages/theme.css
--rw-r--r--   0        0        0   220499 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/styles/cradmin_theme_devilry_superuserui/theme.css
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/templates/devilry_deploy/custom_css.django.css
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/templates/devilry_deploy/custom_css_base.django.html
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/templates/devilry_deploy/footer.django.html
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/templates/devilry_deploy/footer_base.django.html
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/templates/devilry_deploy/frontpage_footer.django.html
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/templates/devilry_deploy/login_footer.django.html
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/templates/devilry_theme3/favicons.django.html
--rw-r--r--   0        0        0    25100 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/templates/devilry_theme3/wcag-debug.django.html
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/templates/devilry_theme3/include/devilry_all_js.django.html
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/templates/devilry_theme3/include/includetest.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/templatetags/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/devilry_theme3/templatetags/devilry_theme3_tags.py
--rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/django_decoupled_docs/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/django_decoupled_docs/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/django_decoupled_docs/models.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/django_decoupled_docs/registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/django_decoupled_docs/templatetags/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/django_decoupled_docs/templatetags/django_decoupled_docs_tags.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   265284 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/locale/en/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0   174316 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   370053 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/locale/nb/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/__init__.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/log.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/settingsproxy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/cradmin_legacy_settings.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/default_urls.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/devilry_test_runner.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/docproxies.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/http_error_handlers.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/i18n.py
--rw-r--r--   0        0        0     9810 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/projectspecific_settings.py
--rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/settings.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/templatecontext.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/formats/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/formats/en/__init__.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/formats/en/formats.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/formats/nb/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/formats/nb/formats.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/management/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/management/commands/__init__.py
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/common/management/commands/devilry_common_merge_candidates.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/__init__.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/dev_urls.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/fabrictasks.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/models.py
--rw-r--r--   0        0        0   353927 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/dumps/old_default.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/management/commands/__init__.py
--rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/management/commands/devilry_developer_create_deliveries_from_filesystemtree.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/management/commands/devilry_developer_delete_all_except_users.py
--rw-r--r--   0        0        0    15531 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/management/commands/devilry_developer_performance_test_db.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/management/commands/devilry_developer_set_all_passwords_to_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/settings/__init__.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/settings/base.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/settings/codeship_test.py
--rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/settings/develop.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/settings/docs.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/settings/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/testhelpers/__init__.py
--rw-r--r--   0        0        0    22236 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/testhelpers/corebuilder.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/testhelpers/datebuilder.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/testhelpers/login.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/testhelpers/skip_rq_tests.py
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/develop/testhelpers/soupselect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/production/__init__.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/production/settings.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/production/urls.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/project/production/wsgi.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/GroupAssignments.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/GroupNodes.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/OrderedDictFallback.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/__init__.py
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/anonymize_database.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/command.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/create_absolute_url.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/custom_templates.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/datetimeutils.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/delay_middleware.py
--rw-r--r--   0        0        0     8118 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/delivery_collection.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/devilry_djangoaggregate_functions.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/devilry_email.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/dictutils.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/filewrapperwithexplicitclose.py
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/groups_groupedby_relatedstudent_and_assignment.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/importutils.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/logexceptionsmiddleware.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/management.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/migrationutils.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/models.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/module.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/nodenamesuggestor.py
--rw-r--r--   0        0        0    11545 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/passed_in_previous_period.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/profile.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/rq_setup.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/setting_utils.py
--rw-r--r--   0        0        0     7675 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/stream_archives.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/verify_unique_entries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/api/__init__.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/api/api_test_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/demodb/__init__.py
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/demodb/demousers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/graphviz/__init__.py
--rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/graphviz/djangomodels.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/graphviz/dot.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/graphviz/sphinx.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/tests/__init__.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/tests/delivery_collection_tests.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/tests/importutils.py
--rwxr-xr-x   0        0        0     7534 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/tests/streamable_archive_tests.py
--rw-r--r--   0        0        0    15352 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/tests/test_anonymize_db.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/tests/test_datetimeutils.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/tests/test_groups_groupedby_relatedstudent_and_assignment.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/tests/test_nodenamesuggestor.py
--rw-r--r--   0        0        0    47879 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/tests/test_passed_in_previous_period.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/tests/test_setting_utils.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/devilry/utils/tests/test_url_datetime.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/LICENSE
--rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/README.md
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0    10491 2020-02-02 00:00:00.000000 devilry-6.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/.coveragerc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/__init__.py
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/admin.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/apps.py
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/baker_recipes.py
+-rw-r--r--   0        0        0    10440 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/deliverystore.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/devilry_core_baker_factories.py
+-rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/group_user_lookup.py
+-rw-r--r--   0        0        0    39763 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/testhelper.py
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/testhelpers.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/api/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/api/applicationstate.py
+-rw-r--r--   0        0        0    34188 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0002_auto_20150915_1127.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0003_auto_20150917_1537.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0004_examiner_relatedexaminer.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0005_relatedexaminer_automatic_anonymous_id.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0006_auto_20151112_1851.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0007_assignment_gradeform_setup_json.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0008_auto_20151222_1955.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0009_assignmentgroup_batchoperation.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0010_assignment_anonymizationmode.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0011_datamigrate_anonymous_to_anonymizationmode.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0012_auto_20160111_2019.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0013_auto_20160111_2021.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0014_auto_20160112_1052.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0015_assignment_uses_custom_candidate_ids.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0016_auto_20160112_1831.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0017_candidate_relatedstudent_replaces_student_field.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0018_auto_20160112_1923.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0019_auto_20160113_2037.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0020_relatedexaminer_active.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0021_examiner_relatedexaminer_replaces_user_field.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0022_auto_20160114_1520.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0023_auto_20160114_1522.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0024_auto_20160114_1524.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0025_auto_20160114_1525.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0026_auto_20160114_1528.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0027_auto_20160116_1843.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0028_auto_20160119_0337.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0029_assignmentgrouphistory.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0030_auto_20170124_1504.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0031_auto_20170125_1601.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0032_datamigrate_update_for_no_none_values_in_assignment_firstdeadline.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0033_auto_20170220_1330.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0034_auto_20170303_1308.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0035_auto_20170523_1747.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0036_auto_20170523_1748.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0037_auto_20170620_1515.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0038_auto_20170621_1720.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0039_assignmentgroup_internal_is_being_deleted.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0040_auto_20180214_1654.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0041_auto_20180220_0651.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0042_candidateassignmentgrouphistory_examinerassignmentgrouphistory.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0043_auto_20180302_1139.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0044_auto_20190624_1238.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0045_auto_20210427_1350.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/0046_auto_20220519_1043.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/migrations/__init__.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/__init__.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/abstract_applicationkeyvalue.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/abstract_is_admin.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/abstract_is_candidate.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/abstract_is_examiner.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/administrators.py
+-rw-r--r--   0        0        0    50913 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/assignment.py
+-rw-r--r--   0        0        0    76482 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/assignment_group.py
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/assignment_group_history.py
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/basenode.py
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/candidate.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/custom_db_fields.py
+-rw-r--r--   0        0        0    16062 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/deadline.py
+-rw-r--r--   0        0        0    13166 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/delivery.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/deliverytypes.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/devilryuserprofile.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/examiner.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/examiner_candidate_group_history.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/filemeta.py
+-rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/groupinvite.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/model_utils.py
+-rw-r--r--   0        0        0    10652 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/period.py
+-rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/period_tag.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/pointrange_to_grade.py
+-rw-r--r--   0        0        0    19027 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/relateduser.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/save_interface.py
+-rw-r--r--   0        0        0    10883 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/static_feedback.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/models/subject.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/comment-summary.django.html
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-base-plain.django.html
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-base.django.html
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-full-plain.django.html
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-full.django.html
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-short.django.html
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/groupstatus.django.html
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/multiple-candidates-long-displayname.django.html
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/multiple-candidates-short-displayname.django.html
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/multiple-examiners-long-displayname.django.html
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/multiple-examiners-short-displayname.django.html
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/period-tags-on-period.django.html
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/relatedexaminers-on-period-tag.django.html
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/relatedstudents-on-period-tag.django.html
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/relatedusers-on-period-tag.django.html
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/single-candidate-long-displayname.django.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/single-candidate-short-displayname.django.html
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/single-examiner-long-displayname-plain.django.html
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/single-examiner-long-displayname.django.html
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/single-examiner-short-displayname.django.html
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/search/indexes/core/assignment_text.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/search/indexes/core/assignmentgroup_candidates.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/search/indexes/core/assignmentgroup_examiners.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/search/indexes/core/assignmentgroup_tags.txt
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/search/indexes/core/assignmentgroup_text.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/search/indexes/core/basenode_text.txt
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/search/indexes/core/format_user.django.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/search/indexes/core/node_text.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/search/indexes/core/period_text.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templates/search/indexes/core/subject_text.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templatetags/__init__.py
+-rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/templatetags/devilry_core_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/__init__.py
+-rw-r--r--   0        0        0    79383 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_assignment.py
+-rw-r--r--   0        0        0   180651 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_assignment_group.py
+-rw-r--r--   0        0        0     8857 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_assignment_group_history.py
+-rw-r--r--   0        0        0     8276 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_candidate.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_deadline.py
+-rw-r--r--   0        0        0    78327 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_devilry_core_tags.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_examiner.py
+-rw-r--r--   0        0        0    30450 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_group_user_lookup.py
+-rw-r--r--   0        0        0    28214 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_groupinvite.py
+-rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_period.py
+-rw-r--r--   0        0        0    12030 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_period_tags.py
+-rw-r--r--   0        0        0    19992 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_pointrange_to_grade.py
+-rw-r--r--   0        0        0    38546 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_relateduser.py
+-rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/tests/test_subject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/views/__init__.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/apps/core/views/download_staticfeedbackfileattachment.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/coreutils/__init__.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/coreutils/utils.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/defaults/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/defaults/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/__init__.py
+-rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/admin.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/apps.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/baker_recipes.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/crinstance_account.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/exceptions.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/middleware.py
+-rw-r--r--   0        0        0    52183 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/models.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/urls.py
+-rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/user_merger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/authbackend/__init__.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/authbackend/default.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/authbackend/ldap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/cradminextensions/__init__.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/cradminextensions/devilry_crmenu_account.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/crapps/__init__.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/crapps/account/__init__.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/crapps/account/index.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/crapps/account/select_language.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/crapps/account/utils.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/migrations/0001_initial.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/migrations/0002_auto_20150917_1731.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/migrations/0003_datamigrate-admins-into-permissiongroups.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/migrations/0004_auto_20151222_1955.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/migrations/0005_auto_20160113_2037.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/migrations/0006_auto_20160120_0424.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/migrations/0007_auto_20210427_1350.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/migrations/0008_auto_20220510_1307.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/migrations/0009_mergeduser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/migrations/__init__.py
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/templates/devilry_account/crapps/account/select_language.django.html
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/templates/devilry_account/templatetags/multiple-users-verbose-inline.django.html
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/templates/devilry_account/templatetags/user-verbose-inline-plain.django.html
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/templates/devilry_account/templatetags/user-verbose-inline.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/templatetags/__init__.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/templatetags/devilry_account_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/tests/__init__.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/tests/test_devilry_account_tags.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/tests/test_middleware.py
+-rw-r--r--   0        0        0    46608 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/tests/test_models.py
+-rw-r--r--   0        0        0    16979 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/tests/test_user_merger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/tests/authbackend/__init__.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/tests/authbackend/test_default.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/tests/test_crapps/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/tests/test_crapps/test_account/__init__.py
+-rw-r--r--   0        0        0    18890 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/tests/test_crapps/test_account/test_index.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_account/tests/test_crapps/test_account/test_select_language.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/__init__.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/models.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tasks.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/__init__.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/devilry_crinstance_admin.py
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/devilry_crmenu_admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_assignmentgroup.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedexaminer.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedstudent.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listfilter/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listfilter/listfilter_assignmentgroup.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listfilter/listfilter_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/multiselect2/__init__.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/multiselect2/multiselect2_relatedstudent.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/listbuilder/__init__.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/listbuilder/admindashboard_subject_listbuilder.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/overview.django.html
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/add_groups_to_examiner.django.html
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/examinerdetails.django.html
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/overview.django.html
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/remove_groups_from_examiner.django.html
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-add.django.html
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-replace.django.html
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag-item-value.django.html
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag.django.html
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/random.django.html
+-rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/select_method.django.html
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/custom-table.django.html
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/gradingconfiguration-update.django.html
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/examiners.django.html
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/gradingconfiguration.django.html
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/published.django.html
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/settings.django.html
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/statistics.django.html
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/students.django.html
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/utilities.django.html
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/includes/batchdownload_assignment.django.html
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-item-value.django.html
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-overview.django.html
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/candidate-item-value.django.html
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/confirm-view.django.html
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/overview.django.html
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select-period-view.django.html
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select_groups_to_pass.django.html
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/statistics/overview.django.html
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups.django.html
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/merge_groups.django.html
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/overview.django.html
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/split_groups.django.html
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-accumulated-score.django.html
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-assignment-item-value.django.html
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-method.django.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-period-item-value.django.html
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/confirm.django.html
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/manual-select-students.django.html
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/preview-relatedstudent-item-value.django.html
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/preview.django.html
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/select-assignments.django.html
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/selectable-assignment-item-value.django.html
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/selected-assignment-item-value.django.html
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/includes/select-assignment-item-value-description.django.html
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-assignment-item-value.django.html
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-method.django.html
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-period-item-value.django.html
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/confirm.django.html
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupdetails/details-renderable.django.html
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupdetails/view.django.html
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupview_base/base-info-view.django.html
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupview_base/base-multiselect-view.django.html
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupview_base/include/no-items-message.django.html
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/common/abstract-type-in-users.django.html
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/common/admin-list-view.django.html
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/common/admins-explained.django.html
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/overview.django.html
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/group_by_assignment.django.html
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_groups.django.html
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_users.django.html
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/listbuilder/admindashboard_subject_listbuilder/value.django.html
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/listbuilder/assignmentgroup_listbuilder/value.django.html
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/listbuilder/listbuilder_relatedexaminer/onassignment-itemvalue.django.html
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/listbuilder/listbuilder_relatedstudent/readonly-itemvalue.django.html
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/multiselect2/multiselect2_relatedstudent/itemvalue.django.html
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/multiselect2/multiselect2_relatedstudent/selecteditem.django.html
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/overview.django.html
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/admins/add.django.html
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/admins/overview-itemvalue.django.html
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/admins/overview.django.html
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/column_header_item.django.html
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/devilry_admin_all_results_overview_table.django.html
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/devilry_all_results_overview.django.html
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/result_cell_value.django.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/student_cell_value.django.html
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/createassignment.django.html
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/helpbox.django.html
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/success_message.django.html
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/suggested_deadlines.django.html
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/edit/updateview.django.html
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/examiners/add.django.html
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview-itemvalue.django.html
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview.django.html
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/add-tag.django.html
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/base-multiselect-view.django.html
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/crud.django.html
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/delete.django.html
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/manage-tags-list-view.django.html
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/tag-item-value.django.html
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/relatedusers/select-method.django.html
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/qualifiedforfinalexams/statuslistview-info-column.django.html
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/qualifiedforfinalexams/userlistview-info-column.django.html
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/add.django.html
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/overview-itemvalue.django.html
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/overview.django.html
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/students-not-added-to-assignments-warning.django.html
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/userselectview-no-searchresults-message.django.html
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/overview.django.html
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/overview_for_period_admins.html
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/admins/add.django.html
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview-itemvalue.django.html
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview.django.html
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/edit/updateview.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/__init__.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_anonymizationmode.py
+-rw-r--r--   0        0        0    44944 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_batchframework_tasks.py
+-rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_crinstance_assignment.py
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_deadline_handling.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_examiner_selfassign.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_examiner_statistics.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_first_deadline.py
+-rw-r--r--   0        0        0    12214 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_grading_configuration.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_long_and_shortname.py
+-rw-r--r--   0        0        0    48383 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_overview.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_projectgroups.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_publishing_time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/examiners/__init__.py
+-rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_add_groups_to_examiner.py
+-rw-r--r--   0        0        0    63295 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_bulk_organize.py
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_examinerdetails.py
+-rw-r--r--   0        0        0    12880 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_overview.py
+-rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_remove_groups_from_examiner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/__init__.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_overview.py
+-rw-r--r--   0        0        0    51914 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period.py
+-rw-r--r--   0        0        0    10256 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period_manual.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/__init__.py
+-rw-r--r--   0        0        0    44849 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_create_groups.py
+-rw-r--r--   0        0        0    45703 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_create_groups_accumulated_score.py
+-rw-r--r--   0        0        0    46531 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_delete_groups.py
+-rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupdetails.py
+-rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_merge_groups.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_overview.py
+-rw-r--r--   0        0        0    50909 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_replace_groups.py
+-rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_split_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/__init__.py
+-rw-r--r--   0        0        0    19748 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_baseinforview.py
+-rw-r--r--   0        0        0    19777 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_basemultiselectview.py
+-rw-r--r--   0        0        0    77200 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_groupviewmixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_download_files/__init__.py
+-rw-r--r--   0        0        0    33016 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_download_files/test_batchdownload_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/common/__init__.py
+-rw-r--r--   0        0        0    16683 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/common/admins_common_testmixins.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/common/test_bulkimport_users_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/cradminextensions/__init__.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/cradminextensions/test_devilry_crmenu_admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/__init__.py
+-rw-r--r--   0        0        0     8928 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedexaminer.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedstudent.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/cradminextensions/test_multiselect2/__init__.py
+-rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/cradminextensions/test_multiselect2/test_multiselect2_relatedstudent.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/dashboard/__init__.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/dashboard/test_createsubject.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/dashboard/test_crinstance_dashboard.py
+-rw-r--r--   0        0        0    18818 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/dashboard/test_overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/__init__.py
+-rw-r--r--   0        0        0    29261 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_assignment_listview.py
+-rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_student_listview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/__init__.py
+-rw-r--r--   0        0        0    29781 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_admins.py
+-rw-r--r--   0        0        0    40873 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_createassignment.py
+-rw-r--r--   0        0        0    15268 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_crinstance_period.py
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_edit.py
+-rw-r--r--   0        0        0    34091 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_examiners.py
+-rw-r--r--   0        0        0    19450 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_overview.py
+-rw-r--r--   0        0        0    10863 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_overview_all_results.py
+-rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_period_all_results_collector.py
+-rw-r--r--   0        0        0    34017 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_students.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_manage_tags/__init__.py
+-rw-r--r--   0        0        0    51030 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags.py
+-rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags_relatedusers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_report/__init__.py
+-rw-r--r--   0        0        0    42098 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_report/test_all_results_generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/subject/__init__.py
+-rw-r--r--   0        0        0    26747 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/subject/test_admins.py
+-rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/subject/test_createperiod.py
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/subject/test_crinstance_subject.py
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/subject/test_edit.py
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/subject/test_overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/__init__.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/test_crinstance_for_periodadmin.py
+-rw-r--r--   0        0        0    11399 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/test_overview_for_periodadmin.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/test_subject_redirect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/__init__.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/anonymizationmode.py
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/crinstance_assignment.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/deadline_handling.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiner_selfassign.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/first_deadline.py
+-rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/gradingconfiguration.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/long_and_shortname.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/overview.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/projectgroups.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/publishing_time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/download_files/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/download_files/backends.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/download_files/batch_download_api.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/download_files/download_archive.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiners/__init__.py
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiners/add_groups_to_examiner.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiners/base_single_examinerview.py
+-rw-r--r--   0        0        0    24438 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiners/bulk_organize.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiners/examinerdetails.py
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiners/overview.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiners/remove_groups_from_examiner.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/__init__.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/overview.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_period.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_semester_manual.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/statistics/__init__.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/statistics/statistics_overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/__init__.py
+-rw-r--r--   0        0        0    18351 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/create_groups.py
+-rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/create_groups_accumulated_score.py
+-rw-r--r--   0        0        0    19774 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/delete_groups.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/groupdetails.py
+-rw-r--r--   0        0        0    11479 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/groupview_base.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/manage_deadlines.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/merge_groups.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/overview.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/replace_groups.py
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/split_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/common/__init__.py
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/common/bulkimport_users_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/__init__.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/createsubject.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/crinstance_dashboard.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/overview.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/__init__.py
+-rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/assignment_list.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/filters.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/student_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/period/__init__.py
+-rw-r--r--   0        0        0    11280 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/period/admins.py
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/period/all_results_generator.py
+-rw-r--r--   0        0        0    16100 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/period/createassignment.py
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/period/crinstance_period.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/period/edit.py
+-rw-r--r--   0        0        0    11244 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/period/examiners.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/period/overview.py
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/period/overview_all_results.py
+-rw-r--r--   0        0        0    12995 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/period/overview_all_results_collector.py
+-rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/period/students.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/period/manage_tags/__init__.py
+-rw-r--r--   0        0        0    24353 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/period/manage_tags/manage_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/subject/__init__.py
+-rw-r--r--   0        0        0    10432 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/subject/admins.py
+-rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/subject/createperiod.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/subject/crinstance_subject.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/subject/edit.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/subject/overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/subject_for_period_admin/__init__.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/subject_for_period_admin/crinstance_subject_for_periodadmin.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/subject_for_period_admin/overview_for_periodadmin.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_admin/views/subject_for_period_admin/subject_redirect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_authenticate/__init__.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_authenticate/allauth_adapter.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_authenticate/apps.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_authenticate/socialaccount_user_updaters.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_authenticate/urls.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/login.django.html
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/logout.django.html
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_authenticate/views/__init__.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_authenticate/views/allauth_views.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_authenticate/views/custom_login_view.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_bulkcreate_users/__init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_bulkcreate_users/create_users.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_bulkcreate_users/urls.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/confirm_bulkcreated_users.django.html
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/show_bulkcreated_users.django.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/submit_bulkcreate_users.django.html
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_bulkcreate_users/views/__init__.py
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_bulkcreate_users/views/submit_bulk_users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_changelog/__init__.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_changelog/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/__init__.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/admin.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/apps.py
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/editor_widget.py
+-rw-r--r--   0        0        0    14740 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/models.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/api/__init__.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/api/preview_markdown.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/migrations/0001_initial.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/migrations/0002_auto_20160109_1210.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/migrations/0003_auto_20160109_1239.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/migrations/0004_commentfile_created_datetime.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/migrations/0005_auto_20160122_1709.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/migrations/0006_auto_20170621_1720.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/migrations/0007_auto_20170630_0309.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/migrations/0008_commentfile_v2_id.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/migrations/0009_auto_20180509_1528.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/migrations/0010_commentedithistory.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/migrations/0011_auto_20220421_1242.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/migrations/__init__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/templates/devilry_comment/devilry_markdown_editor.django.html
+-rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/tests/__init__.py
+-rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/tests/test_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/views/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_comment/views/markdown_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/__init__.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/abstract_batch_action.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/admin.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/apps.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/backend_registry.py
+-rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/backends/__init__.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/backends/backend_mock.py
+-rw-r--r--   0        0        0    10827 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/backends/backends_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/batchjob_mixins/__init__.py
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/batchjob_mixins/assignment_mixin.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/batchjob_mixins/feedbackset_mixin.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/migrations/0001_initial.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/migrations/0002_auto_20170119_1202.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/migrations/0003_auto_20170119_1648.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/migrations/0004_auto_20170120_1733.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/migrations/0005_compressedarchivemeta_created_by.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/migrations/0006_compressedarchivemeta_created_by_role.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/migrations/0007_auto_20181002_1053.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/tests/__init__.py
+-rw-r--r--   0        0        0    14906 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/tests/test_backend.py
+-rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/tests/test_model.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_compressionutil/tests/test_registry.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/__init__.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_acemarkdown.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_crinstance.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_crmenu.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_css_icon_map.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/assignment.py
+-rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/assignmentgroup.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/common.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_sidebar.py
+-rw-r--r--   0        0        0    22529 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_timeline.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/period.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/permissiongroup.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/permissiongroupuser.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/subject.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/user.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listfilter/__init__.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listfilter/assignment.py
+-rw-r--r--   0        0        0    26535 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listfilter/assignmentgroup.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listfilter/user.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listfilter/utils.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_multiselect2/__init__.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_multiselect2/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_tablebuilder/__init__.py
+-rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_tablebuilder/base.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_tablebuilder/base_new.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/cradmin_legacy/standalone-base.django.html
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_acemarkdown.django.html
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/common/goforwardlinkitemframe.django.html
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/account-menuitem.django.html
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/breadcrumb-menuitem.django.html
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/menu.django.html
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignment/description.django.html
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/examiner-item-value.django.html
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/fully-anonymous-subjectadmin-group-item-value.django.html
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/item-value.django.html
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/minimal-item-value.django.html
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/minimal-unanonymized-selected-item.django.html
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-examiner-item-value.django.html
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-fully-anonymous-subjectadmin-group-item-value.django.html
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-item-value.django.html
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/selected-item-full.django.html
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/student-item-value.django.html
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/groupdetails.django.html
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/grouptitle.django.html
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/admin-itemvalue.django.html
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/student-itemvalue.django.html
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/permissiongroup/subjectorperiodpermissiongroup-itemvalue.django.html
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/subject/admin-itemvalue.django.html
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listfilter/utils/devilry_with_result_value_renderable.django.html
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/header_itemvalue.django.html
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/itemframe.django.html
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/itemvalue.django.html
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/row.django.html
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/table.django.html
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_cell.django.html
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_row.django.html
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_tablebuilder.django.html
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_confirmview.django.html
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_createview_with_backlink.django.html
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_updateview_with_backlink.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/__init__.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignment.py
+-rw-r--r--   0        0        0    73418 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignmentgroup.py
+-rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_sidebar.py
+-rw-r--r--   0        0        0    14121 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_timeline.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_period.py
+-rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroup.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroupuser.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listfilter/__init__.py
+-rw-r--r--   0        0        0    21241 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listfilter/test_assignmentgroup_listfilter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_multiselect2/__init__.py
+-rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_multiselect2/test_user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_tablebuilder/__init__.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_tablebuilder/test_table.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/viewhelpers/__init__.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_cradmin/viewhelpers/devilry_confirmview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dataporten_allauth/__init__.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dataporten_allauth/callback.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dataporten_allauth/models.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dataporten_allauth/provider.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dataporten_allauth/urls.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dataporten_allauth/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/__init__.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/admin.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/apps.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/bulk_create_queryset_mixin.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql.py
+-rw-r--r--   0        0        0     7900 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/models.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/general_purpose_functions.sql
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/assignment/triggers.sql
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/assignment_group/triggers.sql
+-rw-r--r--   0        0        0    17478 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/assignment_group_cached_data/rebuild.sql
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/candidate/triggers.sql
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/comment/triggers.sql
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/commentfile/helperfunctions.sql
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/commentfile/triggers.sql
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/examiner/triggers.sql
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/helperfunctions.sql
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/triggers.sql
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/validate.sql
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/groupcomment/triggers.sql
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/imageannotationcomment/triggers.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/devilry_dbcache_testapp/__init__.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/devilry_dbcache_testapp/models.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/migrations/0002_auto_20170108_0948.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/migrations/0003_auto_20170108_1341.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/migrations/0004_auto_20170108_1453.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/migrations/0005_auto_20170124_1504.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/tests/__init__.py
+-rw-r--r--   0        0        0    76816 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_assignment_group_cached_data_triggers.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_assignment_group_triggers.py
+-rw-r--r--   0        0        0    10410 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_bulk_create_queryset_mixin.py
+-rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_candidate_triggers.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_comment_triggers.py
+-rw-r--r--   0        0        0     7767 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_examiner_triggers.py
+-rw-r--r--   0        0        0    17528 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_feedbackset_triggers.py
+-rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_groupcomment_triggers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/__init__.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/cradmin_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/models.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/deadline-bulk-multiselect-filterlistview.django.html
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/manage-deadline.django.html
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline-item-value.django.html
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline.django.html
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/suggested-deadlines.django.html
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-base.django.html
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-excluded-groups-move-deadline.django.html
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-excluded-groups-new-attempt.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/tests/__init__.py
+-rw-r--r--   0        0        0    33071 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/tests/test_deadline_listview.py
+-rw-r--r--   0        0        0    33393 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_admin.py
+-rw-r--r--   0        0        0    87456 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_examiner.py
+-rw-r--r--   0        0        0    76838 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/tests/test_multiselect_groups.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/views/__init__.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/views/deadline_listview.py
+-rw-r--r--   0        0        0    20342 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/views/manage_deadline_view.py
+-rw-r--r--   0        0        0     8626 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/views/multiselect_groups_view.py
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/views/viewutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_detektor/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_detektor/models.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_detektor/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_detektor/migrations/0002_auto_20180119_1137.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_detektor/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_developemail/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_developemail/admin.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_developemail/email_backend.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_developemail/models.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_developemail/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_developemail/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/models.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/rq_backend.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/rq_jobs.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/comment_email/__init__.py
+-rw-r--r--   0        0        0    12374 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/comment_email/comment_email.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/deadline_email/__init__.py
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/deadline_email/deadline_email.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/feedback_email/__init__.py
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/feedback_email/feedback_email.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/groupinvite_email/__init__.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/groupinvite_email/groupinvite_email.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/management/commands/__init__.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/management/commands/devilry_send_testemail.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/templates/devilry_email/comment_email/comment.txt
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/templates/devilry_email/deadline_email/deadline_moved.txt
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/templates/devilry_email/deadline_email/new_attempt.txt
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/templates/devilry_email/feedback_email/assignment_feedback_student.txt
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/templates/devilry_email/groupinvite_email/accepted.txt
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/templates/devilry_email/groupinvite_email/invite.txt
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/templates/devilry_email/groupinvite_email/rejected.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/templatetags/__init__.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/templatetags/comment_email_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/tests/__init__.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/tests/test_bulk_feedback.py
+-rw-r--r--   0        0        0    68868 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/tests/test_comment_email.py
+-rw-r--r--   0        0        0    17611 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/tests/test_deadline_email.py
+-rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_email/tests/test_feedback_email.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_errortemplates/__init__.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_errortemplates/views.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_errortemplates/static/devilry_errortemplates/style.css
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_errortemplates/templates/devilry_errortemplates/404.django.html
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_errortemplates/templates/devilry_errortemplates/500.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/__init__.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/models.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tasks.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/cradminextensions/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/cradminextensions/devilry_crinstance_examiner.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/cradminextensions/devilry_crmenu_examiner.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_create_feedback.django.html
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_new_attempt.django.html
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/grouplist.django.html
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/includes/batchdownload_assignment.django.html
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/column_header_item.django.html
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/grade_cell_value.django.html
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/group_cell_value.django.html
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/simple_group_bulk_feedbackview.django.html
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/text_cell_value.django.html
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/dashboard/assignmentlist.django.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign-group-item-value.django.html
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templatetags/__init__.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/templatetags/devilry_examiner_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_assignment/__init__.py
+-rw-r--r--   0        0        0    31945 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_assignment/test_batchdownload_api.py
+-rw-r--r--   0        0        0    35476 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_assignment/test_batchframework_tasks.py
+-rw-r--r--   0        0        0    65831 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback.py
+-rw-r--r--   0        0        0    28101 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback_simple.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_assignment/test_crinstance_assignment.py
+-rw-r--r--   0        0        0   126915 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_assignment/test_grouplist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_cradminextensions/__init__.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_cradminextensions/test_devilry_crmenu_examiner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_dashboard/__init__.py
+-rw-r--r--   0        0        0    34779 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_dashboard/test_assignmentlist.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_dashboard/test_crinstance_dashboard.py
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_api.py
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_crinstance_selfassign.py
+-rw-r--r--   0        0        0    36880 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_grouplist.py
+-rw-r--r--   0        0        0    12281 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/__init__.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/crinstance_assignment.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/grouplist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/__init__.py
+-rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py
+-rw-r--r--   0        0        0    11506 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_manage_deadline.py
+-rw-r--r--   0        0        0    11298 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_operations_grouplist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/download_files/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/download_files/backends.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/download_files/batch_download_api.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/download_files/download_archive.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/dashboard/__init__.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/dashboard/assignmentlist.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/dashboard/crinstance_dashboard.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/selfassign/__init__.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/selfassign/api.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/selfassign/crinstance_selfassign.py
+-rw-r--r--   0        0        0    10002 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/selfassign/selfassign.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_examiner/views/selfassign/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/__init__.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/crinstance_frontpage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/cradminextensions/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/cradminextensions/devilry_crmenu_frontpage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/cradminextensions/listbuilder/__init__.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/cradminextensions/listbuilder/listbuilder_role.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/templates/devilry_frontpage/base.django.html
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/templates/devilry_frontpage/frontpage.django.html
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/tests/__init__.py
+-rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/tests/test_frontpage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/tests/test_cradminextensions/__init__.py
+-rw-r--r--   0        0        0    11517 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/tests/test_cradminextensions/test_listbuilder_role.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/views/__init__.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_frontpage/views/frontpage.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/models.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/urls.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/templates/devilry_gradeform/advanced.editable.gradeform.django.html
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/templates/devilry_gradeform/advanced.gradeform.django.html
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/templates/devilry_gradeform/base.django.html
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/templates/devilry_gradeform/create.gradeform.django.html
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/templates/devilry_gradeform/setup.gradeform.django.html
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/templatetags/__init__.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/templatetags/devilry_gradeform_tags.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/views/__init__.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/views/editable_gradeform.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/views/grade_form.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/views/points_grade_form.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/views/setup_create_gradeform.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/views/setup_gradeform.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradeform/views/viewable_gradeform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/__init__.py
+-rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/models.py
+-rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/pluginregistry.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/urls.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/migrations/0001_initial.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/migrations/0002_auto_20170108_0948.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/migrations/__init__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/bulkeditfeedbackbuttonbar.django.html
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/editfeedbackbuttonbar.django.html
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/editfeedbackbuttonbar_savedraftonly.django.html
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackbulkeditorbase.django.html
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_bulkpreview.django.html
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_preview.django.html
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackeditorbase.django.html
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/backandforward-bar.django.html
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/backbutton-bar.django.html
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/backward-button.django.html
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/base.django.html
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/currentprogress.django.html
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/forward-button.django.html
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/reconfigurebase.django.html
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/select_points_to_grade_mapper.django.html
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/selectplugin.django.html
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setmaxpoints.django.html
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setpassing_grade_min_points.django.html
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setup_custom_table.django.html
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/summary.django.html
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/use-this-button.django.html
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/editmarkdown.django.html
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/feedbackeditorfilewidget.django.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/__init__.py
+-rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/helpers.py
+-rw-r--r--   0        0        0    10027 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/test_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/__init__.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/test_download_feedbackdraftfile.py
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/test_feedbackdraft_preview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/__init__.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/base.py
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_select_points_to_grade_mapper.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_selectplugin.py
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_setmaxpoints.py
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_setpassing_grade_min_points.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_setup_custom_table.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_summary.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/__init__.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/download_feedbackdraftfile.py
+-rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/feedbackbulkeditorbase.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/feedbackdraft_bulkpreview.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/feedbackdraft_preview.py
+-rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/feedbackeditorbase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/__init__.py
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/base.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/select_points_to_grade_mapper.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/selectplugin.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/setmaxpoints.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/setpassing_grade_min_points.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/setup_custom_table.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/summary.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/widgets/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/widgets/editfeedbackbuttonbar.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/widgets/editmarkdown.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystem/widgets/filewidget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_approved/__init__.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_approved/apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_approved/models.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_approved/urls.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_approved/templates/devilry_gradingsystemplugin_approved/feedbackbulkeditor.django.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_approved/templates/devilry_gradingsystemplugin_approved/feedbackeditor.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_approved/views/__init__.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_approved/views/feedbackeditor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_points/__init__.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_points/apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_points/models.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_points/urls.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_points/templates/devilry_gradingsystemplugin_points/feedbackbulkeditor.django.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_points/templates/devilry_gradingsystemplugin_points/feedbackeditor.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_points/views/__init__.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_points/views/feedbackeditor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/__init__.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/admin.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/apps.py
+-rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/devilry_group_baker_factories.py
+-rw-r--r--   0        0        0    34983 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/models.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tasks.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/urls.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/cradmin_instances/__init__.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/cradmin_instances/crinstance_admin.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/cradmin_instances/crinstance_base.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/cradmin_instances/crinstance_examiner.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/cradmin_instances/crinstance_student.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/feedbackfeed_builder/__init__.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/feedbackfeed_builder/builder_base.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_sidebarbuilder.py
+-rw-r--r--   0        0        0    10659 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_timelinebuilder.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0001_initial.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0002_feedbackset_gradeform_json.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0003_auto_20160106_1418.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0004_auto_20160107_0918.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0005_auto_20160107_0958.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0006_auto_20160107_1000.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0007_auto_20160107_1031.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0008_auto_20160107_1053.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0009_auto_20160107_1100.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0010_auto_20160107_1106.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0011_auto_20160107_1111.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0012_auto_20160107_1129.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0013_auto_20160110_1621.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0014_feedbackset_grading_status.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0015_auto_20160111_1245.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0016_auto_20160114_2202.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0017_auto_20160122_1518.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0018_auto_20160122_1712.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0019_auto_20160822_1945.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0019_auto_20160912_1649.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0020_feedbackset_ignored_datetime.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0021_merge.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0022_auto_20170103_2308.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0023_auto_20170104_0551.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0024_auto_20170107_1838.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0025_auto_20170124_1504.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0026_datamigrate_update_for_no_none_values_in_feedbackset_deadline.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0027_auto_20170206_1146.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0027_auto_20170207_1951.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0028_auto_20170208_1344.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0029_merge.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0030_auto_20170621_1734.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0031_groupcomment_v2_id.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0032_auto_20180214_1654.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0033_feedbacksetgradingupdatehistory.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0034_feedbackset_last_updated_by.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/0035_groupcommentedithistory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/migrations/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/base.django.html
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed.django.html
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_guidelines.django.html
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/group_comment_edit_base.django.html
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_base.django.html
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_discuss.django.html
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_examiner_admin_discuss.django.html
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_base.django.html
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_delete_groupcomment.html
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_discuss.django.html
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_examiner_admin_discuss.django.html
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_feedback.django.html
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/group_comment_history/comment_history.django.html
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/group_comment_history/history_item_value.django.html
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/admin_commentform_discuss_examiner_headingtext.django.html
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/admin_commentform_discuss_public_headingtext.django.html
+-rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/batch_download_archive_script.django.html
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/buttonbar.django.html
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/comments_disabled.django.html
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/examiner.editlastdelivery.django.html
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/examiner_commentform_discuss_examiner_headingtext.django.html
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/examiner_commentform_discuss_public_headingtext.django.html
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/fileupload.django.html
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/groupcomment_edit_delete_option.html
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/student_commentform_headingtext.django.html
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/admin_groupcomment_item_value.django.html
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/base_event_item_value.django.html
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/base_groupcomment_item_value.django.html
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/deadline_expired_item_value.django.html
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/deadline_moved_item_value.django.html
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/examiner_groupcomment_item_value.django.html
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/feedbackset_info_item_value.django.html
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_item_value.django.html
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_updated_item_value.django.html
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/student_groupcomment_item_value.django.html
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/base_sidebar_file_item_value.django.html
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_comment_item_value.django.html
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_feedbackset_item_value.django.html
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_file_item_value.django.html
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_list.django.html
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/template_tags/devilry_group_comment_user_is_none.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templatetags/__init__.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/templatetags/devilry_group_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/__init__.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_devilry_group_mommy_factories.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_templatetags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_crinstance/__init__.py
+-rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_crinstance/test_crinstance_admin.py
+-rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_crinstance/test_crinstance_examiner.py
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_crinstance/test_crinstance_student.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_download/__init__.py
+-rw-r--r--   0        0        0    21694 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_download/test_batchdownload_api.py
+-rw-r--r--   0        0        0    10095 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_download/test_batchframework_compression.py
+-rw-r--r--   0        0        0    17151 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_download/test_feedbackfeed_bulkfiledownload.py
+-rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_download/test_feedbackfeed_filedownload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/admin/__init__.py
+-rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/admin/test_comment_edit_history.py
+-rw-r--r--   0        0        0    37226 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/admin/test_feedbackfeed_admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/__init__.py
+-rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_comment_edit_history.py
+-rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_delete_comment.py
+-rw-r--r--   0        0        0    50866 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_discuss.py
+-rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_comment.py
+-rw-r--r--   0        0        0    13104 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_grade.py
+-rw-r--r--   0        0        0    37037 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_feedback.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/__init__.py
+-rw-r--r--   0        0        0    30200 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_admin.py
+-rw-r--r--   0        0        0    25291 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_common.py
+-rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_examiner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/student/__init__.py
+-rw-r--r--   0        0        0    14087 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/student/test_comment_edit_history.py
+-rw-r--r--   0        0        0   109725 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/student/test_feedbackfeed_student.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed_builders/__init__.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_sidebarbuilder.py
+-rw-r--r--   0        0        0    21620 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_timeline_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_models/__init__.py
+-rw-r--r--   0        0        0    18792 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_models/test_feedback_set.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_models/test_feedbackfeed_model.py
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_models/test_feedbackset_passed_pervious_period.py
+-rw-r--r--   0        0        0    17503 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/tests/test_models/test_group_comment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/utils/__init__.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/utils/download_response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/__init__.py
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/cradmin_comment_history.py
+-rw-r--r--   0        0        0    24391 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/cradmin_feedbackfeed_base.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/group_comment_edit_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/admin/__init__.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/admin/feedbackfeed_admin.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/admin/group_comment_history.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/admin/manage_deadline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/download_files/__init__.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/download_files/backends.py
+-rw-r--r--   0        0        0    15946 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/download_files/batch_download_api.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/download_files/batch_download_files.py
+-rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/download_files/feedbackfeed_bulkfiledownload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/examiner/__init__.py
+-rw-r--r--   0        0        0    21474 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/examiner/feedbackfeed_examiner.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/examiner/group_comment_history.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/examiner/manage_deadline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/student/__init__.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/student/feedbackfeed_student.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_group/views/student/group_comment_history.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/models.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/urls.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/templates/devilry_header/about_me.django.html
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/templates/devilry_header/app.django.html
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/templates/devilry_header/header2_extjsinclude.django.html
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/templates/devilry_header/header2include.django.html
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/templates/devilry_header/includes/change_language.django.html
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/tests/__init__.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/tests/test_aboutme.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/tests/test_change_language.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/views/__init__.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/views/about_me.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_header/views/change_language.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_help/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_help/tests.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_help/urls.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_help/views.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_help/templates/devilry_help/help.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_i18n/__init__.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_i18n/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_i18n/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/__init__.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporter.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/models.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/management/commands/__init__.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/management/commands/devilry_import_v2_database.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/migrations/0001_initial.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/migrations/0002_auto_20190624_1238.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/migrations/0003_auto_20210427_1350.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/migrations/__init__.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/__init__.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/assignment_importer.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/assignmentgroup_importer.py
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/candidate_examiner_importer.py
+-rw-r--r--   0        0        0    13855 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/delivery_feedback_importers.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/feedbackset_importer.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/modelimporter_utils.py
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/node_importer.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/period_importer.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/pointrange_to_grade_importer.py
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/qualifiesforexam_importer.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/relateduser_importer.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/subject_importer.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/user_importer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/scripts/__init__.py
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/scripts/user_add_missing_data_from_json.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/__init__.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/importer_testcase_mixin.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentgroupimporter.py
+-rw-r--r--   0        0        0    11674 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentimporter.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_candidateimporter.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_commentfilecontentimporter.py
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_deliveryimporter.py
+-rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_examinerimporter.py
+-rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_feedbacksetimporter.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_filemetaimporter.py
+-rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_nodeimporter.py
+-rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_periodimporter.py
+-rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointrangetogradeimporter.py
+-rw-r--r--   0        0        0     7374 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointtogrademapimporter.py
+-rw-r--r--   0        0        0    14419 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_qualifiesforexam_importer.py
+-rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedexaminerimporter.py
+-rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedstudentimporter.py
+-rw-r--r--   0        0        0    22341 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_staticfeedbackimporter.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_subjectimporter.py
+-rw-r--r--   0        0        0     8108 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_userimporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_scripts/__init__.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_scripts/test_user_add_missing_data_from_json.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/__init__.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2assignment_directoryparser.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2assignmentgroup_directoryparser.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2candidate_directoryparser.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2deadline_directoryparser.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2delivery_directoryparser.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2examiner_directoryparser.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2filemeta_directoryparser.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2node_directoryparser.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2period_directoryparser.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2pointrangetograde_directoryparser.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2pointtogrademap_directoryparser.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2qualifiesforexam_finalexam_directoryparser.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2qualifiesforexam_status_directoryparser.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2relatedexaminer_directoryparser.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2relatedstudent_directoryparser.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2staticfeedback_directoryparser.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2subject_directoryparser.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/v2user_directoryparser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_markup/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_markup/models.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_markup/parse_markdown.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_markup/urls.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_markup/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_markup/markdown_extensions/__init__.py
+-rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_markup/markdown_extensions/code_diff.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_markup/markdown_extensions/latex_math.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_markup/templates/devilry_markup/code_diff.html
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_markup/templates/devilry_markup/latex_math.html
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_markup/templates/markup/load_latex_support.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/admin.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/migrations/0002_auto_20210427_1350.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/migrations/0003_alter_message_context_type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/migrations/__init__.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/models/__init__.py
+-rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/models/base.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/templates/devilry_message/for_test.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/tests/__init__.py
+-rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/tests/test_message.py
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/tests/test_message_receiver.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/utils/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_message/utils/subject_generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/__init__.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/admin.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/apps.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/cradmin_app.py
+-rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/models.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/pluginhelpers.py
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/plugintyperegistry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/listbuilder/__init__.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/listbuilder/plugin_listbuilder_list.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/migrations/0001_initial.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/migrations/0002_auto_20170223_1112.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/migrations/0003_auto_20170629_1914.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/migrations/0004_auto_20210427_1350.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/migrations/0005_deletedqualifiesforfinalexam.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tablebuilder/__init__.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tablebuilder/tablebuilder.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/base.django.html
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/list_statuses.django.html
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/print_view.html
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/retract_status.django.html
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/selectplugin.django.html
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_preview.django.html
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_show.html
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/includes/qualification_table.django.html
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/description.django.html
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/plugin_item_value.django.html
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/tablebuilder/qualificationstatus_valueitem.django.html
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/tablebuilder/relatedstudent_valueitem.django.html
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/tablebuilder/tableheader_valueitem.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/__init__.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_list_statuses_view.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_models.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_plugin_listbuilder_list.py
+-rw-r--r--   0        0        0    16296 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_pluginhelpers.py
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_pluginselection_view.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_plugintyperegistry.py
+-rw-r--r--   0        0        0    17221 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_preview.py
+-rw-r--r--   0        0        0    22999 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_showstatus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/utils/__init__.py
+-rw-r--r--   0        0        0    21904 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/utils/groups_groupedby_relatedstudent_and_assignments.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/views/__init__.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/views/list_statuses_view.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/views/plugin_mixin.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/views/pluginselection_view.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/views/proxyview.py
+-rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/views/qualification_preview_view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/views/plugin_base_views/__init__.py
+-rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/views/plugin_base_views/base_multiselect_view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/__init__.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/apps.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/models.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/plugin.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/resultscollector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/tests/__init__.py
+-rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/tests/test_resultscollector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/views/__init__.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/views/select_assignment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_points/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_points/apps.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_points/models.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_points/plugin.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_points/resultscollector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_points/tests/__init__.py
+-rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_points/tests/test_resultscollector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_points/views/__init__.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_points/views/select_assignment_and_points.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_students/__init__.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_students/apps.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_students/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_students/tests/__init__.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_students/tests/test_student_selection_view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_students/views/__init__.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_students/views/select_students.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/__init__.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/abstract_generator.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/admin.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/generator_registry.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/models.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/rq_task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/urls.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/migrations/0001_initial.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/migrations/0002_auto_20210427_1350.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/migrations/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/templates/devilry_report/download_report.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/tests/__init__.py
+-rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/tests/test_download_report_view.py
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/tests/test_generator_registry.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/tests/test_report_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/views/__init__.py
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_report/views/download_report.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_resetpassword/__init__.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_resetpassword/urls.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_rest/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_rest/__init__.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_rest/auth.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_rest/formfields.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_rest/models.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_rest/serializehelpers.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_rest/testclient.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_rest/tests/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_rest/tests/test_serializehelpers.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_sandbox/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_sandbox/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_sandbox/models.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_sandbox/sandbox.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_sandbox/urls.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_sandbox/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_sandbox/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_sandbox/management/commands/__init__.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_sandbox/management/commands/devilry_sandboxcreate.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_sandbox/templates/devilry_sandbox/createsubject.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_settings/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_settings/models.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_settings/urls.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_settings/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/__init__.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/api/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/api/assignment/__init__.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/api/assignment/api_utils.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/api/assignment/examiner_average_grading_points.py
+-rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/api/assignment/examiner_details.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/api/assignment/examiner_group_results.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/management/commands/__init__.py
+-rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/management/commands/devilry_create_test_course.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/management/commands/devilry_statistics_make_assignment_with_graded_groups.py
+-rw-r--r--   0        0        0   606439 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/static/devilry_statistics/6.0.0rc2/devilry_statistics_all.js
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/.babelrc
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/.editorconfig
+-rw-r--r--   0        0        0   475670 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/package-lock.json
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/package.json
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/webpack.config.js
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/devilry_statistics_all.js
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerAverageGradingPointsWidget.js
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerDetailsWidget.js
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerGroupResultWidget.js
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/registerAllWidgets.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/tests/__init__.py
+-rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/tests/test_api_examiner_average_grading_points.py
+-rw-r--r--   0        0        0    18649 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/tests/test_api_examiner_details.py
+-rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_statistics/tests/test_api_examiner_group_result.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/__init__.py
+-rw-r--r--   0        0        0     5154 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/models.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/cradminextensions/__init__.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/cradminextensions/columntypes.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/cradminextensions/devilry_crinstance_student.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/cradminextensions/devilry_crmenu_student.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/cradminextensions/studentobjecttable.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/migrations/__init__.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/add_delivery.django.html
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/contactapp/contact.django.html
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery-number-column.django.html
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery-status-column.django.html
+-rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_details.django.html
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_list.django.html
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/overviewapp/overview.django.html
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_delete.django.html
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond.django.html
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond_standalone.django.html
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/projectgroup_overview.django.html
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_period/assignmentsapp/assignmentgroup-list.django.html
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_period/assignmentsapp/statuscolumn.django.html
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_student/allperiods/allperiods.django.html
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_student/recentdeliveriesapp/delivery-summary-with-assignment-column.django.html
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_student/waitingfordeliveriesapp/last-deadline.django.html
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_student/waitingfordeliveriesapp/waiting-for-deliveries-list.django.html
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/delivery-summary-column.django.html
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/naturaltime-and-datetime-column.django.html
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/naturaltime-column.django.html
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/dashboard/dashboard.django.html
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/include/feedback-rendered-view.django.html
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/include/group_breadcrumb.django.html
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/period/overview.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templatetags/__init__.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/templatetags/devilry_student_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/tests/__init__.py
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/tests/test_models.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/tests/test_templatetags.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/tests/upload_testfile1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/tests/test_cradminextensions/__init__.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/tests/test_cradminextensions/test_devilry_crmenu_student.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/tests/test_dashboard/__init__.py
+-rw-r--r--   0        0        0    14380 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/tests/test_dashboard/test_allperiods.py
+-rw-r--r--   0        0        0    41388 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/tests/test_dashboard/test_dashboard.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/tests/test_group/__init__.py
+-rw-r--r--   0        0        0    88623 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/tests/test_group/test_projectgroupapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/tests/test_period/__init__.py
+-rw-r--r--   0        0        0    28524 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/tests/test_period/test_overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/views/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/views/show_delivery.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/views/dashboard/__init__.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/views/dashboard/allperiods.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/views/dashboard/crinstance_dashboard.py
+-rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/views/dashboard/dashboard.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/views/group/__init__.py
+-rw-r--r--   0        0        0    14862 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/views/group/projectgroupapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/views/period/__init__.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/views/period/crinstance_period.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_student/views/period/overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/models.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tasks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/delete_periods/__init__.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/delete_periods/period_delete.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/examples/relatedexaminers.json
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/examples/relatedstudents.json
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/examples/relatedstudents_email_instead_of_username.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_anonymize_database.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_clear_allauth_account_tables.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_compressed_archives.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_inactive_users.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_message_receivers.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_messages_without_receivers.py
+-rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_periods.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_fix_missing_first_feedbackset.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_mark_as_passed_in_previous_period.py
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodadd.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodadminadd.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodadminclear.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodsearch.py
+-rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedexaminers.py
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedstudents.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_permissiongroup_add_subject.py
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_qualifiedforfinalexam_delete_duplicates.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_rename_periodtag_prefix.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_resend_failed_messages.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_setup_dataporten_provider.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_setup_primary_domain.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_show_assignment_guidelines.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectadd.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectadminadd.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectadminclear.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectsearch.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_test_rq_task.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_useradd.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_useraddbulk.py
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_usermerge.py
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_usermod.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/__init__.py
+-rw-r--r--   0        0        0    14750 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_inactive_users.py
+-rw-r--r--   0        0        0    19826 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_periods.py
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminadd.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminclear.py
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_permissiongroup_add_subject.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_qualifiedforfinalexam_delete_duplicates.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadd.py
+-rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminadd.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminclear.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_useraddbulk.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_usermod.py
+-rw-r--r--   0        0        0     7755 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_resend_failed_messages.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/models.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/urls.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/views.py
+-rw-r--r--   0        0        0    40723 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/media/images/groovepaper.png
+-rw-r--r--   0        0        0    14235 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/media/images/favicons/apple-touch-icon.png
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/media/images/favicons/favicon.ico
+-rw-r--r--   0        0        0    65078 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/devilry_all.js
+-rw-r--r--   0        0        0   474892 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/devilry_all.js.map
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/katex/LICENSE
+-rw-r--r--   0        0        0    23112 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/katex/katex.min.css
+-rw-r--r--   0        0        0   598523 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/katex/katex.mjs
+-rw-r--r--   0        0        0    27456 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/commentEditor.js
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/cookie.js
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/examinerSelfAssignButton.js
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/feedbackfeedNavigationHandler.js
+-rw-r--r--   0        0        0    20380 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/fileupload.js
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/helloWorld.js
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/latex_math.js
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/webcomponent_utils.js
+-rw-r--r--   0        0        0   292259 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/styles/cradmin_theme_devilry_mainpages/theme.css
+-rw-r--r--   0        0        0   220567 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/styles/cradmin_theme_devilry_superuserui/theme.css
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/templates/devilry_deploy/custom_css.django.css
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/templates/devilry_deploy/custom_css_base.django.html
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/templates/devilry_deploy/footer.django.html
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/templates/devilry_deploy/footer_base.django.html
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/templates/devilry_deploy/frontpage_footer.django.html
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/templates/devilry_deploy/login_footer.django.html
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/templates/devilry_theme3/favicons.django.html
+-rw-r--r--   0        0        0    25100 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/templates/devilry_theme3/wcag-debug.django.html
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/templates/devilry_theme3/include/devilry_all_js.django.html
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/templates/devilry_theme3/include/includetest.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/templatetags/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/devilry_theme3/templatetags/devilry_theme3_tags.py
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/django_decoupled_docs/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/django_decoupled_docs/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/django_decoupled_docs/models.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/django_decoupled_docs/registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/django_decoupled_docs/templatetags/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/django_decoupled_docs/templatetags/django_decoupled_docs_tags.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   265490 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/locale/en/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0   174397 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   371133 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/locale/nb/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/__init__.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/log.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/settingsproxy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/cradmin_legacy_settings.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/default_urls.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/devilry_test_runner.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/docproxies.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/http_error_handlers.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/i18n.py
+-rw-r--r--   0        0        0     9810 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/projectspecific_settings.py
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/settings.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/templatecontext.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/formats/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/formats/en/__init__.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/formats/en/formats.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/formats/nb/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/formats/nb/formats.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/management/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/management/commands/__init__.py
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/common/management/commands/devilry_common_merge_candidates.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/__init__.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/dev_urls.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/fabrictasks.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/models.py
+-rw-r--r--   0        0        0   353927 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/dumps/old_default.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/management/commands/__init__.py
+-rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/management/commands/devilry_developer_create_deliveries_from_filesystemtree.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/management/commands/devilry_developer_delete_all_except_users.py
+-rw-r--r--   0        0        0    15531 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/management/commands/devilry_developer_performance_test_db.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/management/commands/devilry_developer_set_all_passwords_to_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/settings/__init__.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/settings/base.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/settings/codeship_test.py
+-rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/settings/develop.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/settings/docs.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/settings/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/testhelpers/__init__.py
+-rw-r--r--   0        0        0    22236 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/testhelpers/corebuilder.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/testhelpers/datebuilder.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/testhelpers/login.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/testhelpers/skip_rq_tests.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/develop/testhelpers/soupselect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/production/__init__.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/production/settings.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/production/urls.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/project/production/wsgi.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/GroupAssignments.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/GroupNodes.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/OrderedDictFallback.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/__init__.py
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/anonymize_database.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/command.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/create_absolute_url.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/custom_templates.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/datetimeutils.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/delay_middleware.py
+-rw-r--r--   0        0        0     8118 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/delivery_collection.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/devilry_djangoaggregate_functions.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/devilry_email.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/dictutils.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/filewrapperwithexplicitclose.py
+-rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/groups_groupedby_relatedstudent_and_assignment.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/importutils.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/logexceptionsmiddleware.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/management.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/migrationutils.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/models.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/module.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/nodenamesuggestor.py
+-rw-r--r--   0        0        0    11545 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/passed_in_previous_period.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/profile.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/rq_setup.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/setting_utils.py
+-rw-r--r--   0        0        0     7675 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/stream_archives.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/verify_unique_entries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/api/__init__.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/api/api_test_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/demodb/__init__.py
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/demodb/demousers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/graphviz/__init__.py
+-rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/graphviz/djangomodels.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/graphviz/dot.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/graphviz/sphinx.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/tests/delivery_collection_tests.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/tests/importutils.py
+-rwxr-xr-x   0        0        0     7534 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/tests/streamable_archive_tests.py
+-rw-r--r--   0        0        0    15352 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/tests/test_anonymize_db.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/tests/test_datetimeutils.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/tests/test_groups_groupedby_relatedstudent_and_assignment.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/tests/test_nodenamesuggestor.py
+-rw-r--r--   0        0        0    47879 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/tests/test_passed_in_previous_period.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/tests/test_setting_utils.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/devilry/utils/tests/test_url_datetime.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/README.md
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 devilry-6.0.0rc2/PKG-INFO
```

### Comparing `devilry-6.0.0rc1/devilry/.coveragerc` & `devilry-6.0.0rc2/devilry/.coveragerc`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/admin.py` & `devilry-6.0.0rc2/devilry/apps/core/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/baker_recipes.py` & `devilry-6.0.0rc2/devilry/apps/core/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/deliverystore.py` & `devilry-6.0.0rc2/devilry/apps/core/deliverystore.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/devilry_core_baker_factories.py` & `devilry-6.0.0rc2/devilry/apps/core/devilry_core_baker_factories.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/group_user_lookup.py` & `devilry-6.0.0rc2/devilry/apps/core/group_user_lookup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/testhelper.py` & `devilry-6.0.0rc2/devilry/apps/core/testhelper.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/testhelpers.py` & `devilry-6.0.0rc2/devilry/apps/core/testhelpers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0002_auto_20150915_1127.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0002_auto_20150915_1127.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0003_auto_20150917_1537.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0003_auto_20150917_1537.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0009_assignmentgroup_batchoperation.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0009_assignmentgroup_batchoperation.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0010_assignment_anonymizationmode.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0010_assignment_anonymizationmode.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0011_datamigrate_anonymous_to_anonymizationmode.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0011_datamigrate_anonymous_to_anonymizationmode.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0013_auto_20160111_2021.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0013_auto_20160111_2021.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0015_assignment_uses_custom_candidate_ids.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0015_assignment_uses_custom_candidate_ids.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0017_candidate_relatedstudent_replaces_student_field.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0017_candidate_relatedstudent_replaces_student_field.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0018_auto_20160112_1923.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0018_auto_20160112_1923.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0019_auto_20160113_2037.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0019_auto_20160113_2037.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0021_examiner_relatedexaminer_replaces_user_field.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0021_examiner_relatedexaminer_replaces_user_field.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0027_auto_20160116_1843.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0027_auto_20160116_1843.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0029_assignmentgrouphistory.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0029_assignmentgrouphistory.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0030_auto_20170124_1504.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0030_auto_20170124_1504.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0031_auto_20170125_1601.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0031_auto_20170125_1601.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0032_datamigrate_update_for_no_none_values_in_assignment_firstdeadline.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0032_datamigrate_update_for_no_none_values_in_assignment_firstdeadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0033_auto_20170220_1330.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0033_auto_20170220_1330.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0034_auto_20170303_1308.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0034_auto_20170303_1308.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0037_auto_20170620_1515.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0037_auto_20170620_1515.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0038_auto_20170621_1720.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0038_auto_20170621_1720.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0040_auto_20180214_1654.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0040_auto_20180214_1654.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0041_auto_20180220_0651.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0041_auto_20180220_0651.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0042_candidateassignmentgrouphistory_examinerassignmentgrouphistory.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0042_candidateassignmentgrouphistory_examinerassignmentgrouphistory.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0043_auto_20180302_1139.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0043_auto_20180302_1139.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0044_auto_20190624_1238.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0044_auto_20190624_1238.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/migrations/0046_auto_20220519_1043.py` & `devilry-6.0.0rc2/devilry/apps/core/migrations/0046_auto_20220519_1043.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/__init__.py` & `devilry-6.0.0rc2/devilry/apps/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/abstract_applicationkeyvalue.py` & `devilry-6.0.0rc2/devilry/apps/core/models/abstract_applicationkeyvalue.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/abstract_is_candidate.py` & `devilry-6.0.0rc2/devilry/apps/core/models/abstract_is_candidate.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/abstract_is_examiner.py` & `devilry-6.0.0rc2/devilry/apps/core/models/abstract_is_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/assignment.py` & `devilry-6.0.0rc2/devilry/apps/core/models/assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/assignment_group.py` & `devilry-6.0.0rc2/devilry/apps/core/models/assignment_group.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/assignment_group_history.py` & `devilry-6.0.0rc2/devilry/apps/core/models/assignment_group_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/basenode.py` & `devilry-6.0.0rc2/devilry/apps/core/models/basenode.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/candidate.py` & `devilry-6.0.0rc2/devilry/apps/core/models/candidate.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/custom_db_fields.py` & `devilry-6.0.0rc2/devilry/apps/core/models/custom_db_fields.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/deadline.py` & `devilry-6.0.0rc2/devilry/apps/core/models/deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/delivery.py` & `devilry-6.0.0rc2/devilry/apps/core/models/delivery.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/devilryuserprofile.py` & `devilry-6.0.0rc2/devilry/apps/core/models/devilryuserprofile.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/examiner.py` & `devilry-6.0.0rc2/devilry/apps/core/models/examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/examiner_candidate_group_history.py` & `devilry-6.0.0rc2/devilry/apps/core/models/examiner_candidate_group_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/filemeta.py` & `devilry-6.0.0rc2/devilry/apps/core/models/filemeta.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/groupinvite.py` & `devilry-6.0.0rc2/devilry/apps/core/models/groupinvite.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import django_rq
 from django.core.exceptions import ValidationError
 from django.urls import reverse
 from django.db import models
 from django.db import transaction
 from django.utils import timezone
 from django.utils.translation import gettext_lazy
 
 from devilry.apps.core.models import Assignment
 from devilry.apps.core.models import Candidate
 from devilry.devilry_account.models import User
-from devilry.utils.devilry_email import send_templated_message
+from devilry.devilry_email.groupinvite_email import send_invite_email, \
+    send_accepted_email, send_rejected_email
 from .assignment_group import AssignmentGroup
 
 
 class GroupInviteQuerySet(models.QuerySet):
     def filter_accepted(self):
         """
         Filter all :class:`.GroupInvite` objects that has been accepted
@@ -213,27 +215,25 @@
         source = AssignmentGroup.objects.filter_user_is_candidate(self.sent_to) \
             .filter(parentnode=self.group.parentnode) \
             .get()
         with transaction.atomic():
             source.merge_into(self.group)
 
     def _send_response_notification(self):
-        sent_to_displayname = self.sent_to.get_full_name()
+        queue = django_rq.get_queue(name='email')
         if self.accepted:
-            subject = gettext_lazy('{user} accepted your project group invite').format(user=sent_to_displayname)
-            template_name = 'devilry_core/groupinvite_accepted.django.txt'
+            queue.enqueue(
+                send_accepted_email,
+                groupinvite_id=self.id
+            )
         else:
-            subject = gettext_lazy('{user} rejected your project group invite').format(user=sent_to_displayname)
-            template_name = 'devilry_core/groupinvite_rejected.django.txt'
-        assignment = self.group.assignment
-        send_templated_message(subject, template_name, {
-            'sent_to_displayname': sent_to_displayname,
-            'assignment': assignment.long_name,
-            'subject': assignment.subject.long_name
-        }, self.sent_by)
+            queue.enqueue(
+                send_rejected_email,
+                groupinvite_id=self.id
+            )
 
     def send_invite_notification(self, request):
         """
         Called to send the invite notification. Should be called
         right after creating the invite. Not called in save() to
         make message sending less coupled (to avoid any issues
         with testing and bulk creation of invites).
@@ -247,18 +247,14 @@
             ValueError If ``accepted==None``, or ``id==None``.
 
         """
         if self.accepted is not None:
             raise ValueError(gettext_lazy('Can not send notification for an accepted GroupInvite.'))
         elif self.id is None:
             raise ValueError(gettext_lazy('Can not send notification for an unsaved GroupInvite.'))
-        sent_by_displayname = self.sent_by.get_displayname()
-        assignment = self.group.assignment
-        subject = gettext_lazy('Project group invite for {assignment}').format(assignment=assignment.get_path())
-        template_name = 'devilry_core/groupinvite_invite.django.txt'
-        url = request.build_absolute_uri(reverse('devilry_student_groupinvite_respond', kwargs={'invite_id': self.id}))
-        send_templated_message(subject, template_name, {
-            'sent_by_displayname': sent_by_displayname,
-            'assignment': assignment.long_name,
-            'subject': assignment.subject.long_name,
-            'url': url
-        }, self.sent_to)
+        queue = django_rq.get_queue(name='email')
+        queue.enqueue(
+            send_invite_email,
+            groupinvite_id=self.id,
+            url=request.build_absolute_uri(
+                reverse('devilry_student_groupinvite_respond', kwargs={'invite_id': self.id})
+            ))
```

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/model_utils.py` & `devilry-6.0.0rc2/devilry/apps/core/models/model_utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/period.py` & `devilry-6.0.0rc2/devilry/apps/core/models/period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/period_tag.py` & `devilry-6.0.0rc2/devilry/apps/core/models/period_tag.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/pointrange_to_grade.py` & `devilry-6.0.0rc2/devilry/apps/core/models/pointrange_to_grade.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/relateduser.py` & `devilry-6.0.0rc2/devilry/apps/core/models/relateduser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/save_interface.py` & `devilry-6.0.0rc2/devilry/apps/core/models/save_interface.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/static_feedback.py` & `devilry-6.0.0rc2/devilry/apps/core/models/static_feedback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/models/subject.py` & `devilry-6.0.0rc2/devilry/apps/core/models/subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/comment-summary.django.html` & `devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/comment-summary.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-full-plain.django.html` & `devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-full-plain.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/grade-full.django.html` & `devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/grade-full.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/groupstatus.django.html` & `devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/groupstatus.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/relatedexaminers-on-period-tag.django.html` & `devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/relatedexaminers-on-period-tag.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/templates/devilry_core/templatetags/relatedstudents-on-period-tag.django.html` & `devilry-6.0.0rc2/devilry/apps/core/templates/devilry_core/templatetags/relatedstudents-on-period-tag.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/templates/search/indexes/core/assignmentgroup_text.txt` & `devilry-6.0.0rc2/devilry/apps/core/templates/search/indexes/core/assignmentgroup_text.txt`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/templatetags/devilry_core_tags.py` & `devilry-6.0.0rc2/devilry/apps/core/templatetags/devilry_core_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_assignment.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_assignment_group.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_assignment_group.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_assignment_group_history.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_assignment_group_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_candidate.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_candidate.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_deadline.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_devilry_core_tags.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_devilry_core_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_examiner.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_group_user_lookup.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_group_user_lookup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_groupinvite.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_groupinvite.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from django.urls import reverse
 from model_bakery import baker
 
 from devilry.apps.core import devilry_core_baker_factories as core_baker
 from devilry.apps.core.models import AssignmentGroup
 from devilry.apps.core.models import GroupInvite
 from devilry.devilry_dbcache.customsql import AssignmentGroupDbCacheCustomSql
+from devilry.devilry_message.models import Message, MessageReceiver
 
 
 class TestGroupInviteErrors(TestCase):
     def setUp(self):
         AssignmentGroupDbCacheCustomSql().initialize()
 
     def test_user_sending_is_not_part_of_the_group(self):
@@ -312,24 +313,24 @@
 
     def test_num_queries_accept(self):
         group1 = baker.make('core.AssignmentGroup', parentnode__students_can_create_groups=True)
         group2 = baker.make('core.AssignmentGroup', parentnode=group1.parentnode)
         student1 = core_baker.candidate(group=group1).relatedstudent.user
         student2 = core_baker.candidate(group=group2).relatedstudent.user
         invite = baker.make('core.GroupInvite', sent_by=student1, sent_to=student2, group=group1)
-        with self.assertNumQueries(37):
+        with self.assertNumQueries(45):
             invite.respond(True)
 
     def test_num_queries_reject(self):
         group1 = baker.make('core.AssignmentGroup', parentnode__students_can_create_groups=True)
         group2 = baker.make('core.AssignmentGroup', parentnode=group1.parentnode)
         student1 = core_baker.candidate(group=group1).relatedstudent.user
         student2 = core_baker.candidate(group=group2).relatedstudent.user
         invite = baker.make('core.GroupInvite', sent_by=student1, sent_to=student2, group=group1)
-        with self.assertNumQueries(9):
+        with self.assertNumQueries(17):
             invite.respond(False)
 
     def test_send_invite_mail(self):
         assignment = baker.make(
             'core.Assignment',
             long_name='Assignment 1',
             short_name='assignment1',
@@ -351,14 +352,32 @@
         invite.send_invite_notification(request)
         self.assertEqual(len(mail.outbox), 1)
         self.assertEqual(mail.outbox[0].subject, '[Devilry] Project group invite for Duck1010.s17.assignment1')
         url = request.build_absolute_uri(
             reverse('devilry_student_groupinvite_respond', kwargs={'invite_id': invite.id}))
         self.assertIn(url, mail.outbox[0].body)
 
+        message = Message.objects.get()
+        message_receiver = MessageReceiver.objects.get()
+        self.assertIsNone(message.created_by)
+        self.assertEqual(message.context_type, Message.CONTEXT_TYPE_CHOICES.GROUP_INVITE_INVITATION.value)
+        self.assertDictEqual(message.metadata, {
+            'groupinvite_id': invite.id,
+            'sent_by_user_id': invite.sent_by.id,
+            'sent_to_user_id': invite.sent_to.id
+        })
+        self.assertEqual(message_receiver.user, invite.sent_to)
+        self.assertEqual(message_receiver.subject, 'Project group invite for Duck1010.s17.assignment1')
+        self.assertIn(
+            f'{ invite.sent_by.get_displayname() } invited you to join their project group',
+            message_receiver.message_content_plain
+        )
+        self.assertIn(testgroup.parentnode.long_name, message_receiver.message_content_plain)
+        self.assertIn(testgroup.parentnode.parentnode.parentnode.long_name, message_receiver.message_content_plain.replace('\n', ' '))
+
     def test_send_reject_mail(self):
         assignment = baker.make(
             'core.Assignment',
             long_name='Assignment 1',
             short_name='assignment1',
             parentnode__long_name='Spring2017',
             parentnode__short_name='s17',
@@ -380,14 +399,33 @@
         invite.full_clean()
         invite.save()
         invite.send_invite_notification(self.__fake_request())
         invite.respond(False)
         self.assertEqual(len(mail.outbox), 2)
         self.assertEqual(mail.outbox[1].subject, '[Devilry] Dewey rejected your project group invite')
 
+        self.assertEqual(Message.objects.count(), 2)
+        self.assertEqual(MessageReceiver.objects.count(), 2)
+        message = Message.objects.get(context_type=Message.CONTEXT_TYPE_CHOICES.GROUP_INVITE_REJECTED.value)
+        message_receiver = MessageReceiver.objects.get(message=message)
+        self.assertIsNone(message.created_by)
+        self.assertDictEqual(message.metadata, {
+            'groupinvite_id': invite.id,
+            'sent_by_user_id': invite.sent_by.id,
+            'sent_to_user_id': invite.sent_to.id
+        })
+        self.assertEqual(message_receiver.user, invite.sent_by)
+        self.assertEqual(message_receiver.subject, f'{invite.sent_to.get_full_name()} rejected your project group invite')
+        self.assertIn(
+            f'{ invite.sent_to.get_displayname() } rejected the invite to join your project group',
+            message_receiver.message_content_plain
+        )
+        self.assertIn(testgroup.parentnode.long_name, message_receiver.message_content_plain)
+        self.assertIn(testgroup.parentnode.parentnode.parentnode.long_name, message_receiver.message_content_plain)
+
     def test_send_accept_mail(self):
         assignment = baker.make(
             'core.Assignment',
             long_name='Assignment 1',
             short_name='assignment1',
             parentnode__long_name='Spring2017',
             parentnode__short_name='s17',
@@ -409,14 +447,33 @@
         invite.full_clean()
         invite.save()
         invite.send_invite_notification(self.__fake_request())
         invite.respond(True)
         self.assertEqual(len(mail.outbox), 2)
         self.assertEqual(mail.outbox[1].subject, '[Devilry] Dewey accepted your project group invite')
 
+        self.assertEqual(Message.objects.count(), 2)
+        self.assertEqual(MessageReceiver.objects.count(), 2)
+        message = Message.objects.get(context_type=Message.CONTEXT_TYPE_CHOICES.GROUP_INVITE_ACCEPTED.value)
+        message_receiver = MessageReceiver.objects.get(message=message)
+        self.assertIsNone(message.created_by)
+        self.assertDictEqual(message.metadata, {
+            'groupinvite_id': invite.id,
+            'sent_by_user_id': invite.sent_by.id,
+            'sent_to_user_id': invite.sent_to.id
+        })
+        self.assertEqual(message_receiver.user, invite.sent_by)
+        self.assertEqual(message_receiver.subject, f'{invite.sent_to.get_full_name()} accepted your project group invite')
+        self.assertIn(
+            f'{ invite.sent_to.get_displayname() } accepted the invite to join your project group',
+            message_receiver.message_content_plain
+        )
+        self.assertIn(testgroup.parentnode.long_name, message_receiver.message_content_plain)
+        self.assertIn(testgroup.parentnode.parentnode.parentnode.long_name, message_receiver.message_content_plain)
+
     def test_send_invite_to_choices_queryset(self):
         group1 = baker.make('core.AssignmentGroup', parentnode__students_can_create_groups=True)
         group2 = baker.make('core.AssignmentGroup', parentnode=group1.parentnode)
         group3 = baker.make('core.AssignmentGroup', parentnode=group1.parentnode)
         group4 = baker.make('core.AssignmentGroup', parentnode=group1.parentnode)
         core_baker.candidate(group=group1, fullname="Louie", shortname="louie")
         core_baker.candidate(group=group2, fullname="Huey", shortname="huey")
```

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_period.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_period_tags.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_period_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_pointrange_to_grade.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_pointrange_to_grade.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,14 @@
         self.assertEqual(pointrange_to_grade2, assignment2.pointtogrademap.points_to_grade(2))
 
         # When we update to Django 1.5+, this should start only
         # matching pointrange_to_grade2. See:
         # https://github.com/devilry/devilry-django/issues/563
         matches = assignment2.pointtogrademap.pointrangetograde_set.filter_grades_matching_points(2)
         self.assertEqual({pointrange_to_grade2}, set(matches))
-        # self.assertEquals(set([pointrange_to_grade1, pointrange_to_grade2]), set(matches))
 
     def test_clean_no_entries(self):
         point_to_grade_map = PointToGradeMap.objects.create(assignment=self.assignment)
         self.assertTrue(point_to_grade_map.invalid)
         point_to_grade_map.invalid = True
         self.assertEqual(point_to_grade_map.pointrangetograde_set.count(), 0)
         point_to_grade_map.clean()
```

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_relateduser.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_relateduser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/tests/test_subject.py` & `devilry-6.0.0rc2/devilry/apps/core/tests/test_subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/apps/core/views/download_staticfeedbackfileattachment.py` & `devilry-6.0.0rc2/devilry/apps/core/views/download_staticfeedbackfileattachment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/coreutils/utils.py` & `devilry-6.0.0rc2/devilry/coreutils/utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/admin.py` & `devilry-6.0.0rc2/devilry/devilry_account/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/apps.py` & `devilry-6.0.0rc2/devilry/devilry_account/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/crinstance_account.py` & `devilry-6.0.0rc2/devilry/devilry_account/crinstance_account.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/middleware.py` & `devilry-6.0.0rc2/devilry/devilry_account/middleware.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/models.py` & `devilry-6.0.0rc2/devilry/devilry_account/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/user_merger.py` & `devilry-6.0.0rc2/devilry/devilry_account/user_merger.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/authbackend/default.py` & `devilry-6.0.0rc2/devilry/devilry_account/authbackend/default.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/authbackend/ldap.py` & `devilry-6.0.0rc2/devilry/devilry_account/authbackend/ldap.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/cradminextensions/devilry_crmenu_account.py` & `devilry-6.0.0rc2/devilry/devilry_account/cradminextensions/devilry_crmenu_account.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/crapps/account/index.py` & `devilry-6.0.0rc2/devilry/devilry_account/crapps/account/index.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/crapps/account/select_language.py` & `devilry-6.0.0rc2/devilry/devilry_account/crapps/account/select_language.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/devilry_account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/migrations/0002_auto_20150917_1731.py` & `devilry-6.0.0rc2/devilry/devilry_account/migrations/0002_auto_20150917_1731.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/migrations/0003_datamigrate-admins-into-permissiongroups.py` & `devilry-6.0.0rc2/devilry/devilry_account/migrations/0003_datamigrate-admins-into-permissiongroups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/migrations/0004_auto_20151222_1955.py` & `devilry-6.0.0rc2/devilry/devilry_account/migrations/0004_auto_20151222_1955.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/migrations/0005_auto_20160113_2037.py` & `devilry-6.0.0rc2/devilry/devilry_account/migrations/0005_auto_20160113_2037.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/migrations/0006_auto_20160120_0424.py` & `devilry-6.0.0rc2/devilry/devilry_account/migrations/0006_auto_20160120_0424.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/migrations/0007_auto_20210427_1350.py` & `devilry-6.0.0rc2/devilry/devilry_account/migrations/0007_auto_20210427_1350.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/migrations/0008_auto_20220510_1307.py` & `devilry-6.0.0rc2/devilry/devilry_account/migrations/0008_auto_20220510_1307.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/migrations/0009_mergeduser.py` & `devilry-6.0.0rc2/devilry/devilry_account/migrations/0009_mergeduser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html` & `devilry-6.0.0rc2/devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/templates/devilry_account/crapps/account/select_language.django.html` & `devilry-6.0.0rc2/devilry/devilry_account/templates/devilry_account/crapps/account/select_language.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/templatetags/devilry_account_tags.py` & `devilry-6.0.0rc2/devilry/devilry_account/templatetags/devilry_account_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/tests/test_devilry_account_tags.py` & `devilry-6.0.0rc2/devilry/devilry_account/tests/test_devilry_account_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/tests/test_middleware.py` & `devilry-6.0.0rc2/devilry/devilry_account/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/tests/test_models.py` & `devilry-6.0.0rc2/devilry/devilry_account/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/tests/test_user_merger.py` & `devilry-6.0.0rc2/devilry/devilry_account/tests/test_user_merger.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/tests/authbackend/test_default.py` & `devilry-6.0.0rc2/devilry/devilry_account/tests/authbackend/test_default.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/tests/test_crapps/test_account/test_index.py` & `devilry-6.0.0rc2/devilry/devilry_account/tests/test_crapps/test_account/test_index.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_account/tests/test_crapps/test_account/test_select_language.py` & `devilry-6.0.0rc2/devilry/devilry_account/tests/test_crapps/test_account/test_select_language.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/apps.py` & `devilry-6.0.0rc2/devilry/devilry_admin/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tasks.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tasks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/urls.py` & `devilry-6.0.0rc2/devilry/devilry_admin/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/devilry_crmenu_admin.py` & `devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/devilry_crmenu_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_assignmentgroup.py` & `devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_assignmentgroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedexaminer.py` & `devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedexaminer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedstudent.py` & `devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listbuilder/listbuilder_relatedstudent.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listfilter/listfilter_assignmentgroup.py` & `devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listfilter/listfilter_assignmentgroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py` & `devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/listfilter/listfilter_tags.py` & `devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/listfilter/listfilter_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/cradminextensions/multiselect2/multiselect2_relatedstudent.py` & `devilry-6.0.0rc2/devilry/devilry_admin/cradminextensions/multiselect2/multiselect2_relatedstudent.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/add_groups_to_examiner.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/add_groups_to_examiner.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/examinerdetails.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/examinerdetails.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/remove_groups_from_examiner.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/remove_groups_from_examiner.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-add.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-add.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-replace.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/manual-replace.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag-item-value.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/organize-by-tag.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/random.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/random.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/select_method.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/examiners/bulk_organize/select_method.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/custom-table.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/custom-table.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/gradingconfiguration-update.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/gradingconfiguration-update/gradingconfiguration-update.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/examiners.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/examiners.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/gradingconfiguration.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/gradingconfiguration.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/published.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/published.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/settings.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/settings.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/statistics.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/statistics.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/students.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/students.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/include/utilities.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/include/utilities.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/includes/batchdownload_assignment.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/includes/batchdownload_assignment.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-item-value.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/assignment-overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/candidate-item-value.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/candidate-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/confirm-view.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/confirm-view.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select-period-view.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select-period-view.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select_groups_to_pass.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/passed_previous_period/select_groups_to_pass.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/statistics/overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/statistics/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/merge_groups.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/merge_groups.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/split_groups.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/split_groups.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-accumulated-score.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-accumulated-score.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-assignment-item-value.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-assignment-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-method.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-method.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-period-item-value.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/choose-period-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/confirm.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/confirm.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/manual-select-students.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/manual-select-students.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/preview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/preview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/select-assignments.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/create_groups/grading_points_based/select-assignments.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-method.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-method.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-period-item-value.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/choose-period-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/confirm.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/delete_groups/confirm.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupdetails/view.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/assignment/students/groupdetails/view.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/common/abstract-type-in-users.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/common/abstract-type-in-users.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/common/admin-list-view.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/common/admin-list-view.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/common/admins-explained.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/common/admins-explained.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/group_by_assignment.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/group_by_assignment.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_groups.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_groups.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_users.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/dashboard/student_feedbackfeed_wizard/student_feedbackfeed_list_users.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/listbuilder/assignmentgroup_listbuilder/value.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/listbuilder/assignmentgroup_listbuilder/value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/listbuilder/listbuilder_relatedexaminer/onassignment-itemvalue.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/listbuilder/listbuilder_relatedexaminer/onassignment-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/admins/add.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/admins/add.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/admins/overview-itemvalue.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/admins/overview-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/admins/overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/admins/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/devilry_all_results_overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/devilry_all_results_overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/result_cell_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/all_results_overview/result_cell_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/createassignment.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/createassignment.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/helpbox.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/helpbox.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/success_message.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/success_message.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/createassignment/suggested_deadlines.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/createassignment/suggested_deadlines.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/edit/updateview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/edit/updateview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/examiners/add.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/examiners/add.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview-itemvalue.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/examiners/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/add-tag.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/add-tag.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/base-multiselect-view.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/base-multiselect-view.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/crud.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/crud.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/delete.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/delete.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/manage-tags-list-view.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/manage-tags-list-view.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/tag-item-value.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/tag-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/relatedusers/select-method.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/manage_tags/relatedusers/select-method.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/add.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/add.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/overview-itemvalue.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/overview-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/period/students/overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/period/students/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/overview_for_period_admins.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/overview_for_period_admins.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/admins/add.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/admins/add.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview-itemvalue.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/admins/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/templates/devilry_admin/subject/edit/updateview.django.html` & `devilry-6.0.0rc2/devilry/devilry_admin/templates/devilry_admin/subject/edit/updateview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_anonymizationmode.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_anonymizationmode.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_batchframework_tasks.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_batchframework_tasks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_crinstance_assignment.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_crinstance_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_deadline_handling.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_deadline_handling.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_examiner_selfassign.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_examiner_selfassign.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_examiner_statistics.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_examiner_statistics.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_first_deadline.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_first_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_grading_configuration.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_grading_configuration.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_long_and_shortname.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_long_and_shortname.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_projectgroups.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_projectgroups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_publishing_time.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_publishing_time.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_add_groups_to_examiner.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_add_groups_to_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_bulk_organize.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_bulk_organize.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_examinerdetails.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_examinerdetails.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/examiners/test_remove_groups_from_examiner.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/examiners/test_remove_groups_from_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period_manual.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/passed_previous_semester/test_passed_previous_period_manual.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_create_groups.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_create_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_create_groups_accumulated_score.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_create_groups_accumulated_score.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_delete_groups.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_delete_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupdetails.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupdetails.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_merge_groups.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_merge_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_replace_groups.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_replace_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_split_group.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_split_group.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_baseinforview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_baseinforview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_basemultiselectview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_basemultiselectview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_groupviewmixin.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/students/test_groupview_base/test_groupviewmixin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/assignment/test_download_files/test_batchdownload_api.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/assignment/test_download_files/test_batchdownload_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/common/admins_common_testmixins.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/common/admins_common_testmixins.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/common/test_bulkimport_users_common.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/common/test_bulkimport_users_common.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/cradminextensions/test_devilry_crmenu_admin.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/cradminextensions/test_devilry_crmenu_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedexaminer.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedexaminer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedstudent.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/cradminextensions/test_listbuilder/test_listbuilder_relatedstudent.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/cradminextensions/test_multiselect2/test_multiselect2_relatedstudent.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/cradminextensions/test_multiselect2/test_multiselect2_relatedstudent.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/dashboard/test_createsubject.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/dashboard/test_createsubject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/dashboard/test_overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/dashboard/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_assignment_listview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_assignment_listview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_student_listview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/dashboard/test_student_feedbackfeed_wizard/test_student_listview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_admins.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_admins.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_createassignment.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_createassignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_crinstance_period.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_crinstance_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_edit.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_edit.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_examiners.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_examiners.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_overview_all_results.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_overview_all_results.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_period_all_results_collector.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_period_all_results_collector.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_students.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_students.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,54 +37,14 @@
             mockresponse.request.cradmin_instance.reverse_url.call_args_list[0]
         )
         self.assertEqual(
             mock.call(appname='manage_tags', args=(), viewname='add_tag', kwargs={}),
             mockresponse.request.cradmin_instance.reverse_url.call_args_list[1]
         )
 
-    # def test_link_urls_with_period_tags_rendered(self):
-    #     testperiod = baker.make('core.Period')
-    #     testperiodtag = baker.make('core.PeriodTag', period=testperiod, tag='a')
-    #     testperiodtag.relatedexaminers.add(baker.make('core.RelatedExaminer', period=testperiod))
-    #     testperiodtag.relatedstudents.add(baker.make('core.RelatedStudent', period=testperiod))
-    #     mockresponse = self.mock_http200_getrequest_htmls(cradmin_role=testperiod)
-    #     self.assertEquals(6, len(mockresponse.request.cradmin_instance.reverse_url.call_args_list))
-    #     self.assertEquals(
-    #         mock.call(appname='overview', args=(), viewname='INDEX', kwargs={}),
-    #         mockresponse.request.cradmin_instance.reverse_url.call_args_list[0]
-    #     )
-    #     self.assertEquals(
-    #         mock.call(appname='manage_tags', args=(), viewname='add_tag', kwargs={}),
-    #         mockresponse.request.cradmin_instance.reverse_url.call_args_list[1]
-    #     )
-    #     self.assertEquals(
-    #         mock.call('edit', args=(testperiodtag.id,), kwargs={}),
-    #         mockresponse.request.cradmin_app.reverse_appurl.call_args_list[3]
-    #     )
-    #     self.assertEquals(
-    #         mock.call('delete', args=(testperiodtag.id,), kwargs={}),
-    #         mockresponse.request.cradmin_app.reverse_appurl.call_args_list[4]
-    #     )
-    #     self.assertEquals(
-    #         mock.call(appname='manage_tags', args=(), viewname='add_students', kwargs={'tag': 'a'}),
-    #         mockresponse.request.cradmin_instance.reverse_url.call_args_list[5]
-    #     )
-    #     self.assertEquals(
-    #         mock.call(appname='manage_tags', args=(), viewname='add_examiners', kwargs={'tag': 'a'}),
-    #         mockresponse.request.cradmin_instance.reverse_url.call_args_list[6]
-    #     )
-    #     self.assertEquals(
-    #         mock.call(appname='manage_tags', args=(), viewname='remove_students', kwargs={'tag': 'a'}),
-    #         mockresponse.request.cradmin_instance.reverse_url.call_args_list[7]
-    #     )
-    #     self.assertEquals(
-    #         mock.call(appname='manage_tags', args=(), viewname='remove_examiners', kwargs={'tag': 'a'}),
-    #         mockresponse.request.cradmin_instance.reverse_url.call_args_list[8]
-    #     )
-
     def test_num_item_values_rendered(self):
         testperiod = baker.make('core.Period')
         baker.make('core.PeriodTag', period=testperiod)
         baker.make('core.PeriodTag', period=testperiod)
         baker.make('core.PeriodTag', period=testperiod)
         mockresponse = self.mock_http200_getrequest_htmls(
             cradmin_role=testperiod
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags_relatedusers.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_manage_tags/test_manage_tags_relatedusers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/period/test_report/test_all_results_generator.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/period/test_report/test_all_results_generator.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/subject/test_admins.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/subject/test_admins.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/subject/test_createperiod.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/subject/test_createperiod.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/subject/test_crinstance_subject.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/subject/test_crinstance_subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/subject/test_edit.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/subject/test_edit.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/subject/test_overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/subject/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/test_crinstance_for_periodadmin.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/test_crinstance_for_periodadmin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/test_overview_for_periodadmin.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/test_overview_for_periodadmin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/tests/subject_for_period_admin/test_subject_redirect.py` & `devilry-6.0.0rc2/devilry/devilry_admin/tests/subject_for_period_admin/test_subject_redirect.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/anonymizationmode.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/anonymizationmode.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/crinstance_assignment.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/crinstance_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/deadline_handling.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/deadline_handling.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiner_selfassign.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiner_selfassign.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/first_deadline.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/first_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/gradingconfiguration.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/gradingconfiguration.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/projectgroups.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/projectgroups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/publishing_time.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/publishing_time.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/download_files/batch_download_api.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/download_files/batch_download_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/download_files/download_archive.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/download_files/download_archive.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiners/add_groups_to_examiner.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiners/add_groups_to_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiners/base_single_examinerview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiners/base_single_examinerview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiners/bulk_organize.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiners/bulk_organize.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiners/examinerdetails.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiners/examinerdetails.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiners/overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiners/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/examiners/remove_groups_from_examiner.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/examiners/remove_groups_from_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/__init__.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/__init__.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_period.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_semester_manual.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/passed_previous_period/passed_previous_semester_manual.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/statistics/statistics_overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/statistics/statistics_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/create_groups.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/create_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/create_groups_accumulated_score.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/create_groups_accumulated_score.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/delete_groups.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/delete_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/groupdetails.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/groupdetails.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/groupview_base.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/groupview_base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/manage_deadlines.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/manage_deadlines.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/merge_groups.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/merge_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/replace_groups.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/replace_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/assignment/students/split_group.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/assignment/students/split_group.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/common/bulkimport_users_common.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/common/bulkimport_users_common.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/createsubject.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/createsubject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/crinstance_dashboard.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/crinstance_dashboard.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/__init__.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/assignment_list.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/assignment_list.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/filters.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/filters.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/student_list.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/dashboard/student_feedbackfeed_wizard/student_list.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/period/admins.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/period/admins.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/period/all_results_generator.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/period/all_results_generator.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/period/createassignment.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/period/createassignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/period/crinstance_period.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/period/crinstance_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/period/edit.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/period/edit.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/period/examiners.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/period/examiners.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/period/overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/period/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/period/overview_all_results.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/period/overview_all_results.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/period/overview_all_results_collector.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/period/overview_all_results_collector.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/period/students.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/period/students.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/period/manage_tags/manage_tags.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/period/manage_tags/manage_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/subject/admins.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/subject/admins.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/subject/createperiod.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/subject/createperiod.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/subject/crinstance_subject.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/subject/crinstance_subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/subject/edit.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/subject/edit.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/subject/overview.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/subject/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/subject_for_period_admin/crinstance_subject_for_periodadmin.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/subject_for_period_admin/crinstance_subject_for_periodadmin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/subject_for_period_admin/overview_for_periodadmin.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/subject_for_period_admin/overview_for_periodadmin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_admin/views/subject_for_period_admin/subject_redirect.py` & `devilry-6.0.0rc2/devilry/devilry_admin/views/subject_for_period_admin/subject_redirect.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_authenticate/allauth_adapter.py` & `devilry-6.0.0rc2/devilry/devilry_authenticate/allauth_adapter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_authenticate/apps.py` & `devilry-6.0.0rc2/devilry/devilry_authenticate/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_authenticate/socialaccount_user_updaters.py` & `devilry-6.0.0rc2/devilry/devilry_authenticate/socialaccount_user_updaters.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_authenticate/urls.py` & `devilry-6.0.0rc2/devilry/devilry_authenticate/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/login.django.html` & `devilry-6.0.0rc2/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/login.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/logout.django.html` & `devilry-6.0.0rc2/devilry/devilry_authenticate/templates/devilry_authenticate/allauth/logout.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_authenticate/views/allauth_views.py` & `devilry-6.0.0rc2/devilry/devilry_authenticate/views/allauth_views.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_authenticate/views/custom_login_view.py` & `devilry-6.0.0rc2/devilry/devilry_authenticate/views/custom_login_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_bulkcreate_users/create_users.py` & `devilry-6.0.0rc2/devilry/devilry_bulkcreate_users/create_users.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_bulkcreate_users/urls.py` & `devilry-6.0.0rc2/devilry/devilry_bulkcreate_users/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/confirm_bulkcreated_users.django.html` & `devilry-6.0.0rc2/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/confirm_bulkcreated_users.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/show_bulkcreated_users.django.html` & `devilry-6.0.0rc2/devilry/devilry_bulkcreate_users/templates/devilry_bulkcreate_users/show_bulkcreated_users.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_bulkcreate_users/views/submit_bulk_users.py` & `devilry-6.0.0rc2/devilry/devilry_bulkcreate_users/views/submit_bulk_users.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_changelog/models.py` & `devilry-6.0.0rc2/devilry/devilry_changelog/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_comment/editor_widget.py` & `devilry-6.0.0rc2/devilry/devilry_comment/editor_widget.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_comment/models.py` & `devilry-6.0.0rc2/devilry/devilry_comment/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_comment/api/preview_markdown.py` & `devilry-6.0.0rc2/devilry/devilry_comment/api/preview_markdown.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_comment/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/devilry_comment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_comment/migrations/0002_auto_20160109_1210.py` & `devilry-6.0.0rc2/devilry/devilry_comment/migrations/0002_auto_20160109_1210.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_comment/migrations/0003_auto_20160109_1239.py` & `devilry-6.0.0rc2/devilry/devilry_comment/migrations/0003_auto_20160109_1239.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_comment/migrations/0006_auto_20170621_1720.py` & `devilry-6.0.0rc2/devilry/devilry_comment/migrations/0006_auto_20170621_1720.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_comment/migrations/0010_commentedithistory.py` & `devilry-6.0.0rc2/devilry/devilry_comment/migrations/0010_commentedithistory.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_comment/migrations/0011_auto_20220421_1242.py` & `devilry-6.0.0rc2/devilry/devilry_comment/migrations/0011_auto_20220421_1242.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html` & `devilry-6.0.0rc2/devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_comment/tests/test_models.py` & `devilry-6.0.0rc2/devilry/devilry_comment/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/abstract_batch_action.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/abstract_batch_action.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/admin.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/backend_registry.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/backend_registry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/models.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/backends/backend_mock.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/backends/backend_mock.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/backends/backends_base.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/backends/backends_base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/batchjob_mixins/assignment_mixin.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/batchjob_mixins/assignment_mixin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/batchjob_mixins/feedbackset_mixin.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/batchjob_mixins/feedbackset_mixin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/migrations/0002_auto_20170119_1202.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/migrations/0002_auto_20170119_1202.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/migrations/0003_auto_20170119_1648.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/migrations/0003_auto_20170119_1648.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/migrations/0005_compressedarchivemeta_created_by.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/migrations/0005_compressedarchivemeta_created_by.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/migrations/0006_compressedarchivemeta_created_by_role.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/migrations/0006_compressedarchivemeta_created_by_role.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/tests/test_backend.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/tests/test_model.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_compressionutil/tests/test_registry.py` & `devilry-6.0.0rc2/devilry/devilry_compressionutil/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_acemarkdown.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_acemarkdown.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_crinstance.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_crinstance.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_crmenu.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_crmenu.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/assignment.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/assignmentgroup.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/assignmentgroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_sidebar.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_sidebar.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_timeline.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/feedbackfeed_timeline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/period.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/permissiongroup.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/permissiongroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/permissiongroupuser.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/permissiongroupuser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listbuilder/subject.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listbuilder/subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listfilter/assignment.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listfilter/assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listfilter/assignmentgroup.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listfilter/assignmentgroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listfilter/user.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listfilter/user.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_listfilter/utils.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_listfilter/utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_multiselect2/user.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_multiselect2/user.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_tablebuilder/base.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_tablebuilder/base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/devilry_tablebuilder/base_new.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/devilry_tablebuilder/base_new.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/cradmin_legacy/standalone-base.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/cradmin_legacy/standalone-base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_acemarkdown.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_acemarkdown.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/account-menuitem.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_crmenu/account-menuitem.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/examiner-item-value.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/examiner-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-examiner-item-value.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/multiselect-examiner-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/groupdetails.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/groupdetails.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/admin-itemvalue.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/admin-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/student-itemvalue.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/period/student-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/permissiongroup/subjectorperiodpermissiongroup-itemvalue.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/permissiongroup/subjectorperiodpermissiongroup-itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listfilter/utils/devilry_with_result_value_renderable.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listfilter/utils/devilry_with_result_value_renderable.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/row.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/row.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/table.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/devilry_tablebuilder/table.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_tablebuilder.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/new_devilry_tablebuilder/base_tablebuilder.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_confirmview.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_confirmview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_createview_with_backlink.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_createview_with_backlink.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_updateview_with_backlink.django.html` & `devilry-6.0.0rc2/devilry/devilry_cradmin/templates/devilry_cradmin/viewhelpers/devilry_updateview_with_backlink.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignment.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignmentgroup.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_assignmentgroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_sidebar.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_sidebar.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_timeline.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_feedbackfeed_timeline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_period.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroup.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroupuser.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_permissiongroupuser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_user.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listbuilder/test_user.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_listfilter/test_assignmentgroup_listfilter.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_listfilter/test_assignmentgroup_listfilter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_devilry_multiselect2/test_user.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_devilry_multiselect2/test_user.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/tests/test_tablebuilder/test_table.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/tests/test_tablebuilder/test_table.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_cradmin/viewhelpers/devilry_confirmview.py` & `devilry-6.0.0rc2/devilry/devilry_cradmin/viewhelpers/devilry_confirmview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dataporten_allauth/callback.py` & `devilry-6.0.0rc2/devilry/devilry_dataporten_allauth/callback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dataporten_allauth/views.py` & `devilry-6.0.0rc2/devilry/devilry_dataporten_allauth/views.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/admin.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/bulk_create_queryset_mixin.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/bulk_create_queryset_mixin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/models.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/assignment/triggers.sql` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/assignment/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/assignment_group/triggers.sql` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/assignment_group/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/assignment_group_cached_data/rebuild.sql` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/assignment_group_cached_data/rebuild.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/candidate/triggers.sql` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/candidate/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/comment/triggers.sql` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/comment/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/commentfile/helperfunctions.sql` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/commentfile/helperfunctions.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/commentfile/triggers.sql` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/commentfile/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/examiner/triggers.sql` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/examiner/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/helperfunctions.sql` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/helperfunctions.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/triggers.sql` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/validate.sql` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/feedbackset/validate.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/groupcomment/triggers.sql` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/groupcomment/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/customsql_sqlcode/imageannotationcomment/triggers.sql` & `devilry-6.0.0rc2/devilry/devilry_dbcache/customsql_sqlcode/imageannotationcomment/triggers.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/migrations/0002_auto_20170108_0948.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/migrations/0002_auto_20170108_0948.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/migrations/0003_auto_20170108_1341.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/migrations/0003_auto_20170108_1341.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/migrations/0004_auto_20170108_1453.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/migrations/0004_auto_20170108_1453.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/migrations/0005_auto_20170124_1504.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/migrations/0005_auto_20170124_1504.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_assignment_group_cached_data_triggers.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_assignment_group_cached_data_triggers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_benchmarks.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_bulk_create_queryset_mixin.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_bulk_create_queryset_mixin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_candidate_triggers.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_candidate_triggers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_comment_triggers.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_comment_triggers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_examiner_triggers.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_examiner_triggers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_feedbackset_triggers.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_feedbackset_triggers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_dbcache/tests/test_groupcomment_triggers.py` & `devilry-6.0.0rc2/devilry/devilry_dbcache/tests/test_groupcomment_triggers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/cradmin_app.py` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/cradmin_app.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/deadline-bulk-multiselect-filterlistview.django.html` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/deadline-bulk-multiselect-filterlistview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/manage-deadline.django.html` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/manage-deadline.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline-item-value.django.html` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline.django.html` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/select-deadline.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/suggested-deadlines.django.html` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/suggested-deadlines.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-base.django.html` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/templates/devilry_deadlinemanagement/includes/info-box-base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/tests/test_deadline_listview.py` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/tests/test_deadline_listview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_admin.py` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_examiner.py` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/tests/test_manage_deadline_view_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/tests/test_multiselect_groups.py` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/tests/test_multiselect_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/views/deadline_listview.py` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/views/deadline_listview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/views/manage_deadline_view.py` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/views/manage_deadline_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/views/multiselect_groups_view.py` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/views/multiselect_groups_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_deadlinemanagement/views/viewutils.py` & `devilry-6.0.0rc2/devilry/devilry_deadlinemanagement/views/viewutils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_detektor/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/devilry_detektor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_detektor/migrations/0002_auto_20180119_1137.py` & `devilry-6.0.0rc2/devilry/devilry_detektor/migrations/0002_auto_20180119_1137.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_developemail/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/devilry_developemail/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/utils.py` & `devilry-6.0.0rc2/devilry/devilry_email/utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/comment_email/comment_email.py` & `devilry-6.0.0rc2/devilry/devilry_email/comment_email/comment_email.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,34 +70,14 @@
     from devilry.devilry_group.models import GroupComment
     try:
         return GroupComment.objects.get(id=comment_id)
     except:
         logger.error('Mail: Something went wrong. GroupComment with ID#{} does not exist'.format(comment_id))
 
 
-def get_student_users_not_comment_poster(group, exclude_user=None):
-    """
-    Get all student users in assignment group, and exclude the user that created the comment.
-    """
-    queryset = get_student_users_in_group(group=group)
-    if not exclude_user:
-        return queryset
-    return queryset.exclude(id=exclude_user.id)
-
-
-def get_examiner_users_not_comment_poster(group, exclude_user=None):
-    """
-    Get all examiner users in assignment group, and exclude the user that created the comment.
-    """
-    queryset = get_examiner_users_in_group(group=group)
-    if not exclude_user:
-        return queryset
-    return queryset.exclude(id=exclude_user.id)
-
-
 def get_subject_and_period_admins_users(group):
     """
     Get all User objects where the user is :class:`~.devilry.devilry_core.models.Subject`
     or :class:`~.devilry.devilry_core.models.Period` admins for the assignment group.
     """
     period_permissiongroups = PeriodPermissionGroup.objects \
         .filter(period=group.parentnode.period) \
@@ -185,15 +165,15 @@
 
 def send_examiner_comment_email(comment_id, domain_url_start):
     """
     Send email to examiner users.
 
     The email content will be the same for all examiners.
 
-    If no examiner users exists for the assignment, :class:`~.devilry.devilry_core.models.Subject`
+    If no examiner-users exists for the assignment group, :class:`~.devilry.devilry_core.models.Subject`
     and :class:`~.devilry.devilry_core.models.Period` admins connected to the assignemnt are sat
     as recipients of the email and extra info is added in the template.
 
     How do the mails differ?
 
     Student comments::
         Email subjects:
@@ -210,25 +190,35 @@
     Comments from admins::
         Email subject:
             ``An admin added a new comment for <assignment name>``
     """
     comment = get_comment(comment_id=comment_id)
     absolute_url = build_feedbackfeed_absolute_url(
         domain_scheme=domain_url_start, group_id=comment.feedback_set.group.id, instance_id='devilry_group_examiner')
-    recipients = list(
-        get_examiner_users_not_comment_poster(group=comment.feedback_set.group, exclude_user=comment.user))
-    has_examiner = True
+
+    examiner_users_in_group_queryset = get_examiner_users_in_group(group=comment.feedback_set.group)
+    has_examiner = examiner_users_in_group_queryset.exists()
+    recipients = list(examiner_users_in_group_queryset.exclude(id=comment.user.id))
+
     if not recipients:
-        if comment.text.strip() == '':
-            # Do not spam admins with notifications for comments without any text.
+        if not has_examiner:
+            # No examiners assigned to the group. Set recipients to the subject- 
+            # and period-admin users so they receive an e-mail informing that the 
+            # group has no examiners assigned.
+            if comment.text.strip() == '':
+                # Do not spam admins with notifications for comments without any text.
+                return
+            absolute_url = build_feedbackfeed_absolute_url(
+                domain_scheme=domain_url_start, group_id=comment.feedback_set.group.id, instance_id='devilry_group_admin')
+            recipients = list(get_subject_and_period_admins_users(group=comment.feedback_set.group))
+        else:
+            # Group has an examiner, but no recipients.
+            # This happens when the group has one examiner and the user is also the comment-poster.
             return
-        absolute_url = build_feedbackfeed_absolute_url(
-            domain_scheme=domain_url_start, group_id=comment.feedback_set.group.id, instance_id='devilry_group_admin')
-        recipients = list(get_subject_and_period_admins_users(group=comment.feedback_set.group))
-        has_examiner = False
+
     send_comment_email(
         comment=comment,
         user_list=recipients,
         feedbackfeed_url=absolute_url,
         crinstance_id='devilry_group_examiner',
         domain_scheme=domain_url_start,
         has_examiner=has_examiner
@@ -271,19 +261,19 @@
     Comments from admins::
         Email subject:
             ``An admin added a new comment for <assignment name>``
     """
     comment = get_comment(comment_id=comment_id)
     absolute_url = build_feedbackfeed_absolute_url(
         domain_scheme=domain_url_start, group_id=comment.feedback_set.group.id)
-    student_users = list(get_student_users_not_comment_poster(group=comment.feedback_set.group, exclude_user=comment.user))
+    recipients = list(get_student_users_in_group(group=comment.feedback_set.group).exclude(id=comment.user.id))
 
     send_comment_email(
         comment=comment,
-        user_list=student_users,
+        user_list=recipients,
         feedbackfeed_url=absolute_url,
         domain_scheme=domain_url_start,
         crinstance_id='devilry_group_student'
     )
 
     if from_student_poster:
         send_comment_email(
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/deadline_email/deadline_email.py` & `devilry-6.0.0rc2/devilry/devilry_email/deadline_email/deadline_email.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/feedback_email/feedback_email.py` & `devilry-6.0.0rc2/devilry/devilry_email/feedback_email/feedback_email.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/management/commands/devilry_send_testemail.py` & `devilry-6.0.0rc2/devilry/devilry_email/management/commands/devilry_send_testemail.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/templates/devilry_email/comment_email/comment.txt` & `devilry-6.0.0rc2/devilry/devilry_email/templates/devilry_email/comment_email/comment.txt`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/templates/devilry_email/deadline_email/deadline_moved.txt` & `devilry-6.0.0rc2/devilry/devilry_email/templates/devilry_email/deadline_email/deadline_moved.txt`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/templates/devilry_email/deadline_email/new_attempt.txt` & `devilry-6.0.0rc2/devilry/devilry_email/templates/devilry_email/deadline_email/new_attempt.txt`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/templates/devilry_email/feedback_email/assignment_feedback_student.txt` & `devilry-6.0.0rc2/devilry/devilry_email/templates/devilry_email/feedback_email/assignment_feedback_student.txt`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/templatetags/comment_email_tags.py` & `devilry-6.0.0rc2/devilry/devilry_email/templatetags/comment_email_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/tests/test_bulk_feedback.py` & `devilry-6.0.0rc2/devilry/devilry_email/tests/test_bulk_feedback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/tests/test_comment_email.py` & `devilry-6.0.0rc2/devilry/devilry_email/tests/test_comment_email.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,15 +357,15 @@
         baker.make(
             'devilry_account.PeriodPermissionGroup',
             period=assignment.period,
             permissiongroup=permission_group
         )
         if not admin_user:
             admin_user = baker.make(settings.AUTH_USER_MODEL)
-        baker.make('devilry_account.UserEmail', user=admin_user, email='period_admin@example.com')
+            baker.make('devilry_account.UserEmail', user=admin_user, email='period_admin@example.com')
         baker.make(
             'devilry_account.PermissionGroupUser',
             permissiongroup=permission_group,
             user=admin_user
         )
 
     def _setup_subject_admin(self, assignment):
@@ -503,14 +503,15 @@
         testassignment = baker.make_recipe('devilry.apps.core.assignment_activeperiod_start',
                                            long_name='Assignment 1')
         testgroup = baker.make('core.AssignmentGroup', parentnode=testassignment)
         test_feedbackset = group_baker.feedbackset_first_attempt_unpublished(
             group=testgroup, deadline_datetime=timezone.now() + timezone.timedelta(days=1))
 
         admin_user = baker.make(settings.AUTH_USER_MODEL)
+        baker.make('devilry_account.UserEmail', user=admin_user, email='adminuser@example.com')
         self._setup_period_admin(assignment=testassignment, admin_user=admin_user)
 
         # The user that posted the comment
         comment_user = baker.make(settings.AUTH_USER_MODEL, shortname='testuser@example.com')
         baker.make('core.Candidate', assignment_group=test_feedbackset.group, relatedstudent__user=comment_user)
         test_groupcomment = baker.make('devilry_group.GroupComment',
                                        feedback_set=test_feedbackset,
@@ -525,15 +526,19 @@
         self.assertEqual(len(mail.outbox), 1)
         self.assertEqual(Message.objects.count(), 1)
         self.assertEqual(MessageReceiver.objects.count(), 1)
         self.assertTrue(MessageReceiver.objects.filter(user=admin_user).exists())
         self.assertEqual(Message.objects.filter(status='sent').count(), 1)
         self.assertEqual(MessageReceiver.objects.filter(status='sent').count(), 1)
 
-    def test_send_examiner_comment_no_examiner_subject_from_student_another_examiner(self):
+    def test_send_examiner_comment_single_examiner_as_examiner_comment_poster(self):
+        # Test that no e-mail is sent if the comment-poster is the only examiner in the group.
+        # This is because we exclude the comment-poster (examiners does not receive a receipt), 
+        # but since the comment-poster is also an examiner that means that the group has an 
+        # examiner and no e-mail should be sent to admins.
         testassignment = baker.make_recipe('devilry.apps.core.assignment_activeperiod_start',
                                            long_name='Assignment 1')
         testgroup = baker.make('core.AssignmentGroup', parentnode=testassignment)
         test_feedbackset = group_baker.feedbackset_first_attempt_unpublished(
             group=testgroup, deadline_datetime=timezone.now() + timezone.timedelta(days=1))
 
         self._setup_period_and_subject_admins(assignment=testassignment)
@@ -547,21 +552,44 @@
                                        user_role=Comment.USER_ROLE_EXAMINER,
                                        user=comment_user)
         baker.make('devilry_account.UserEmail', user=comment_user, email='testuser@example.com')
         send_examiner_comment_email(
             comment_id=test_groupcomment.id,
             domain_url_start='http://www.example.com/', )
 
-        self.assertEqual(len(mail.outbox), 2)
-        self.assertIn(mail.outbox[0].recipients()[0], ['period_admin@example.com', 'subject_admin@example.com'])
-        self.assertIn(mail.outbox[1].recipients()[0], ['period_admin@example.com', 'subject_admin@example.com'])
-        self.assertEqual(
-            mail.outbox[0].subject,
-            '[Devilry] An examiner added a new comment for {}'.format(
-                test_feedbackset.group.parentnode.long_name))
+        self.assertEqual(len(mail.outbox), 0)
+        self.assertEqual(Message.objects.count(), 0)
+
+    def test_send_examiner_comment_single_examiner_as_period_admin_comment_poster(self):
+        # Tests that e-mail is not sent to the examiner-user when they also a period-admin 
+        # and posts a comment as admin.
+        testassignment = baker.make_recipe('devilry.apps.core.assignment_activeperiod_start',
+                                           long_name='Assignment 1')
+        testgroup = baker.make('core.AssignmentGroup', parentnode=testassignment)
+        test_feedbackset = group_baker.feedbackset_first_attempt_unpublished(
+            group=testgroup, deadline_datetime=timezone.now() + timezone.timedelta(days=1))
+
+        self._setup_period_and_subject_admins(assignment=testassignment)
+
+        # The user that posted the comment
+        comment_user = baker.make(settings.AUTH_USER_MODEL, shortname='examiner@example.com')
+        baker.make('core.Examiner', assignmentgroup=test_feedbackset.group, relatedexaminer__user=comment_user)
+        self._setup_period_admin(assignment=testassignment, admin_user=comment_user)
+        test_groupcomment = baker.make('devilry_group.GroupComment',
+                                       feedback_set=test_feedbackset,
+                                       text='This is a test',
+                                       user_role=Comment.USER_ROLE_ADMIN,
+                                       user=comment_user)
+        baker.make('devilry_account.UserEmail', user=comment_user, email='examiner@example.com')
+        send_examiner_comment_email(
+            comment_id=test_groupcomment.id,
+            domain_url_start='http://www.example.com/', )
+
+        self.assertEqual(len(mail.outbox), 0)
+        self.assertEqual(Message.objects.count(), 0)
 
     def test_send_examiner_no_examiner_admin_comment(self):
         testassignment = baker.make_recipe('devilry.apps.core.assignment_activeperiod_start',
                                            long_name='Assignment 1')
         testgroup = baker.make('core.AssignmentGroup', parentnode=testassignment)
         test_feedbackset = group_baker.feedbackset_first_attempt_unpublished(
             group=testgroup, deadline_datetime=timezone.now() + timezone.timedelta(days=1))
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/tests/test_deadline_email.py` & `devilry-6.0.0rc2/devilry/devilry_email/tests/test_deadline_email.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_email/tests/test_feedback_email.py` & `devilry-6.0.0rc2/devilry/devilry_email/tests/test_feedback_email.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/apps.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tasks.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tasks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/urls.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/cradminextensions/devilry_crmenu_examiner.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/cradminextensions/devilry_crmenu_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_create_feedback.django.html` & `devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_create_feedback.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_new_attempt.django.html` & `devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/bulk_new_attempt.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/grouplist.django.html` & `devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/grouplist.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/includes/batchdownload_assignment.django.html` & `devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/includes/batchdownload_assignment.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/grade_cell_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/grade_cell_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/simple_group_bulk_feedbackview.django.html` & `devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/simple_group_bulk_feedbackview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/dashboard/assignmentlist.django.html` & `devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/dashboard/assignmentlist.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign-group-item-value.django.html` & `devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign-group-item-value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign.django.html` & `devilry-6.0.0rc2/devilry/devilry_examiner/templates/devilry_examiner/selfassign/selfassign.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/templatetags/devilry_examiner_tags.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/templatetags/devilry_examiner_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_assignment/test_batchdownload_api.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_assignment/test_batchdownload_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_assignment/test_batchframework_tasks.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_assignment/test_batchframework_tasks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback_simple.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_assignment/test_bulkcreate_feedback_simple.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_assignment/test_crinstance_assignment.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_assignment/test_crinstance_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_assignment/test_grouplist.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_assignment/test_grouplist.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_cradminextensions/test_devilry_crmenu_examiner.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_cradminextensions/test_devilry_crmenu_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_dashboard/test_assignmentlist.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_dashboard/test_assignmentlist.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_dashboard/test_crinstance_dashboard.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_dashboard/test_crinstance_dashboard.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_api.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_crinstance_selfassign.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_crinstance_selfassign.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_grouplist.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_grouplist.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_utils.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/tests/test_selfassign/test_selfassign_utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/crinstance_assignment.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/crinstance_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/grouplist.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/grouplist.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_manage_deadline.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_manage_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_operations_grouplist.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/bulkoperations/bulk_operations_grouplist.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/download_files/batch_download_api.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/download_files/batch_download_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/assignment/download_files/download_archive.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/assignment/download_files/download_archive.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/dashboard/assignmentlist.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/dashboard/assignmentlist.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/dashboard/crinstance_dashboard.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/dashboard/crinstance_dashboard.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/selfassign/api.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/selfassign/api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/selfassign/crinstance_selfassign.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/selfassign/crinstance_selfassign.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/selfassign/selfassign.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/selfassign/selfassign.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_examiner/views/selfassign/utils.py` & `devilry-6.0.0rc2/devilry/devilry_examiner/views/selfassign/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         .select_related('parentnode') \
         .filter(parentnode_id__in=assignment_queryset.values_list('id', flat=True)) \
         .annotate(number_of_examiners=models.Count('examiners')) \
         .filter(
             models.Q(examiners__relatedexaminer__user=user)
             |
             models.Q(number_of_examiners__lt=models.F('parentnode__examiner_self_assign_limit'))
-        )
+        ).distinct()
     return assignmentgroup_queryset
 
 
 def selfassign_available_periods(user):
     return Period.objects \
         .filter_active() \
         .filter(
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_frontpage/crinstance_frontpage.py` & `devilry-6.0.0rc2/devilry/devilry_frontpage/crinstance_frontpage.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_frontpage/cradminextensions/listbuilder/listbuilder_role.py` & `devilry-6.0.0rc2/devilry/devilry_frontpage/cradminextensions/listbuilder/listbuilder_role.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_frontpage/templates/devilry_frontpage/frontpage.django.html` & `devilry-6.0.0rc2/devilry/devilry_frontpage/templates/devilry_frontpage/frontpage.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_frontpage/tests/test_frontpage.py` & `devilry-6.0.0rc2/devilry/devilry_frontpage/tests/test_frontpage.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_frontpage/tests/test_cradminextensions/test_listbuilder_role.py` & `devilry-6.0.0rc2/devilry/devilry_frontpage/tests/test_cradminextensions/test_listbuilder_role.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_frontpage/views/frontpage.py` & `devilry-6.0.0rc2/devilry/devilry_frontpage/views/frontpage.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradeform/templates/devilry_gradeform/setup.gradeform.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradeform/templates/devilry_gradeform/setup.gradeform.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradeform/views/editable_gradeform.py` & `devilry-6.0.0rc2/devilry/devilry_gradeform/views/editable_gradeform.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradeform/views/grade_form.py` & `devilry-6.0.0rc2/devilry/devilry_gradeform/views/grade_form.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradeform/views/setup_create_gradeform.py` & `devilry-6.0.0rc2/devilry/devilry_gradeform/views/setup_create_gradeform.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradeform/views/setup_gradeform.py` & `devilry-6.0.0rc2/devilry/devilry_gradeform/views/setup_gradeform.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradeform/views/viewable_gradeform.py` & `devilry-6.0.0rc2/devilry/devilry_gradeform/views/viewable_gradeform.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/models.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/pluginregistry.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/pluginregistry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/urls.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/migrations/0002_auto_20170108_0948.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/migrations/0002_auto_20170108_0948.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/bulkeditfeedbackbuttonbar.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/bulkeditfeedbackbuttonbar.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/editfeedbackbuttonbar.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/editfeedbackbuttonbar.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackbulkeditorbase.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackbulkeditorbase.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_bulkpreview.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_bulkpreview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_preview.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/feedbackdraft_preview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/base.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/currentprogress.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/currentprogress.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/select_points_to_grade_mapper.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/select_points_to_grade_mapper.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/selectplugin.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/selectplugin.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setmaxpoints.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setmaxpoints.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setpassing_grade_min_points.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setpassing_grade_min_points.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setup_custom_table.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/setup_custom_table.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/summary.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/admin/summary.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/editmarkdown.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/editmarkdown.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/feedbackeditorfilewidget.django.html` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/templates/devilry_gradingsystem/widgets/feedbackeditorfilewidget.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/helpers.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/test_models.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/test_download_feedbackdraftfile.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/test_download_feedbackdraftfile.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/test_feedbackdraft_preview.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/test_feedbackdraft_preview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/base.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_select_points_to_grade_mapper.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_select_points_to_grade_mapper.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_selectplugin.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_selectplugin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_setmaxpoints.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_setmaxpoints.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_setpassing_grade_min_points.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_setpassing_grade_min_points.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_setup_custom_table.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_setup_custom_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,27 +25,14 @@
                 points_to_grade_mapper='custom-table'
             )\
             .add_admins(self.admin1)
         self.url = reverse('devilry_gradingsystem_admin_setup_custom_table', kwargs={
             'assignmentid': self.assignmentbuilder.assignment.id,
         })
 
-    # def test_render(self):
-    #     myregistry = GradingSystemPluginRegistry()
-    #     myregistry.add(MockPointsPluginApi)
-    #     myregistry.add(MockApprovedPluginApi)
-    #     with patch('devilry.devilry_gradingsystem.views.admin.selectplugin.gradingsystempluginregistry', myregistry):
-    #         response = self.get_as(self.admin1)
-    #         self.assertEquals(response.status_code, 200)
-    #         html = response.content
-    #         self.assertEquals(cssGet(html, '.page-header h1').text.strip(),
-    #             'How would you like to configure the plugin?')
-    #         self.assertEquals(len(cssFind(html, '.devilry_gradingsystem_selectplugin_box')), 2)
-
-
     def test_post(self):
         with patch('devilry.apps.core.models.assignment.gradingsystempluginregistry', self.myregistry):
             response = self.post_as(self.admin1, {
                 'form-0-grade': ['F'],
                 'form-0-minimum_points': ['0'],
                 'form-1-grade': ['C'],
                 'form-1-minimum_points': ['50'],
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/tests/views/admin/test_summary.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/tests/views/admin/test_summary.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/download_feedbackdraftfile.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/download_feedbackdraftfile.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/feedbackbulkeditorbase.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/feedbackbulkeditorbase.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/feedbackdraft_bulkpreview.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/feedbackdraft_bulkpreview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/feedbackdraft_preview.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/feedbackdraft_preview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/feedbackeditorbase.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/feedbackeditorbase.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/base.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/select_points_to_grade_mapper.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/select_points_to_grade_mapper.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/selectplugin.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/selectplugin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/setmaxpoints.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/setmaxpoints.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/setpassing_grade_min_points.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/setpassing_grade_min_points.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/setup_custom_table.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/setup_custom_table.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/views/admin/summary.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/views/admin/summary.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/widgets/editmarkdown.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/widgets/editmarkdown.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystem/widgets/filewidget.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystem/widgets/filewidget.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_approved/apps.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_approved/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_approved/views/feedbackeditor.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_approved/views/feedbackeditor.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_points/apps.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_points/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_gradingsystemplugin_points/views/feedbackeditor.py` & `devilry-6.0.0rc2/devilry/devilry_gradingsystemplugin_points/views/feedbackeditor.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/admin.py` & `devilry-6.0.0rc2/devilry/devilry_group/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/apps.py` & `devilry-6.0.0rc2/devilry/devilry_group/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/devilry_group_baker_factories.py` & `devilry-6.0.0rc2/devilry/devilry_group/devilry_group_baker_factories.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/models.py` & `devilry-6.0.0rc2/devilry/devilry_group/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tasks.py` & `devilry-6.0.0rc2/devilry/devilry_group/tasks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/urls.py` & `devilry-6.0.0rc2/devilry/devilry_group/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/cradmin_instances/crinstance_admin.py` & `devilry-6.0.0rc2/devilry/devilry_group/cradmin_instances/crinstance_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/cradmin_instances/crinstance_base.py` & `devilry-6.0.0rc2/devilry/devilry_group/cradmin_instances/crinstance_base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/cradmin_instances/crinstance_examiner.py` & `devilry-6.0.0rc2/devilry/devilry_group/cradmin_instances/crinstance_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/cradmin_instances/crinstance_student.py` & `devilry-6.0.0rc2/devilry/devilry_group/cradmin_instances/crinstance_student.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/feedbackfeed_builder/builder_base.py` & `devilry-6.0.0rc2/devilry/devilry_group/feedbackfeed_builder/builder_base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_sidebarbuilder.py` & `devilry-6.0.0rc2/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_sidebarbuilder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_timelinebuilder.py` & `devilry-6.0.0rc2/devilry/devilry_group/feedbackfeed_builder/feedbackfeed_timelinebuilder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0003_auto_20160106_1418.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0003_auto_20160106_1418.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0004_auto_20160107_0918.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0004_auto_20160107_0918.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0007_auto_20160107_1031.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0007_auto_20160107_1031.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0008_auto_20160107_1053.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0008_auto_20160107_1053.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0009_auto_20160107_1100.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0009_auto_20160107_1100.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0010_auto_20160107_1106.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0010_auto_20160107_1106.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0011_auto_20160107_1111.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0011_auto_20160107_1111.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0012_auto_20160107_1129.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0012_auto_20160107_1129.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0013_auto_20160110_1621.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0013_auto_20160110_1621.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0014_feedbackset_grading_status.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0014_feedbackset_grading_status.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0015_auto_20160111_1245.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0015_auto_20160111_1245.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0016_auto_20160114_2202.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0016_auto_20160114_2202.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0017_auto_20160122_1518.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0017_auto_20160122_1518.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0019_auto_20160822_1945.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0019_auto_20160822_1945.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0019_auto_20160912_1649.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0019_auto_20160912_1649.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0023_auto_20170104_0551.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0023_auto_20170104_0551.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0024_auto_20170107_1838.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0024_auto_20170107_1838.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0025_auto_20170124_1504.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0025_auto_20170124_1504.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0026_datamigrate_update_for_no_none_values_in_feedbackset_deadline.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0026_datamigrate_update_for_no_none_values_in_feedbackset_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0027_auto_20170206_1146.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0027_auto_20170206_1146.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0027_auto_20170207_1951.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0027_auto_20170207_1951.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0030_auto_20170621_1734.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0030_auto_20170621_1734.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0032_auto_20180214_1654.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0032_auto_20180214_1654.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0033_feedbacksetgradingupdatehistory.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0033_feedbacksetgradingupdatehistory.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0034_feedbackset_last_updated_by.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0034_feedbackset_last_updated_by.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/migrations/0035_groupcommentedithistory.py` & `devilry-6.0.0rc2/devilry/devilry_group/migrations/0035_groupcommentedithistory.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_guidelines.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_guidelines.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/group_comment_edit_base.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/group_comment_edit_base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_base.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_admin/feedbackfeed_admin_base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_base.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/group_comment_history/comment_history.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/group_comment_history/comment_history.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/group_comment_history/history_item_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/group_comment_history/history_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/batch_download_archive_script.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/batch_download_archive_script.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/buttonbar.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/buttonbar.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/examiner.editlastdelivery.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/examiner.editlastdelivery.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/groupcomment_edit_delete_option.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/groupcomment_edit_delete_option.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/include/student_commentform_headingtext.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/include/student_commentform_headingtext.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/admin_groupcomment_item_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/admin_groupcomment_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/base_groupcomment_item_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/base_groupcomment_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/deadline_moved_item_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/deadline_moved_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/examiner_groupcomment_item_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/examiner_groupcomment_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/feedbackset_info_item_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/feedbackset_info_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_item_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_updated_item_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/grading_updated_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/student_groupcomment_item_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/student_groupcomment_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_comment_item_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_comment_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_feedbackset_item_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_feedbackset_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_file_item_value.django.html` & `devilry-6.0.0rc2/devilry/devilry_group/templates/devilry_group/listbuilder_sidebar/sidebar_file_item_value.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/templatetags/devilry_group_tags.py` & `devilry-6.0.0rc2/devilry/devilry_group/templatetags/devilry_group_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_devilry_group_mommy_factories.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_devilry_group_mommy_factories.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_templatetags.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_crinstance/test_crinstance_admin.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_crinstance/test_crinstance_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_crinstance/test_crinstance_examiner.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_crinstance/test_crinstance_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_crinstance/test_crinstance_student.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_crinstance/test_crinstance_student.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_download/test_batchdownload_api.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_download/test_batchdownload_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_download/test_batchframework_compression.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_download/test_batchframework_compression.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_download/test_feedbackfeed_bulkfiledownload.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_download/test_feedbackfeed_bulkfiledownload.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_download/test_feedbackfeed_filedownload.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_download/test_feedbackfeed_filedownload.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/admin/test_comment_edit_history.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/admin/test_comment_edit_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/admin/test_feedbackfeed_admin.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/admin/test_feedbackfeed_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_comment_edit_history.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_comment_edit_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_delete_comment.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_delete_comment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_discuss.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_discuss.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_comment.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_comment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_grade.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_edit_grade.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_feedback.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/examiner/test_feedbackfeed_examiner_feedback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_admin.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_common.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_common.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_examiner.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/mixins/mixin_feedbackfeed_examiner.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/student/test_comment_edit_history.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/student/test_comment_edit_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed/student/test_feedbackfeed_student.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed/student/test_feedbackfeed_student.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_sidebarbuilder.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_sidebarbuilder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_timeline_builder.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_feedbackfeed_builders/test_feedbackfeed_timeline_builder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_models/test_feedback_set.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_models/test_feedback_set.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_models/test_feedbackfeed_model.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_models/test_feedbackfeed_model.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_models/test_feedbackset_passed_pervious_period.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_models/test_feedbackset_passed_pervious_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/tests/test_models/test_group_comment.py` & `devilry-6.0.0rc2/devilry/devilry_group/tests/test_models/test_group_comment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/utils/download_response.py` & `devilry-6.0.0rc2/devilry/devilry_group/utils/download_response.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/cradmin_comment_history.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/cradmin_comment_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/cradmin_feedbackfeed_base.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/cradmin_feedbackfeed_base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/group_comment_edit_base.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/group_comment_edit_base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/admin/feedbackfeed_admin.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/admin/feedbackfeed_admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/admin/group_comment_history.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/admin/group_comment_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/admin/manage_deadline.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/admin/manage_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/download_files/backends.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/download_files/backends.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/download_files/batch_download_api.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/download_files/batch_download_api.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/download_files/batch_download_files.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/download_files/batch_download_files.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/download_files/feedbackfeed_bulkfiledownload.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/download_files/feedbackfeed_bulkfiledownload.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/examiner/feedbackfeed_examiner.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/examiner/feedbackfeed_examiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,14 @@
             comment_id=comment.id,
             domain_url_start=self.request.build_absolute_uri('/'))
 
     def save_object(self, form, commit=False):
         comment = super(ExaminerPublicDiscussView, self).save_object(form=form)
         comment.visibility = group_models.GroupComment.VISIBILITY_VISIBLE_TO_EVERYONE
         comment.published_datetime = timezone.now()
-        # self.__send_comment_email(comment=comment)
         return super(ExaminerPublicDiscussView, self).save_object(form=form, commit=True)
 
     def perform_after_save(self, comment):
         self.__send_comment_email(comment=comment)
 
     def get_success_url(self):
         return str(self.request.cradmin_app.reverse_appurl(viewname='public-discuss'))
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/examiner/group_comment_history.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/examiner/group_comment_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/examiner/manage_deadline.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/examiner/manage_deadline.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/student/feedbackfeed_student.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/student/feedbackfeed_student.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_group/views/student/group_comment_history.py` & `devilry-6.0.0rc2/devilry/devilry_group/views/student/group_comment_history.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_header/templates/devilry_header/about_me.django.html` & `devilry-6.0.0rc2/devilry/devilry_header/templates/devilry_header/about_me.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_header/templates/devilry_header/header2include.django.html` & `devilry-6.0.0rc2/devilry/devilry_header/templates/devilry_header/header2include.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_header/templates/devilry_header/includes/change_language.django.html` & `devilry-6.0.0rc2/devilry/devilry_header/templates/devilry_header/includes/change_language.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_header/tests/test_aboutme.py` & `devilry-6.0.0rc2/devilry/devilry_header/tests/test_aboutme.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_header/tests/test_change_language.py` & `devilry-6.0.0rc2/devilry/devilry_header/tests/test_change_language.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_header/views/about_me.py` & `devilry-6.0.0rc2/devilry/devilry_header/views/about_me.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_header/views/change_language.py` & `devilry-6.0.0rc2/devilry/devilry_header/views/change_language.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_help/tests.py` & `devilry-6.0.0rc2/devilry/devilry_help/tests.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_help/views.py` & `devilry-6.0.0rc2/devilry/devilry_help/views.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_help/templates/devilry_help/help.django.html` & `devilry-6.0.0rc2/devilry/devilry_help/templates/devilry_help/help.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_i18n/middleware.py` & `devilry-6.0.0rc2/devilry/devilry_i18n/middleware.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/models.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparser.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparser.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/management/commands/devilry_import_v2_database.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/management/commands/devilry_import_v2_database.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/__init__.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/__init__.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/assignment_importer.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/assignment_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/assignmentgroup_importer.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/assignmentgroup_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/candidate_examiner_importer.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/candidate_examiner_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/delivery_feedback_importers.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/delivery_feedback_importers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/feedbackset_importer.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/feedbackset_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/modelimporter_utils.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/modelimporter_utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/node_importer.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/node_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/period_importer.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/period_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/pointrange_to_grade_importer.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/pointrange_to_grade_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/qualifiesforexam_importer.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/qualifiesforexam_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/relateduser_importer.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/relateduser_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/subject_importer.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/subject_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/modelimporters/user_importer.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/modelimporters/user_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/scripts/user_add_missing_data_from_json.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/scripts/user_add_missing_data_from_json.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/importer_testcase_mixin.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/importer_testcase_mixin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentgroupimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentgroupimporter.py`

 * *Files 26% similar despite different names*

```diff
@@ -83,30 +83,14 @@
         self.create_v2dump(model_name='core.assignmentgroup',
                            data=self._create_assignmentgroup_dict(assignment=test_assignment))
         group_importer = AssignmentGroupImporter(input_root=self.temp_root_dir)
         group_importer.import_models()
         group = AssignmentGroup.objects.first()
         self.assertEqual(group.parentnode, test_assignment)
 
-    # def test_importer_imported_model_created(self):
-    #     test_assignment = baker.make('core.Assignment')
-    #     assignment_data_dict = self._create_assignmentgroup_dict(assignment=test_assignment)
-    #     self.create_v2dump(model_name='core.assignmentgroup',
-    #                        data=assignment_data_dict)
-    #     group_importer = AssignmentGroupImporter(input_root=self.temp_root_dir)
-    #     group_importer.import_models()
-    #     group = AssignmentGroup.objects.first()
-    #     self.assertEquals(ImportedModel.objects.count(), 1)
-    #     imported_model = ImportedModel.objects.get(
-    #         content_object_id=group.id,
-    #         content_type=ContentType.objects.get_for_model(model=group)
-    #     )
-    #     self.assertEquals(imported_model.content_object, group)
-    #     self.assertEquals(imported_model.data, assignment_data_dict)
-
     def test_auto_sequence_numbered_objects_uses_meta_max_id(self):
         test_assignment = baker.make('core.Assignment')
         self.create_v2dump(model_name='core.assignmentgroup',
                            data=self._create_assignmentgroup_dict(assignment=test_assignment),
                            model_meta=self._create_model_meta())
         group_importer = AssignmentGroupImporter(input_root=self.temp_root_dir)
         group_importer.import_models()
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_assignmentimporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,30 +199,14 @@
         self.create_v2dump(model_name='core.assignment',
                            data=self._create_assignment_dict(period=test_period))
         assignmentimporter = AssignmentImporter(input_root=self.temp_root_dir)
         assignmentimporter.import_models()
         assignment = Assignment.objects.first()
         self.assertEqual(assignment.parentnode, test_period)
 
-    # def test_importer_imported_model_created(self):
-    #     test_period = baker.make_recipe('devilry.apps.core.period_active')
-    #     assignment_data_dict = self._create_assignment_dict(period=test_period)
-    #     self.create_v2dump(model_name='core.assignment',
-    #                        data=assignment_data_dict)
-    #     assignmentimporter = AssignmentImporter(input_root=self.temp_root_dir)
-    #     assignmentimporter.import_models()
-    #     assignment = Assignment.objects.first()
-    #     self.assertEquals(ImportedModel.objects.count(), 1)
-    #     imported_model = ImportedModel.objects.get(
-    #         content_object_id=assignment.id,
-    #         content_type=ContentType.objects.get_for_model(model=assignment)
-    #     )
-    #     self.assertEquals(imported_model.content_object, assignment)
-    #     self.assertEquals(imported_model.data, assignment_data_dict)
-
     def test_auto_sequence_numbered_objects_uses_meta_max_id(self):
         test_period = baker.make_recipe('devilry.apps.core.period_active')
         self.create_v2dump(model_name='core.assignment',
                            data=self._create_assignment_dict(period=test_period),
                            model_meta=self._create_model_meta())
         assignmentimporter = AssignmentImporter(input_root=self.temp_root_dir)
         assignmentimporter.import_models()
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_candidateimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_candidateimporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,31 +104,14 @@
         self.create_v2dump(model_name='core.candidate',
                            data=self._create_candidate_dict(assignment_group=test_group, user=test_user))
         candidate_importer = CandidateImporter(input_root=self.temp_root_dir)
         candidate_importer.import_models()
         candidate = Candidate.objects.first()
         self.assertEqual(candidate.relatedstudent.period, test_group.parentnode.parentnode)
 
-    # def test_importer_imported_model_created(self):
-    #     test_user = baker.make(settings.AUTH_USER_MODEL)
-    #     test_group = baker.make('core.AssignmentGroup')
-    #     examiner_data_dict = self._create_candidate_dict(assignment_group=test_group, user=test_user)
-    #     self.create_v2dump(model_name='core.candidate',
-    #                        data=examiner_data_dict)
-    #     candidate_importer = CandidateImporter(input_root=self.temp_root_dir)
-    #     candidate_importer.import_models()
-    #     candidate = Candidate.objects.first()
-    #     self.assertEquals(ImportedModel.objects.count(), 1)
-    #     imported_model = ImportedModel.objects.get(
-    #         content_object_id=candidate.id,
-    #         content_type=ContentType.objects.get_for_model(model=candidate)
-    #     )
-    #     self.assertEquals(imported_model.content_object, candidate)
-    #     self.assertEquals(imported_model.data, examiner_data_dict)
-
     def test_auto_sequence_numbered_objects_uses_meta_max_id(self):
         test_user = baker.make(settings.AUTH_USER_MODEL)
         test_group = baker.make('core.AssignmentGroup')
         self.create_v2dump(model_name='core.candidate',
                            data=self._create_candidate_dict(assignment_group=test_group, user=test_user),
                            model_meta=self._create_model_meta())
         candidate_importer = CandidateImporter(input_root=self.temp_root_dir)
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_commentfilecontentimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_commentfilecontentimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_deliveryimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_deliveryimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_examinerimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_examinerimporter.py`

 * *Files 18% similar despite different names*

```diff
@@ -101,31 +101,14 @@
         self.create_v2dump(model_name='core.examiner',
                            data=self._create_examiner_dict(assignment_group=test_group, user=test_user))
         examiner_importer = ExaminerImporter(input_root=self.temp_root_dir)
         examiner_importer.import_models()
         examiner = Examiner.objects.first()
         self.assertEqual(examiner.relatedexaminer.period, test_group.parentnode.parentnode)
 
-    # def test_importer_imported_model_created(self):
-    #     test_user = baker.make(settings.AUTH_USER_MODEL)
-    #     test_group = baker.make('core.AssignmentGroup')
-    #     examiner_data_dict = self._create_examiner_dict(assignment_group=test_group, user=test_user)
-    #     self.create_v2dump(model_name='core.examiner',
-    #                        data=examiner_data_dict)
-    #     examiner_importer = ExaminerImporter(input_root=self.temp_root_dir)
-    #     examiner_importer.import_models()
-    #     examiner = Examiner.objects.first()
-    #     self.assertEquals(ImportedModel.objects.count(), 1)
-    #     imported_model = ImportedModel.objects.get(
-    #         content_object_id=examiner.id,
-    #         content_type=ContentType.objects.get_for_model(model=examiner)
-    #     )
-    #     self.assertEquals(imported_model.content_object, examiner)
-    #     self.assertEquals(imported_model.data, examiner_data_dict)
-
     def test_auto_sequence_numbered_objects_uses_meta_max_id(self):
         test_user = baker.make(settings.AUTH_USER_MODEL)
         test_group = baker.make('core.AssignmentGroup')
         self.create_v2dump(model_name='core.examiner',
                            data=self._create_examiner_dict(assignment_group=test_group, user=test_user),
                            model_meta=self._create_model_meta())
         examiner_importer = ExaminerImporter(input_root=self.temp_root_dir)
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_feedbacksetimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_feedbacksetimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_filemetaimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_filemetaimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_nodeimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_nodeimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_periodimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_periodimporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,31 +141,14 @@
         self.assertEqual(account_models.PermissionGroup.objects.count(), 1)
         self.assertEqual(account_models.PermissionGroupUser.objects.count(), 1)
         self.assertEqual(account_models.SubjectPermissionGroup.objects.count(), 1)
         periods_for_admin_list = Period.objects.filter_user_is_admin(test_admin_user)
         self.assertEqual(len(periods_for_admin_list), 1)
         self.assertEqual(periods_for_admin_list[0], period)
 
-    # def test_importer_imported_model_log_created(self):
-    #     test_admin_user = baker.make(settings.AUTH_USER_MODEL)
-    #     test_subject = baker.make('core.Subject')
-    #     period_data_dict = self._create_period_dict(subject=test_subject, test_admin_user=test_admin_user)
-    #     self.create_v2dump(model_name='core.period',
-    #                        data=period_data_dict)
-    #     periodimporter = PeriodImporter(input_root=self.temp_root_dir)
-    #     periodimporter.import_models()
-    #     period = Period.objects.first()
-    #     self.assertEquals(ImportedModel.objects.count(), 1)
-    #     imported_model = ImportedModel.objects.get(
-    #         content_object_id=period.id,
-    #         content_type=ContentType.objects.get_for_model(model=period)
-    #     )
-    #     self.assertEquals(imported_model.content_object, period)
-    #     self.assertEquals(imported_model.data, period_data_dict)
-
     def test_auto_sequence_numbered_objects_uses_meta_max_id(self):
         test_admin_user = baker.make(settings.AUTH_USER_MODEL)
         test_subject = baker.make('core.Subject')
         self.create_v2dump(model_name='core.period',
                            data=self._create_period_dict(subject=test_subject, test_admin_user=test_admin_user),
                            model_meta=self._create_model_meta())
         periodimporter = PeriodImporter(input_root=self.temp_root_dir)
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointrangetogradeimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointrangetogradeimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointtogrademapimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_pointtogrademapimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_qualifiesforexam_importer.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_qualifiesforexam_importer.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedexaminerimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedexaminerimporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,25 +51,14 @@
                            data=self._create_related_examiner_dict(period=test_period, user=test_user))
         relatedexaminer_importer = RelatedExaminerImporter(input_root=self.temp_root_dir)
         relatedexaminer_importer.import_models()
         related_examiner = RelatedExaminer.objects.first()
         self.assertEqual(related_examiner.pk, 6)
         self.assertEqual(related_examiner.id, 6)
 
-    # def test_importer_period_tag_period(self):
-    #     test_user = baker.make(settings.AUTH_USER_MODEL)
-    #     test_period = baker.make('core.Period')
-    #     self.create_v2dump(model_name='core.relatedexaminer',
-    #                        data=self._create_related_examiner_dict(period=test_period, user=test_user))
-    #     relatedexaminer_importer = RelatedExaminerImporter(input_root=self.temp_root_dir)
-    #     relatedexaminer_importer.import_models()
-    #     period_tag = PeriodTag.objects.first()
-    #     self.assertEquals(period_tag.period, test_period)
-    #     self.assertEquals(ImportedModel.objects.count(), 1)
-
     def test_importer_period_tag_single_tag_created(self):
         test_user = baker.make(settings.AUTH_USER_MODEL)
         test_period = baker.make('core.Period')
         self.create_v2dump(model_name='core.relatedexaminer',
                            data=self._create_related_examiner_dict(period=test_period, user=test_user))
         relatedexaminer_importer = RelatedExaminerImporter(input_root=self.temp_root_dir)
         relatedexaminer_importer.import_models()
@@ -130,31 +119,14 @@
         relatedexaminer_importer.import_models()
         related_examiner = RelatedExaminer.objects.first()
         period_tags = PeriodTag.objects.all()
         self.assertEqual(period_tags.count(), 4)
         for period_tag in period_tags:
             self.assertIn(related_examiner, period_tag.relatedexaminers.all())
 
-    # def test_importer_imported_model_created(self):
-    #     test_user = baker.make(settings.AUTH_USER_MODEL)
-    #     test_period = baker.make('core.Period')
-    #     related_examiner_data_dict = self._create_related_examiner_dict(period=test_period, user=test_user)
-    #     self.create_v2dump(model_name='core.relatedexaminer',
-    #                        data=related_examiner_data_dict)
-    #     relatedexaminer_importer = RelatedExaminerImporter(input_root=self.temp_root_dir)
-    #     relatedexaminer_importer.import_models()
-    #     related_examiner = RelatedExaminer.objects.first()
-    #     self.assertEquals(ImportedModel.objects.count(), 1)
-    #     imported_model = ImportedModel.objects.get(
-    #         content_object_id=related_examiner.id,
-    #         content_type=ContentType.objects.get_for_model(model=related_examiner)
-    #     )
-    #     self.assertEquals(imported_model.content_object, related_examiner)
-    #     self.assertEquals(imported_model.data, related_examiner_data_dict)
-
     def test_auto_sequence_numbered_objects_uses_meta_max_id(self):
         test_user = baker.make(settings.AUTH_USER_MODEL)
         test_period = baker.make('core.Period')
         self.create_v2dump(model_name='core.relatedexaminer',
                            data=self._create_related_examiner_dict(period=test_period, user=test_user),
                            model_meta=self._create_model_meta())
         relatedexaminer_importer = RelatedExaminerImporter(input_root=self.temp_root_dir)
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedstudentimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_relatedstudentimporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,31 +130,14 @@
         relatedstudent_importer.import_models()
         related_examiner = RelatedStudent.objects.first()
         period_tags = PeriodTag.objects.all()
         self.assertEqual(period_tags.count(), 4)
         for period_tag in period_tags:
             self.assertIn(related_examiner, period_tag.relatedstudents.all())
 
-    # def test_importer_imported_model_created(self):
-    #     test_user = baker.make(settings.AUTH_USER_MODEL)
-    #     test_period = baker.make('core.Period')
-    #     related_student_data_dict = self._create_related_student_dict(period=test_period, user=test_user)
-    #     self.create_v2dump(model_name='core.relatedstudent',
-    #                        data=related_student_data_dict)
-    #     relatedstudent_importer = RelatedStudentImporter(input_root=self.temp_root_dir)
-    #     relatedstudent_importer.import_models()
-    #     related_student = RelatedStudent.objects.first()
-    #     self.assertEquals(ImportedModel.objects.count(), 1)
-    #     imported_model = ImportedModel.objects.get(
-    #         content_object_id=related_student.id,
-    #         content_type=ContentType.objects.get_for_model(model=related_student)
-    #     )
-    #     self.assertEquals(imported_model.content_object, related_student)
-    #     self.assertEquals(imported_model.data, related_student_data_dict)
-
     def test_auto_sequence_numbered_objects_uses_meta_max_id(self):
         test_user = baker.make(settings.AUTH_USER_MODEL)
         test_period = baker.make('core.Period')
         self.create_v2dump(model_name='core.relatedstudent',
                            data=self._create_related_student_dict(period=test_period, user=test_user),
                            model_meta=self._create_model_meta())
         relatedstudent_importer = RelatedStudentImporter(input_root=self.temp_root_dir)
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_staticfeedbackimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_staticfeedbackimporter.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_subjectimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_subjectimporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,30 +98,14 @@
         subject = Subject.objects.first()
         self.assertEqual(account_models.PermissionGroup.objects.count(), 1)
         self.assertEqual(account_models.SubjectPermissionGroup.objects.count(), 1)
         subjects_for_admin_list = Subject.objects.filter_user_is_admin(test_admin_user)
         self.assertEqual(len(subjects_for_admin_list), 1)
         self.assertEqual(subjects_for_admin_list[0], subject)
 
-    # def test_importer_imported_model_created(self):
-    #     test_admin_user = baker.make(settings.AUTH_USER_MODEL)
-    #     subject_data_dict = self._create_subject_dict(test_admin_user=test_admin_user)
-    #     self.create_v2dump(model_name='core.subject',
-    #                        data=subject_data_dict)
-    #     subjectimporter = SubjectImporter(input_root=self.temp_root_dir)
-    #     subjectimporter.import_models()
-    #     subject = Subject.objects.first()
-    #     self.assertEquals(ImportedModel.objects.count(), 1)
-    #     imported_model = ImportedModel.objects.get(
-    #         content_object_id=subject.id,
-    #         content_type=ContentType.objects.get_for_model(model=subject)
-    #     )
-    #     self.assertEquals(imported_model.content_object, subject)
-    #     self.assertEquals(imported_model.data, subject_data_dict)
-
     def test_auto_sequence_numbered_objects_uses_meta_max_id(self):
         test_admin_user = baker.make(settings.AUTH_USER_MODEL)
         self.create_v2dump(model_name='core.subject',
                            data=self._create_subject_dict(test_admin_user=test_admin_user),
                            model_meta=self._create_model_meta())
         subjectimporter = SubjectImporter(input_root=self.temp_root_dir)
         subjectimporter.import_models()
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_modelimporters/test_userimporter.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_modelimporters/test_userimporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,25 +111,14 @@
                            data=user_dict,
                            model_meta=self._create_model_meta())
         userimporter = UserImporter(input_root=self.temp_root_dir)
         userimporter.import_models()
         user = get_user_model().objects.first()
         self.assertIsNotNone(user.last_login)
 
-    # Does not seem to work, but that does not matter since
-    # all known v2 installs use unusable password and custom
-    # login backend
-    # def test_importer_password(self):
-    #     self.create_v2dump(model_name='auth.user',
-    #                        data=self._create_user_dict())
-    #     userimporter = UserImporter(input_root=self.temp_root_dir)
-    #     userimporter.import_models()
-    #     user = get_user_model().objects.first()
-    #     self.assertEquals(user.password, 'md5$krPxlZzbpjsm$8f4799f31464dfd7f907d4321883afcf')
-
     def test_importer_useremail(self):
         self.create_v2dump(model_name='auth.user',
                            data=self._create_user_dict(),
                            model_meta=self._create_model_meta())
         userimporter = UserImporter(input_root=self.temp_root_dir)
         userimporter.import_models()
         self.assertEqual(UserEmail.objects.count(), 1)
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/tests/test_scripts/test_user_add_missing_data_from_json.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/tests/test_scripts/test_user_add_missing_data_from_json.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_import_v2database/v2dump_directoryparsers/__init__.py` & `devilry-6.0.0rc2/devilry/devilry_import_v2database/v2dump_directoryparsers/__init__.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_markup/parse_markdown.py` & `devilry-6.0.0rc2/devilry/devilry_markup/parse_markdown.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_markup/views.py` & `devilry-6.0.0rc2/devilry/devilry_markup/views.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_markup/markdown_extensions/code_diff.py` & `devilry-6.0.0rc2/devilry/devilry_markup/markdown_extensions/code_diff.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_markup/markdown_extensions/latex_math.py` & `devilry-6.0.0rc2/devilry/devilry_markup/markdown_extensions/latex_math.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_markup/templates/devilry_markup/code_diff.html` & `devilry-6.0.0rc2/devilry/devilry_markup/templates/devilry_markup/code_diff.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_message/admin.py` & `devilry-6.0.0rc2/devilry/devilry_message/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_message/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/devilry_message/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_message/migrations/0002_auto_20210427_1350.py` & `devilry-6.0.0rc2/devilry/devilry_message/migrations/0002_auto_20210427_1350.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_message/models/base.py` & `devilry-6.0.0rc2/devilry/devilry_message/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from ievv_opensource.utils import choices_with_meta
 
 from devilry.devilry_email.utils import activate_translation_for_user
 from devilry.utils.devilry_email import send_message
 
 
-class MessageReceiverQuerySet(models.QuerySet):
+class MessageQuerySet(models.QuerySet):
     def filter_message_with_no_message_receivers(self):
         """
         Filter all :obj:`.Message`s without any :class:`.MessageReceiver`s.
         """
         return self.annotate(receiver_count=models.Count('messagereceiver'))\
             .filter(receiver_count=0)
 
@@ -37,15 +37,15 @@
     status of the message and creates recipients for the email to be sent.
 
     Notes:
         The actual subject and message-content is stored on each :class:`.MessageReceiver` with a
         foreignkey to this class. The reason for this being that we want to save the subject and content
         in the preferred language of the user.
     """
-    objects = MessageReceiverQuerySet.as_manager()
+    objects = MessageQuerySet.as_manager()
 
     #: When the message was created.
     created_datetime = models.DateTimeField(
         blank=True, null=True, default=timezone.now
     )
 
     #: The user that created the message.
@@ -116,15 +116,21 @@
         choices_with_meta.Choice(value='deadline_moved',
                                  label='Deadline moved'),
         choices_with_meta.Choice(value='new_attempt',
                                  label='New attempt'),
         choices_with_meta.Choice(value='feedback',
                                  label='Feedback'),
         choices_with_meta.Choice(value='feedback_updated',
-                                 label='Grading updated')
+                                 label='Grading updated'),
+        choices_with_meta.Choice(value='group_invite_invitation',
+                                 label='Group invitation: invitation'),
+        choices_with_meta.Choice(value='group_invite_accepted',
+                                 label='Group invitation: accepted'),
+        choices_with_meta.Choice(value='group_invite_rejected',
+                                 label='Group invitation: rejected'),
     )
 
     #: The context type of the message.
     #: See `CONTEXT_TYPE_CHOICES` for more info.
     context_type = models.CharField(
         max_length=255,
         blank=False, null=False,
@@ -285,15 +291,14 @@
             subject_generator: A subclass of
                 :class:`devilry.devilry_message.utils.subject_generator.SubjectTextGenerator`
             template_name: Template to render content with (a path).
             template_context: Context data for template.
 
         Returns:
             :class:`.MessageRecveiver`: Unsaved instance.
-
         """
         current_language = translation.get_language()
         activate_translation_for_user(user=user)
         message_receiver = MessageReceiver(
             user=user,
             message=message,
             message_type=message_type,
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_message/tests/test_message.py` & `devilry-6.0.0rc2/devilry/devilry_message/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_message/tests/test_message_receiver.py` & `devilry-6.0.0rc2/devilry/devilry_message/tests/test_message_receiver.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/admin.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/apps.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/apps.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/cradmin_app.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/cradmin_app.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/models.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/pluginhelpers.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/pluginhelpers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/plugintyperegistry.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/plugintyperegistry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/listbuilder/plugin_listbuilder_list.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/listbuilder/plugin_listbuilder_list.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/migrations/0002_auto_20170223_1112.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/migrations/0002_auto_20170223_1112.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/migrations/0005_deletedqualifiesforfinalexam.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/migrations/0005_deletedqualifiesforfinalexam.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tablebuilder/tablebuilder.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tablebuilder/tablebuilder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/base.django.html` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/base.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/list_statuses.django.html` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/list_statuses.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/print_view.html` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/print_view.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/retract_status.django.html` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/retract_status.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/selectplugin.django.html` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/selectplugin.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_preview.django.html` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_preview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_show.html` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/status_show.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/includes/qualification_table.django.html` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/includes/qualification_table.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/description.django.html` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/templates/devilry_qualifiesforexam/listbuilder/description.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_list_statuses_view.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_list_statuses_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_models.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_plugin_listbuilder_list.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_plugin_listbuilder_list.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_pluginhelpers.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_pluginhelpers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_pluginselection_view.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_pluginselection_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_plugintyperegistry.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_plugintyperegistry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_preview.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_preview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/tests/test_showstatus.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/tests/test_showstatus.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/utils/groups_groupedby_relatedstudent_and_assignments.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/utils/groups_groupedby_relatedstudent_and_assignments.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/views/list_statuses_view.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/views/list_statuses_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/views/pluginselection_view.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/views/pluginselection_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/views/proxyview.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/views/proxyview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/views/qualification_preview_view.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/views/qualification_preview_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam/views/plugin_base_views/base_multiselect_view.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam/views/plugin_base_views/base_multiselect_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/plugin.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/plugin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/resultscollector.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/resultscollector.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/tests/test_resultscollector.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/tests/test_resultscollector.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_approved/views/select_assignment.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_approved/views/select_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_points/plugin.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_points/plugin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_points/resultscollector.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_points/resultscollector.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_points/tests/test_resultscollector.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_points/tests/test_resultscollector.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_points/views/select_assignment_and_points.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_points/views/select_assignment_and_points.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_students/plugin.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_students/plugin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_students/tests/test_student_selection_view.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_students/tests/test_student_selection_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_qualifiesforexam_plugin_students/views/select_students.py` & `devilry-6.0.0rc2/devilry/devilry_qualifiesforexam_plugin_students/views/select_students.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_report/abstract_generator.py` & `devilry-6.0.0rc2/devilry/devilry_report/abstract_generator.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_report/admin.py` & `devilry-6.0.0rc2/devilry/devilry_report/admin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_report/generator_registry.py` & `devilry-6.0.0rc2/devilry/devilry_report/generator_registry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_report/models.py` & `devilry-6.0.0rc2/devilry/devilry_report/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_report/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/devilry_report/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_report/migrations/0002_auto_20210427_1350.py` & `devilry-6.0.0rc2/devilry/devilry_report/migrations/0002_auto_20210427_1350.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_report/templates/devilry_report/download_report.django.html` & `devilry-6.0.0rc2/devilry/devilry_report/templates/devilry_report/download_report.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_report/tests/test_download_report_view.py` & `devilry-6.0.0rc2/devilry/devilry_report/tests/test_download_report_view.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_report/tests/test_generator_registry.py` & `devilry-6.0.0rc2/devilry/devilry_report/tests/test_generator_registry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_report/tests/test_report_model.py` & `devilry-6.0.0rc2/devilry/devilry_report/tests/test_report_model.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_report/views/download_report.py` & `devilry-6.0.0rc2/devilry/devilry_report/views/download_report.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_resetpassword/urls.py` & `devilry-6.0.0rc2/devilry/devilry_resetpassword/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_rest/auth.py` & `devilry-6.0.0rc2/devilry/devilry_rest/auth.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_rest/formfields.py` & `devilry-6.0.0rc2/devilry/devilry_rest/formfields.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_rest/serializehelpers.py` & `devilry-6.0.0rc2/devilry/devilry_rest/serializehelpers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_rest/testclient.py` & `devilry-6.0.0rc2/devilry/devilry_rest/testclient.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_rest/tests/test_serializehelpers.py` & `devilry-6.0.0rc2/devilry/devilry_rest/tests/test_serializehelpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 from unittest import TestCase
 
 from devilry.devilry_rest.serializehelpers import format_timedelta, format_datetime
 
 
 class TestRestFormat(TestCase):
     def test_format_datetime(self):
-        self.assertEquals(format_datetime(datetime(2012, 1, 27, 14, 40, 45)),
+        self.assertEqual(format_datetime(datetime(2012, 1, 27, 14, 40, 45)),
                           '2012-01-27 14:40:45')
 
     def _test_delta(self, mk):
-        self.assertEquals(format_timedelta(mk(datetime(2005, 5, 20, 15, 20, 0),
+        self.assertEqual(format_timedelta(mk(datetime(2005, 5, 20, 15, 20, 0),
                                               datetime(2005, 5, 20, 15, 15, 0))),
                           {'days': 0, 'hours': 0, 'minutes': 5, 'seconds': 0})
-        self.assertEquals(format_timedelta(mk(datetime(2005, 5, 20, 15, 0, 20),
+        self.assertEqual(format_timedelta(mk(datetime(2005, 5, 20, 15, 0, 20),
                                               datetime(2005, 5, 20, 15, 0, 10))),
                           {'days': 0, 'hours': 0, 'minutes': 0, 'seconds': 10})
-        self.assertEquals(format_timedelta(mk(datetime(2005, 5, 20, 15, 0, 0),
+        self.assertEqual(format_timedelta(mk(datetime(2005, 5, 20, 15, 0, 0),
                                               datetime(2005, 5, 20, 14, 0, 0))),
                           {'days': 0, 'hours': 1, 'minutes': 0, 'seconds': 0})
-        self.assertEquals(format_timedelta(mk(datetime(2005, 5, 20, 14, 0, 0),
+        self.assertEqual(format_timedelta(mk(datetime(2005, 5, 20, 14, 0, 0),
                                               datetime(2005, 5, 19, 14, 0, 0))),
                           {'days': 1, 'hours': 0, 'minutes': 0, 'seconds': 0})
-        self.assertEquals(format_timedelta(mk(datetime(2005, 5, 20, 14, 0, 0),
+        self.assertEqual(format_timedelta(mk(datetime(2005, 5, 20, 14, 0, 0),
                                               datetime(2005, 2, 20, 14, 0, 0))),
                           {'days': 89, 'hours': 0, 'minutes': 0, 'seconds': 0})
-        self.assertEquals(format_timedelta(mk(datetime(2005, 5, 20, 15, 20, 12),
+        self.assertEqual(format_timedelta(mk(datetime(2005, 5, 20, 15, 20, 12),
                                               datetime(2005, 5, 20, 14, 0, 0))),
                           {'days': 0, 'hours': 1, 'minutes': 20, 'seconds': 12})
 
     def test_format_timedelta_positive(self):
         self._test_delta(lambda a, b: a-b)
 
     def test_format_timedelta_negative(self):
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_sandbox/sandbox.py` & `devilry-6.0.0rc2/devilry/devilry_sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_sandbox/urls.py` & `devilry-6.0.0rc2/devilry/devilry_sandbox/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_sandbox/views.py` & `devilry-6.0.0rc2/devilry/devilry_sandbox/views.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_sandbox/management/commands/devilry_sandboxcreate.py` & `devilry-6.0.0rc2/devilry/devilry_sandbox/management/commands/devilry_sandboxcreate.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_sandbox/templates/devilry_sandbox/createsubject.django.html` & `devilry-6.0.0rc2/devilry/devilry_sandbox/templates/devilry_sandbox/createsubject.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_settings/views.py` & `devilry-6.0.0rc2/devilry/devilry_settings/views.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/urls.py` & `devilry-6.0.0rc2/devilry/devilry_statistics/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/api/assignment/api_utils.py` & `devilry-6.0.0rc2/devilry/devilry_statistics/api/assignment/api_utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/api/assignment/examiner_average_grading_points.py` & `devilry-6.0.0rc2/devilry/devilry_statistics/api/assignment/examiner_average_grading_points.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/api/assignment/examiner_details.py` & `devilry-6.0.0rc2/devilry/devilry_statistics/api/assignment/examiner_details.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/api/assignment/examiner_group_results.py` & `devilry-6.0.0rc2/devilry/devilry_statistics/api/assignment/examiner_group_results.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/management/commands/devilry_create_test_course.py` & `devilry-6.0.0rc2/devilry/devilry_statistics/management/commands/devilry_create_test_course.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/management/commands/devilry_statistics_make_assignment_with_graded_groups.py` & `devilry-6.0.0rc2/devilry/devilry_statistics/management/commands/devilry_statistics_make_assignment_with_graded_groups.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/static/devilry_statistics/6.0.0rc1/devilry_statistics_all.js` & `devilry-6.0.0rc2/devilry/devilry_statistics/static/devilry_statistics/6.0.0rc2/devilry_statistics_all.js`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/package-lock.json` & `devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/package-lock.json`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/package.json` & `devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/package.json`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/devilry_statistics_all.js` & `devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/devilry_statistics_all.js`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerAverageGradingPointsWidget.js` & `devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerAverageGradingPointsWidget.js`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerDetailsWidget.js` & `devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerDetailsWidget.js`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerGroupResultWidget.js` & `devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/ExaminerGroupResultWidget.js`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/registerAllWidgets.js` & `devilry-6.0.0rc2/devilry/devilry_statistics/staticsources/devilry_statistics/scripts/javascript/widgets/registerAllWidgets.js`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/tests/test_api_examiner_average_grading_points.py` & `devilry-6.0.0rc2/devilry/devilry_statistics/tests/test_api_examiner_average_grading_points.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/tests/test_api_examiner_details.py` & `devilry-6.0.0rc2/devilry/devilry_statistics/tests/test_api_examiner_details.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_statistics/tests/test_api_examiner_group_result.py` & `devilry-6.0.0rc2/devilry/devilry_statistics/tests/test_api_examiner_group_result.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/models.py` & `devilry-6.0.0rc2/devilry/devilry_student/models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/urls.py` & `devilry-6.0.0rc2/devilry/devilry_student/urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/cradminextensions/columntypes.py` & `devilry-6.0.0rc2/devilry/devilry_student/cradminextensions/columntypes.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/cradminextensions/devilry_crmenu_student.py` & `devilry-6.0.0rc2/devilry/devilry_student/cradminextensions/devilry_crmenu_student.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/migrations/0001_initial.py` & `devilry-6.0.0rc2/devilry/devilry_student/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html` & `devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/add_delivery.django.html` & `devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/add_delivery.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/contactapp/contact.django.html` & `devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/contactapp/contact.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery-status-column.django.html` & `devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery-status-column.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_details.django.html` & `devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_details.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_list.django.html` & `devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_list.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/overviewapp/overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/overviewapp/overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_delete.django.html` & `devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_delete.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond.django.html` & `devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond_standalone.django.html` & `devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/groupinvite_respond_standalone.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/projectgroup_overview.django.html` & `devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/projectgroup_overview.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/delivery-summary-column.django.html` & `devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/cradminextensions/columntypes/delivery-summary-column.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templates/devilry_student/dashboard/dashboard.django.html` & `devilry-6.0.0rc2/devilry/devilry_student/templates/devilry_student/dashboard/dashboard.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/templatetags/devilry_student_tags.py` & `devilry-6.0.0rc2/devilry/devilry_student/templatetags/devilry_student_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/tests/test_models.py` & `devilry-6.0.0rc2/devilry/devilry_student/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/tests/test_templatetags.py` & `devilry-6.0.0rc2/devilry/devilry_student/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/tests/test_cradminextensions/test_devilry_crmenu_student.py` & `devilry-6.0.0rc2/devilry/devilry_student/tests/test_cradminextensions/test_devilry_crmenu_student.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/tests/test_dashboard/test_allperiods.py` & `devilry-6.0.0rc2/devilry/devilry_student/tests/test_dashboard/test_allperiods.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/tests/test_dashboard/test_dashboard.py` & `devilry-6.0.0rc2/devilry/devilry_student/tests/test_dashboard/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/tests/test_group/test_projectgroupapp.py` & `devilry-6.0.0rc2/devilry/devilry_student/tests/test_group/test_projectgroupapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1652,15 +1652,15 @@
         group = baker.make('core.AssignmentGroup', parentnode=testassignment)
         group1 = baker.make('core.AssignmentGroup', parentnode=testassignment)
         candidate = core_baker.candidate(group=group, fullname="April Duck", shortname="april@example.com")
         candidate1 = core_baker.candidate(group=group1, fullname="Dewey Duck", shortname="dewey@example.com")
         invite = baker.make('core.GroupInvite', group=group,
                             sent_by=candidate.relatedstudent.user, sent_to=candidate1.relatedstudent.user)
 
-        with self.assertNumQueries(13):
+        with self.assertNumQueries(26):
             self.mock_http302_postrequest(
                 requestuser=candidate1.relatedstudent.user,
                 viewkwargs={
                     'invite_id': invite.id
                 },
                 requestkwargs={
                     'data': {
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/tests/test_period/test_overview.py` & `devilry-6.0.0rc2/devilry/devilry_student/tests/test_period/test_overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/views/show_delivery.py` & `devilry-6.0.0rc2/devilry/devilry_student/views/show_delivery.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/views/dashboard/allperiods.py` & `devilry-6.0.0rc2/devilry/devilry_student/views/dashboard/allperiods.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/views/dashboard/crinstance_dashboard.py` & `devilry-6.0.0rc2/devilry/devilry_student/views/dashboard/crinstance_dashboard.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/views/dashboard/dashboard.py` & `devilry-6.0.0rc2/devilry/devilry_student/views/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/views/group/projectgroupapp.py` & `devilry-6.0.0rc2/devilry/devilry_student/views/group/projectgroupapp.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/views/period/crinstance_period.py` & `devilry-6.0.0rc2/devilry/devilry_student/views/period/crinstance_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_student/views/period/overview.py` & `devilry-6.0.0rc2/devilry/devilry_student/views/period/overview.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/delete_periods/period_delete.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/delete_periods/period_delete.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/examples/relatedstudents_email_instead_of_username.json` & `devilry-6.0.0rc2/devilry/devilry_superadmin/examples/relatedstudents_email_instead_of_username.json`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_anonymize_database.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_anonymize_database.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_compressed_archives.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_compressed_archives.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_inactive_users.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_inactive_users.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_message_receivers.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_message_receivers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_messages_without_receivers.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_messages_without_receivers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_delete_periods.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_delete_periods.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_fix_missing_first_feedbackset.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_fix_missing_first_feedbackset.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_mark_as_passed_in_previous_period.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_mark_as_passed_in_previous_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodadd.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodadminadd.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodadminadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodadminclear.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodadminclear.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodsearch.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodsearch.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedexaminers.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedexaminers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedstudents.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_periodsetrelatedstudents.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_permissiongroup_add_subject.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_permissiongroup_add_subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_qualifiedforfinalexam_delete_duplicates.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_qualifiedforfinalexam_delete_duplicates.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_rename_periodtag_prefix.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_rename_periodtag_prefix.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_resend_failed_messages.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_resend_failed_messages.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_setup_dataporten_provider.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_setup_dataporten_provider.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_setup_primary_domain.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_setup_primary_domain.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_show_assignment_guidelines.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_show_assignment_guidelines.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectadd.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectadminadd.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectadminadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectadminclear.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectadminclear.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_subjectsearch.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_subjectsearch.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_test_rq_task.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_test_rq_task.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_useradd.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_useradd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_useraddbulk.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_useraddbulk.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_usermerge.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_usermerge.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/management/commands/devilry_usermod.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/management/commands/devilry_usermod.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_inactive_users.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_inactive_users.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_periods.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_delete_periods.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminadd.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminclear.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_periodadminclear.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_permissiongroup_add_subject.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_permissiongroup_add_subject.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_qualifiedforfinalexam_delete_duplicates.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_qualifiedforfinalexam_delete_duplicates.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadd.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminadd.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminadd.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminclear.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_subjectadminclear.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_useraddbulk.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_useraddbulk.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_usermod.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_devilry_usermod.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_superadmin/tests/test_management_commands/test_resend_failed_messages.py` & `devilry-6.0.0rc2/devilry/devilry_superadmin/tests/test_management_commands/test_resend_failed_messages.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/media/images/groovepaper.png` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/media/images/groovepaper.png`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/media/images/favicons/apple-touch-icon.png` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/media/images/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/media/images/favicons/favicon.ico` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/media/images/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/devilry_all.js` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/devilry_all.js`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/devilry_all.js.map` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/devilry_all.js.map`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/katex/LICENSE` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/katex/LICENSE`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/katex/katex.min.css` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/katex/katex.min.css`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/katex/katex.mjs` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/katex/katex.mjs`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/commentEditor.js` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/commentEditor.js`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/cookie.js` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/cookie.js`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/examinerSelfAssignButton.js` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/examinerSelfAssignButton.js`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/feedbackfeedNavigationHandler.js` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/feedbackfeedNavigationHandler.js`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/fileupload.js` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/fileupload.js`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/scripts/plain_es6/latex_math.js` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/scripts/plain_es6/latex_math.js`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/styles/cradmin_theme_devilry_mainpages/theme.css` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/styles/cradmin_theme_devilry_mainpages/theme.css`

 * *Files 0% similar despite different names*

```diff
@@ -7348,14 +7348,18 @@
 }
 .alert.alert-danger .btn.btn-default:hover,
 .alert.alert-warning .btn.btn-default:hover {
   background: #191919;
   border-color: #191919;
   color: #fff;
 }
+.alert.alert-danger a,
+.alert.alert-warning a {
+  color: #fef6f5;
+}
 a.cradmin-legacy-listbuilder-itemframe-link.devilry-cradmin-legacy-listbuilder-itemframe-goforward {
   position: relative;
 }
 a.cradmin-legacy-listbuilder-itemframe-link.devilry-cradmin-legacy-listbuilder-itemframe-goforward .devilry-cradmin-legacy-listbuilder-itemframe-goforward-icon {
   color: #ddd;
   font-size: 50px;
   position: absolute;
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc1/styles/cradmin_theme_devilry_superuserui/theme.css` & `devilry-6.0.0rc2/devilry/devilry_theme3/static/devilry_theme3/6.0.0rc2/styles/cradmin_theme_devilry_superuserui/theme.css`

 * *Files 0% similar despite different names*

```diff
@@ -7440,14 +7440,18 @@
 }
 .alert.alert-danger .btn.btn-default:hover,
 .alert.alert-warning .btn.btn-default:hover {
   background: #191919;
   border-color: #191919;
   color: #fff;
 }
+.alert.alert-danger a,
+.alert.alert-warning a {
+  color: #fef6f5;
+}
 a.cradmin-legacy-listbuilder-itemframe-link.devilry-cradmin-legacy-listbuilder-itemframe-goforward {
   position: relative;
 }
 a.cradmin-legacy-listbuilder-itemframe-link.devilry-cradmin-legacy-listbuilder-itemframe-goforward .devilry-cradmin-legacy-listbuilder-itemframe-goforward-icon {
   color: #ddd;
   font-size: 50px;
   position: absolute;
```

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/templates/devilry_theme3/wcag-debug.django.html` & `devilry-6.0.0rc2/devilry/devilry_theme3/templates/devilry_theme3/wcag-debug.django.html`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/devilry_theme3/templatetags/devilry_theme3_tags.py` & `devilry-6.0.0rc2/devilry/devilry_theme3/templatetags/devilry_theme3_tags.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/django_decoupled_docs/README.rst` & `devilry-6.0.0rc2/devilry/django_decoupled_docs/README.rst`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/django_decoupled_docs/registry.py` & `devilry-6.0.0rc2/devilry/django_decoupled_docs/registry.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/locale/en/LC_MESSAGES/django.po` & `devilry-6.0.0rc2/devilry/locale/en/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-07 08:34+0200\n"
+"POT-Creation-Date: 2023-07-19 14:06+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -302,34 +302,34 @@
 msgid "Closed without feedback"
 msgstr ""
 
 #: devilry/apps/core/models/assignment_group.py:1009
 msgid "Waiting for something"
 msgstr ""
 
-#: devilry/apps/core/models/assignment_group.py:1215
+#: devilry/apps/core/models/assignment_group.py:1226
 #: devilry/apps/core/templates/devilry_core/templatetags/multiple-candidates-long-displayname.django.html:8
 #: devilry/apps/core/templates/devilry_core/templatetags/multiple-candidates-short-displayname.django.html:8
 msgctxt "core assignmentgroup"
 msgid "no students in group"
 msgstr ""
 
-#: devilry/apps/core/models/assignment_group.py:1219
+#: devilry/apps/core/models/assignment_group.py:1230
 #, python-format
 msgctxt "core assignmentgroup"
 msgid "group#%(groupid)s - no students in group"
 msgstr ""
 
-#: devilry/apps/core/models/assignment_group.py:1580
+#: devilry/apps/core/models/assignment_group.py:1591
 msgid ""
 "Cannot merge self into target, self and target is not part of same "
 "AssignmentGroup"
 msgstr ""
 
-#: devilry/apps/core/models/assignment_group.py:1633
+#: devilry/apps/core/models/assignment_group.py:1644
 msgid "Cannot merge less than 2 groups"
 msgstr ""
 
 #: devilry/apps/core/models/basenode.py:53
 msgid "Path"
 msgstr ""
 
@@ -341,24 +341,24 @@
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:37
 #: devilry/devilry_admin/views/dashboard/overview.py:107
 msgid "Short name"
 msgstr ""
 
 #: devilry/apps/core/models/custom_db_fields.py:22
 msgid ""
-"Up to 20 letters of lowercase english letters (a-z), numbers, underscore (\"_"
-"\") and hyphen (\"-\"). Used when the name takes too much space."
+"Up to 20 letters of lowercase english letters (a-z), numbers, underscore "
+"(\"_\") and hyphen (\"-\"). Used when the name takes too much space."
 msgstr ""
 
 #: devilry/apps/core/models/custom_db_fields.py:33
 msgid "Can only contain numbers, lowercase letters, '_' and '-'. "
 msgstr ""
 
 #: devilry/apps/core/models/custom_db_fields.py:40
-#: devilry/devilry_account/models.py:926
+#: devilry/devilry_account/models.py:934
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:28
 #: devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py:24
 #: devilry/devilry_cradmin/devilry_listfilter/assignment.py:17
 #: devilry/devilry_cradmin/devilry_listfilter/assignment.py:63
 #: devilry/devilry_header/templates/devilry_header/about_me.django.html:20
 #: devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/projectgroup_overview.django.html:70
 msgid "Name"
@@ -380,86 +380,71 @@
 #: devilry/apps/core/models/delivery.py:156
 #: devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/groupdetails.django.html:52
 #: devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/feedbackset_info_item_value.django.html:14
 #: devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_details.django.html:89
 msgid "Deadline"
 msgstr ""
 
-#: devilry/apps/core/models/groupinvite.py:146
+#: devilry/apps/core/models/groupinvite.py:148
 msgid "The selected student is not eligible to join the group."
 msgstr ""
 
-#: devilry/apps/core/models/groupinvite.py:152
+#: devilry/apps/core/models/groupinvite.py:154
 msgid "The user sending an invite must be a Candiate on the group."
 msgstr ""
 
-#: devilry/apps/core/models/groupinvite.py:154
+#: devilry/apps/core/models/groupinvite.py:156
 msgid "The student is already a member of the group."
 msgstr ""
 
-#: devilry/apps/core/models/groupinvite.py:159
+#: devilry/apps/core/models/groupinvite.py:161
 msgid ""
 "The student is already invited to join the group, but they have not "
 "responded yet."
 msgstr ""
 
-#: devilry/apps/core/models/groupinvite.py:166
+#: devilry/apps/core/models/groupinvite.py:168
 #: devilry/devilry_student/views/group/projectgroupapp.py:281
 msgid ""
 "Creating project groups without administrator approval is not allowed on "
 "this assignment anymore. Please contact you course administrator if you "
 "think this is wrong."
 msgstr ""
 
-#: devilry/apps/core/models/groupinvite.py:171
+#: devilry/apps/core/models/groupinvite.py:173
 #: devilry/devilry_student/views/group/projectgroupapp.py:286
 msgid ""
 "This assignment does not allow students to form project groups on their own."
 msgstr ""
 
-#: devilry/apps/core/models/groupinvite.py:174
+#: devilry/apps/core/models/groupinvite.py:176
 msgid "The invited student is not registered on this assignment."
 msgstr ""
 
-#: devilry/apps/core/models/groupinvite.py:182
+#: devilry/apps/core/models/groupinvite.py:184
 msgid ""
 "The invited student is already in a project group with more than 1 students."
 msgstr ""
 
-#: devilry/apps/core/models/groupinvite.py:198
+#: devilry/apps/core/models/groupinvite.py:200
 msgid "This invite has already been accepted."
 msgstr ""
 
-#: devilry/apps/core/models/groupinvite.py:200
+#: devilry/apps/core/models/groupinvite.py:202
 msgid "This invite has already been declined."
 msgstr ""
 
-#: devilry/apps/core/models/groupinvite.py:222
-#, python-brace-format
-msgid "{user} accepted your project group invite"
-msgstr ""
-
-#: devilry/apps/core/models/groupinvite.py:225
-#, python-brace-format
-msgid "{user} rejected your project group invite"
-msgstr ""
-
 #: devilry/apps/core/models/groupinvite.py:251
 msgid "Can not send notification for an accepted GroupInvite."
 msgstr ""
 
 #: devilry/apps/core/models/groupinvite.py:253
 msgid "Can not send notification for an unsaved GroupInvite."
 msgstr ""
 
-#: devilry/apps/core/models/groupinvite.py:256
-#, python-brace-format
-msgid "Project group invite for {assignment}"
-msgstr ""
-
 #: devilry/apps/core/models/period.py:190
 msgid "semester"
 msgstr ""
 
 #: devilry/apps/core/models/period.py:191
 msgid "semesters"
 msgstr ""
@@ -522,36 +507,14 @@
 msgstr ""
 
 #: devilry/apps/core/models/subject.py:123
 #: devilry/devilry_admin/views/dashboard/overview.py:61
 msgid "courses"
 msgstr ""
 
-#: devilry/apps/core/templates/devilry_core/groupinvite_accepted.django.txt:1
-#, python-format
-msgid ""
-"%(sent_to_displayname)s accepted the invite to join your project\n"
-"group for %(subject)s %(assignment)s"
-msgstr ""
-
-#: devilry/apps/core/templates/devilry_core/groupinvite_invite.django.txt:1
-#, python-format
-msgid ""
-"%(sent_by_displayname)s invited you to join their project\n"
-"group for %(subject)s %(assignment)s.\n"
-"Accept or reject the offer here:"
-msgstr ""
-
-#: devilry/apps/core/templates/devilry_core/groupinvite_rejected.django.txt:1
-#, python-format
-msgid ""
-"%(sent_to_displayname)s rejected the invite to join your project\n"
-"group for %(subject)s %(assignment)s"
-msgstr ""
-
 #: devilry/apps/core/templates/devilry_core/templatetags/comment-summary.django.html:6
 #, python-format
 msgid "%(commentcount)s comment from student."
 msgstr ""
 
 #: devilry/apps/core/templates/devilry_core/templatetags/comment-summary.django.html:10
 #, python-format
@@ -660,287 +623,287 @@
 #: devilry/devilry_account/admin.py:27
 msgid ""
 "Raw passwords are not stored, so there is no way to see this user's "
 "password, but you can change the password using <a href=\"password/\">this "
 "form</a>."
 msgstr ""
 
-#: devilry/devilry_account/admin.py:209 devilry/devilry_account/models.py:470
+#: devilry/devilry_account/admin.py:209 devilry/devilry_account/models.py:478
 msgid "Users"
 msgstr ""
 
 #: devilry/devilry_account/apps.py:7
 msgid "Devilry account"
 msgstr ""
 
 #: devilry/devilry_account/cradminextensions/devilry_crmenu_account.py:10
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:17
 msgid "Account"
 msgstr ""
 
-#: devilry/devilry_account/models.py:413
+#: devilry/devilry_account/models.py:421
 msgid "superuser status"
 msgstr ""
 
-#: devilry/devilry_account/models.py:415
+#: devilry/devilry_account/models.py:423
 msgid ""
 "Designates that this user has all permissions without explicitly assigning "
 "them."
 msgstr ""
 
-#: devilry/devilry_account/models.py:427
+#: devilry/devilry_account/models.py:435
 msgid ""
 "The short name for the user. This is set automatically to the email or "
 "username depending on the method used for authentication."
 msgstr ""
 
-#: devilry/devilry_account/models.py:433
+#: devilry/devilry_account/models.py:441
 msgid "Full name"
 msgstr ""
 
-#: devilry/devilry_account/models.py:439
+#: devilry/devilry_account/models.py:447
 #: devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py:34
 msgid "Last name"
 msgstr ""
 
-#: devilry/devilry_account/models.py:444
+#: devilry/devilry_account/models.py:452
 msgid "date joined"
 msgstr ""
 
-#: devilry/devilry_account/models.py:450
+#: devilry/devilry_account/models.py:458
 msgid "Suspension time"
 msgstr ""
 
-#: devilry/devilry_account/models.py:451
+#: devilry/devilry_account/models.py:459
 msgid "Time when the account was suspended"
 msgstr ""
 
-#: devilry/devilry_account/models.py:456
+#: devilry/devilry_account/models.py:464
 msgid "Reason for suspension"
 msgstr ""
 
-#: devilry/devilry_account/models.py:462
+#: devilry/devilry_account/models.py:470
 msgid "Preferred language"
 msgstr ""
 
-#: devilry/devilry_account/models.py:469
+#: devilry/devilry_account/models.py:477
 msgid "User"
 msgstr ""
 
-#: devilry/devilry_account/models.py:533
+#: devilry/devilry_account/models.py:541
 msgid "Can not provide a reason for suspension when suspension time is blank."
 msgstr ""
 
-#: devilry/devilry_account/models.py:535
+#: devilry/devilry_account/models.py:543
 msgid "Short name is required."
 msgstr ""
 
-#: devilry/devilry_account/models.py:683
+#: devilry/devilry_account/models.py:691
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:70
 msgid "Email address"
 msgstr ""
 
-#: devilry/devilry_account/models.py:684
+#: devilry/devilry_account/models.py:692
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:68
 msgid "Email addresses"
 msgstr ""
 
-#: devilry/devilry_account/models.py:692
+#: devilry/devilry_account/models.py:700
 #: devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py:14
 msgid "Email"
 msgstr ""
 
-#: devilry/devilry_account/models.py:700
+#: devilry/devilry_account/models.py:708
 msgid "Send notifications to this email address?"
 msgstr ""
 
-#: devilry/devilry_account/models.py:707
+#: devilry/devilry_account/models.py:715
 msgid "Is this your primary email?"
 msgstr ""
 
-#: devilry/devilry_account/models.py:709 devilry/devilry_account/models.py:768
+#: devilry/devilry_account/models.py:717 devilry/devilry_account/models.py:776
 #: devilry/devilry_student/cradminextensions/columntypes.py:79
 msgid "No"
 msgstr ""
 
-#: devilry/devilry_account/models.py:710 devilry/devilry_account/models.py:769
+#: devilry/devilry_account/models.py:718 devilry/devilry_account/models.py:777
 #: devilry/devilry_student/cradminextensions/columntypes.py:78
 msgid "Yes"
 msgstr ""
 
-#: devilry/devilry_account/models.py:712
+#: devilry/devilry_account/models.py:720
 msgid ""
 "Your primary email is the email address used when we need to display a "
 "single email address."
 msgstr ""
 
-#: devilry/devilry_account/models.py:732
+#: devilry/devilry_account/models.py:740
 #, python-format
 msgid "%(email)s - User%(userid)s#%(userhortname)s"
 msgstr ""
 
-#: devilry/devilry_account/models.py:748 devilry/devilry_account/models.py:757
+#: devilry/devilry_account/models.py:756 devilry/devilry_account/models.py:765
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:54
 #: devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py:17
 #: devilry/devilry_header/templates/devilry_header/about_me.django.html:29
 msgid "Username"
 msgstr ""
 
-#: devilry/devilry_account/models.py:749
+#: devilry/devilry_account/models.py:757
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:52
 msgid "Usernames"
 msgstr ""
 
-#: devilry/devilry_account/models.py:766
+#: devilry/devilry_account/models.py:774
 msgid "Is this your primary username?"
 msgstr ""
 
-#: devilry/devilry_account/models.py:771
+#: devilry/devilry_account/models.py:779
 msgid ""
 "Your primary username is shown alongside your full name to identify you to "
 "teachers, examiners and other students."
 msgstr ""
 
-#: devilry/devilry_account/models.py:794
+#: devilry/devilry_account/models.py:802
 #, python-format
 msgid "%(username)s - User%(userid)s"
 msgstr ""
 
-#: devilry/devilry_account/models.py:807
+#: devilry/devilry_account/models.py:815
 msgid "Permission group user"
 msgstr ""
 
-#: devilry/devilry_account/models.py:808
+#: devilry/devilry_account/models.py:816
 msgid "Permission group users"
 msgstr ""
 
-#: devilry/devilry_account/models.py:820
+#: devilry/devilry_account/models.py:828
 #, python-format
 msgid "%(user)s in group %(permissiongroup)s"
 msgstr ""
 
-#: devilry/devilry_account/models.py:913
+#: devilry/devilry_account/models.py:921
 msgid "Department administrator group"
 msgstr ""
 
-#: devilry/devilry_account/models.py:914
+#: devilry/devilry_account/models.py:922
 msgid "Course administrator group"
 msgstr ""
 
-#: devilry/devilry_account/models.py:915
+#: devilry/devilry_account/models.py:923
 msgid "Semester administrator group"
 msgstr ""
 
-#: devilry/devilry_account/models.py:919 devilry/devilry_account/models.py:920
+#: devilry/devilry_account/models.py:927 devilry/devilry_account/models.py:928
 msgid "Permission group"
 msgstr ""
 
-#: devilry/devilry_account/models.py:927
+#: devilry/devilry_account/models.py:935
 msgid "A unique name for this group."
 msgstr ""
 
-#: devilry/devilry_account/models.py:933
+#: devilry/devilry_account/models.py:941
 msgid "Created time"
 msgstr ""
 
-#: devilry/devilry_account/models.py:934
+#: devilry/devilry_account/models.py:942
 msgid "The time when this group was created."
 msgstr ""
 
-#: devilry/devilry_account/models.py:940
+#: devilry/devilry_account/models.py:948
 msgid "Last updated time"
 msgstr ""
 
-#: devilry/devilry_account/models.py:941
+#: devilry/devilry_account/models.py:949
 msgid "The time when this group last updated."
 msgstr ""
 
-#: devilry/devilry_account/models.py:947
+#: devilry/devilry_account/models.py:955
 msgid "Last updated from syncsystem time"
 msgstr ""
 
-#: devilry/devilry_account/models.py:948
+#: devilry/devilry_account/models.py:956
 msgid "The time when this group last updated from a third party sync system."
 msgstr ""
 
-#: devilry/devilry_account/models.py:959
+#: devilry/devilry_account/models.py:967
 msgid "Permission group type"
 msgstr ""
 
-#: devilry/devilry_account/models.py:960
+#: devilry/devilry_account/models.py:968
 msgid ""
 "Course and semester administrator groups can only be assigned to a single "
 "course or semester. Department administrator groups can be assigned to "
 "multiple courses. You can not change this for existing permission groups."
 msgstr ""
 
-#: devilry/devilry_account/models.py:976
+#: devilry/devilry_account/models.py:984
 msgid "Custom manageable?"
 msgstr ""
 
-#: devilry/devilry_account/models.py:977
+#: devilry/devilry_account/models.py:985
 msgid ""
 "Is this group mageable by non-superusers. Can not be enabled for department "
 "administrator groups."
 msgstr ""
 
-#: devilry/devilry_account/models.py:985
+#: devilry/devilry_account/models.py:993
 msgid "Users in this group"
 msgstr ""
 
-#: devilry/devilry_account/models.py:996
+#: devilry/devilry_account/models.py:1004
 msgid "Department administrator groups can not be custom manageable."
 msgstr ""
 
-#: devilry/devilry_account/models.py:1001
+#: devilry/devilry_account/models.py:1009
 msgid "Permission group type can not be changed."
 msgstr ""
 
-#: devilry/devilry_account/models.py:1092
+#: devilry/devilry_account/models.py:1100
 msgid "Semester permission group"
 msgstr ""
 
-#: devilry/devilry_account/models.py:1093
+#: devilry/devilry_account/models.py:1101
 msgid "Semester permission groups"
 msgstr ""
 
-#: devilry/devilry_account/models.py:1106
+#: devilry/devilry_account/models.py:1114
 #, python-format
 msgid "Semester administrators for %(period)s"
 msgstr ""
 
-#: devilry/devilry_account/models.py:1115
+#: devilry/devilry_account/models.py:1123
 msgid ""
 "Only semesters can be added to semester administrator permission groups."
 msgstr ""
 
-#: devilry/devilry_account/models.py:1122
+#: devilry/devilry_account/models.py:1130
 msgid "Only a single editable permission group is allowed for a semester."
 msgstr ""
 
-#: devilry/devilry_account/models.py:1244
+#: devilry/devilry_account/models.py:1252
 msgid "Course permission group"
 msgstr ""
 
-#: devilry/devilry_account/models.py:1245
+#: devilry/devilry_account/models.py:1253
 msgid "Course permission groups"
 msgstr ""
 
-#: devilry/devilry_account/models.py:1258
+#: devilry/devilry_account/models.py:1266
 #, python-format
 msgid "Course administrators for %(subject)s"
 msgstr ""
 
-#: devilry/devilry_account/models.py:1268
+#: devilry/devilry_account/models.py:1276
 msgid ""
 "Courses can only be added to course and department administrator permission "
 "groups."
 msgstr ""
 
-#: devilry/devilry_account/models.py:1276
+#: devilry/devilry_account/models.py:1284
 msgid "Only a single editable permission group is allowed for a course."
 msgstr ""
 
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:21
 msgid "Account overview"
 msgstr ""
 
@@ -3908,16 +3871,16 @@
 
 #: devilry/devilry_admin/views/period/createassignment.py:50
 msgid "Type the name of your assignment."
 msgstr ""
 
 #: devilry/devilry_admin/views/period/createassignment.py:52
 msgid ""
-"Up to 20 letters of lowercase english letters (a-z), numbers, underscore (\"_"
-"\") and hyphen (\"-\")."
+"Up to 20 letters of lowercase english letters (a-z), numbers, underscore "
+"(\"_\") and hyphen (\"-\")."
 msgstr ""
 
 #: devilry/devilry_admin/views/period/createassignment.py:56
 #: devilry/devilry_admin/views/period/createassignment.py:319
 msgid ""
 "Choose how you would like to set up students for the new assignment. You can "
 "add all students from the semester, no students or copy students and "
@@ -4591,16 +4554,16 @@
 
 #: devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html:265
 msgid "Switching diff styles does not work in markdown preview window/tab."
 msgstr ""
 
 #: devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html:273
 msgid ""
-"You can add latex math using the <code>$math$ $/math$</code> or <code>"
-"$mathblock$ $/mathblock$</code> tags."
+"You can add latex math using the <code>$math$ $/math$</code> or "
+"<code>$mathblock$ $/mathblock$</code> tags."
 msgstr ""
 
 #: devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html:297
 msgid ""
 "Make an unordered list by preceding one or more lines of text with * symbol."
 msgstr ""
 
@@ -5216,14 +5179,32 @@
 msgstr ""
 
 #: devilry/devilry_email/feedback_email/feedback_email.py:24
 #, python-format
 msgid "Feedback updated for %(assignment_name)s"
 msgstr ""
 
+#: devilry/devilry_email/groupinvite_email/groupinvite_email.py:52
+#, python-brace-format
+msgctxt "group invite"
+msgid "{user} accepted your project group invite"
+msgstr ""
+
+#: devilry/devilry_email/groupinvite_email/groupinvite_email.py:90
+#, python-brace-format
+msgctxt "group invite"
+msgid "{user} rejected your project group invite"
+msgstr ""
+
+#: devilry/devilry_email/groupinvite_email/groupinvite_email.py:128
+#, python-brace-format
+msgctxt "group invite"
+msgid "Project group invite for {assignment}"
+msgstr ""
+
 #: devilry/devilry_email/templates/devilry_email/comment_email/comment.txt:4
 msgctxt "devilry comment email"
 msgid "Assignment"
 msgstr ""
 
 #: devilry/devilry_email/templates/devilry_email/comment_email/comment.txt:6
 msgctxt "devilry comment email"
@@ -5296,14 +5277,38 @@
 msgstr ""
 
 #: devilry/devilry_email/templates/devilry_email/feedback_email/assignment_feedback_student.txt:30
 msgctxt "devilry email feedback"
 msgid "See the delivery feed for more details"
 msgstr ""
 
+#: devilry/devilry_email/templates/devilry_email/groupinvite_email/accepted.txt:3
+#, python-format
+msgctxt "group invite"
+msgid ""
+"%(sent_to_displayname)s accepted the invite to join your project group for "
+"%(subject)s %(assignment)s"
+msgstr ""
+
+#: devilry/devilry_email/templates/devilry_email/groupinvite_email/invite.txt:3
+#, python-format
+msgctxt "group invite"
+msgid ""
+"%(sent_by_displayname)s invited you to join their project group for "
+"%(subject)s %(assignment)s. Accept or reject the offer here:"
+msgstr ""
+
+#: devilry/devilry_email/templates/devilry_email/groupinvite_email/rejected.txt:3
+#, python-format
+msgctxt "group invite"
+msgid ""
+"%(sent_to_displayname)s rejected the invite to join your project group for "
+"%(subject)s %(assignment)s"
+msgstr ""
+
 #: devilry/devilry_examiner/cradminextensions/devilry_crmenu_examiner.py:15
 msgctxt "breadcrumb"
 msgid "Examiner"
 msgstr ""
 
 #: devilry/devilry_examiner/templates/devilry_examiner/assignment/grouplist.django.html:17
 msgid "Bulk feedback"
@@ -5331,15 +5336,15 @@
 #: devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html:4
 #: devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html:11
 msgid "Passed"
 msgstr ""
 
 #: devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/grade_cell_value.django.html:9
 #: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:47
-#: devilry/devilry_message/models/base.py:353
+#: devilry/devilry_message/models/base.py:358
 #: devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html:6
 #: devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html:13
 msgid "Failed"
 msgstr ""
 
 #: devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/simple_group_bulk_feedbackview.django.html:27
 msgid ""
@@ -5437,21 +5442,21 @@
 msgstr ""
 
 #: devilry/devilry_examiner/templatetags/devilry_examiner_tags.py:57
 msgid "Show feedback"
 msgstr ""
 
 #: devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py:52
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:359
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:358
 msgctxt "grading"
 msgid "Passed?"
 msgstr ""
 
 #: devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py:53
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:360
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:359
 msgctxt "grading"
 msgid "Check to provide a passing grade."
 msgstr ""
 
 #: devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py:97
 msgid "Bulk create feedback"
 msgstr ""
@@ -5462,16 +5467,16 @@
 msgstr ""
 
 #: devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py:90
 msgid "Students in groups"
 msgstr ""
 
 #: devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py:91
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:341
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:364
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:340
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:363
 msgid "Grading"
 msgstr ""
 
 #: devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py:92
 msgid "Comment text"
 msgstr ""
 
@@ -6155,15 +6160,15 @@
 
 #: devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html:16
 msgid "Back to feed"
 msgstr ""
 
 #: devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html:21
 #: devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/feedbackset_info_item_value.django.html:67
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:396
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:395
 msgid "Edit grade"
 msgstr ""
 
 #: devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html:29
 msgid "Current result"
 msgstr ""
 
@@ -6434,15 +6439,15 @@
 msgstr ""
 
 #: devilry/devilry_group/templatetags/devilry_group_tags.py:73
 msgid "tenth"
 msgstr ""
 
 #: devilry/devilry_group/views/admin/feedbackfeed_admin.py:114
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:300
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:299
 msgid "Add note"
 msgstr ""
 
 #: devilry/devilry_group/views/cradmin_comment_history.py:26
 msgctxt "comment edit history item"
 msgid "Only visible to you"
 msgstr ""
@@ -6462,116 +6467,116 @@
 msgid "Comment edit history"
 msgstr ""
 
 #: devilry/devilry_group/views/cradmin_comment_history.py:62
 msgid "No items"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:80
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:90
 msgid ""
 "A comment must have either text or a file attached, or both. An empty "
 "comment is not allowed."
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:98
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:108
 msgid "Post comment"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:414
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:425
 msgid "Upload files by dragging and dropping them here"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:417
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:428
 msgid "... or select files"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:420
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:431
 msgid "Select files for upload"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:423
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:434
 msgid "Files queued for upload:"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:426
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:437
 msgid ""
 "You can browse the upload queue and check upload status further down on the "
 "page."
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:429
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:440
 msgid "Invalid filetype"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:431
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:442
 msgctxt "devilry_fileupload"
 msgid "Uploading"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:432
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:443
 msgctxt "devilry_fileupload"
 msgid "Uploaded"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:433
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:444
 msgctxt "devilry_fileupload"
 msgid "Failed"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:434
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:445
 msgctxt "devilry_fileupload"
 msgid "Deleting"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:435
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:446
 msgctxt "devilry_fileupload"
 msgid "Delete failed, try again"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:436
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:447
 msgctxt "devilry_fileupload"
 msgid "Upload status:"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:437
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:448
 msgctxt "devilry_fileupload"
 msgid "Dismiss/close error message"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:438
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:449
 msgctxt "devilry_fileupload"
 msgid "Remove file"
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:440
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:451
 #, python-format
 msgid ""
 "Filename is too long. Please use file names shorter than "
 "%(max_filename_length)s characters."
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:444
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:455
 msgid ""
 "Server timeout while uploading the file. This may be caused by a poor upload "
 "link and/or a too large file."
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:447
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:458
 msgid ""
 "Unknown error. May be a server glitch or a bug. Please try again, and report "
 "the error if it happens multiple times."
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:450
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:461
 msgid ""
 "We could not delete the file. This may be a server glitch or bug. Please try "
 "again, and report if the error happens multiple times."
 msgstr ""
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:563
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:574
 msgid "Comment added!"
 msgstr ""
 
 #: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:49
 msgctxt "grading"
 msgid "Grade"
 msgstr ""
@@ -6595,25 +6600,25 @@
 msgid "Publish feedback"
 msgstr ""
 
 #: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:228
 msgid "Feedback is already published!"
 msgstr ""
 
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:344
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:343
 msgid ""
 "Give a score between {} to {} where {} is the minimum amount of points "
 "needed to pass."
 msgstr ""
 
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:365
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:364
 msgid "Check the box to give a passing grade"
 msgstr ""
 
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:494
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:493
 msgid "Groupcomment"
 msgstr ""
 
 #: devilry/devilry_group/views/group_comment_edit_base.py:55
 #: devilry/devilry_group/views/group_comment_edit_base.py:58
 msgid "Edit comment"
 msgstr ""
@@ -6716,24 +6721,24 @@
 msgstr ""
 
 #: devilry/devilry_message/models/base.py:78
 msgid "Sending"
 msgstr ""
 
 #: devilry/devilry_message/models/base.py:80
-#: devilry/devilry_message/models/base.py:355
+#: devilry/devilry_message/models/base.py:360
 msgid "Error"
 msgstr ""
 
 #: devilry/devilry_message/models/base.py:82
-#: devilry/devilry_message/models/base.py:357
+#: devilry/devilry_message/models/base.py:362
 msgid "Sent"
 msgstr ""
 
-#: devilry/devilry_message/models/base.py:351
+#: devilry/devilry_message/models/base.py:356
 msgid "Not sent"
 msgstr ""
 
 #: devilry/devilry_qualifiesforexam/models.py:93
 msgid "Ready for export"
 msgstr ""
```

### Comparing `devilry-6.0.0rc1/devilry/locale/en/LC_MESSAGES/djangojs.po` & `devilry-6.0.0rc2/devilry/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/locale/nb/LC_MESSAGES/django.mo` & `devilry-6.0.0rc2/devilry/locale/nb/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Devilry\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2022-06-07 08:38+0200\n"
+"PO-Revision-Date: 2023-07-19 13:23+0200\n"
 "Last-Translator: Espen Angell Kristiansen <espen@appresso.no>\n"
 "Language-Team: Norwegian Bokmål (http://www.transifex.com/projects/p/devilry/"
 "language/nb/)\n"
 "Language: nb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 3.0.1\n"
+"X-Generator: Poedit 3.2\n"
 
 msgid ""
 "\n"
 "            Add tags to the semester\n"
 "        "
 msgstr ""
 "\n"
@@ -122,37 +122,14 @@
 
 msgid "%(percent)s%% Complete"
 msgstr "%(percent)s%% Ferdig"
 
 msgid "%(sent_by)s invited you to join their group."
 msgstr "%(sent_by)s inviterte deg til å bli med i deres gruppe."
 
-msgid ""
-"%(sent_by_displayname)s invited you to join their project\n"
-"group for %(subject)s %(assignment)s.\n"
-"Accept or reject the offer here:"
-msgstr ""
-"%(sent_by_displayname)s har invitert deg til sin prosjektgruppe\n"
-"for %(subject)s %(assignment)s.\n"
-"Godta eller avslå tilbudet her:"
-
-msgid ""
-"%(sent_to_displayname)s accepted the invite to join your project\n"
-"group for %(subject)s %(assignment)s"
-msgstr ""
-"%(sent_to_displayname)s godtok invitasjonen til din prosjektgruppe\n"
-"for %(subject)s %(assignment)s"
-
-msgid ""
-"%(sent_to_displayname)s rejected the invite to join your project\n"
-"group for %(subject)s %(assignment)s"
-msgstr ""
-"%(sent_to_displayname)s avslo invitasjonen til din prosjektgruppe\n"
-"for %(subject)s %(assignment)s"
-
 msgid "%(studentcount)s student"
 msgid_plural "%(studentcount)s students"
 msgstr[0] "%(studentcount)s student"
 msgstr[1] "%(studentcount)s studenter"
 
 msgid "%(studentcount)s students in %(groupcount)s project group"
 msgid_plural "%(studentcount)s students in %(groupcount)s project groups"
@@ -2461,17 +2438,14 @@
 
 msgid "Project group"
 msgstr "Prosjektgruppe"
 
 msgid "Project group details"
 msgstr "Detaljer om prosjektgruppe"
 
-msgid "Project group invite for {assignment}"
-msgstr "Invitasjon til prosjektgruppe for {assignment}"
-
 msgid "Project group members"
 msgstr "Prosjektgruppemedlemmer"
 
 msgid "Project groups"
 msgstr "Prosjektgrupper"
 
 msgid "Provide a message as to why the Status needs to be retracted."
@@ -3213,15 +3187,15 @@
 "deadlines, adding deliveries after the deadline is prohibited."
 msgstr ""
 "Innleveringsfristen har utgått. Siden dette kurset har harde frister, er det "
 "ikke lov til å legge til innleveringer etter innleveringsfristen."
 
 msgid ""
 "The download will start automatically as soon as the report is finished."
-msgstr "Nedlastingen vil starte så for rapporten er ferdig."
+msgstr "Nedlastingen vil starte så fort rapporten er ferdig."
 
 msgid ""
 "The feedback progress in percentages. How many of the groups has been given "
 "the grade passed/failed or have not been corrected yet."
 msgstr ""
 "Fremgang i prosenter. Hvor stor andel av gruppene fått karakteren bestått/"
 "ikke-bestått, eller har ikke blitt rettet enda."
@@ -3491,15 +3465,15 @@
 msgid "This assignment is open for deliveries."
 msgstr "Denne oppgaven er åpen for innleveringer."
 
 msgid ""
 "This assignment uses hard deadlines. Students will not be able to write "
 "comments or upload files after the deadline has expired."
 msgstr ""
-"Denne oppdaven bruker harde frister. Studenter vil ikke kunne skrive "
+"Denne oppgaven bruker harde frister. Studenter vil ikke kunne skrive "
 "kommentarer eller laste opp innleveringer etter fristen."
 
 msgid ""
 "This assignment uses hard deadlines. You will not be able to write comments "
 "or upload files after the deadline has expired."
 msgstr ""
 "Denne oppgaven bruker harde frister. Du vil ikke kunne skrive kommentarer "
@@ -5460,14 +5434,51 @@
 msgid "Grade"
 msgstr "Karakter"
 
 msgctxt "group in active semester filter"
 msgid "Active semesters?"
 msgstr "Aktive semestre?"
 
+msgctxt "group invite"
+msgid ""
+"%(sent_by_displayname)s invited you to join their project group for "
+"%(subject)s %(assignment)s. Accept or reject the offer here:"
+msgstr ""
+"%(sent_by_displayname)s har invitert deg til sin prosjektgruppe\n"
+"for %(subject)s %(assignment)s.\n"
+"Godta eller avslå tilbudet her:"
+
+msgctxt "group invite"
+msgid ""
+"%(sent_to_displayname)s accepted the invite to join your project group for "
+"%(subject)s %(assignment)s"
+msgstr ""
+"%(sent_to_displayname)s aksepterte invitasjonen til din prosjektgruppe for "
+"%(subject)s %(assignment)s"
+
+msgctxt "group invite"
+msgid ""
+"%(sent_to_displayname)s rejected the invite to join your project group for "
+"%(subject)s %(assignment)s"
+msgstr ""
+"%(sent_to_displayname)s avslo invitasjonen til din prosjektgruppe\n"
+"for %(subject)s %(assignment)s"
+
+msgctxt "group invite"
+msgid "Project group invite for {assignment}"
+msgstr "Invitasjon til prosjektgruppe for {assignment}"
+
+msgctxt "group invite"
+msgid "{user} accepted your project group invite"
+msgstr "{user} aksepterte invitasjonen til din prosjektgruppe"
+
+msgctxt "group invite"
+msgid "{user} rejected your project group invite"
+msgstr "{user} avslo invitasjonen til din prosjektgruppe"
+
 msgctxt "group is passing grade filter"
 msgid "Both"
 msgstr "Begge"
 
 msgctxt "group is passing grade filter"
 msgid "Passing grade?"
 msgstr "Ståkarakter?"
@@ -5884,13 +5895,7 @@
 
 msgid ""
 "{grade} occurs multiple times in the map. A grade must be unique within the "
 "map."
 msgstr ""
 "{grade} forekommer flere ganger i tabellen. En karakter må være unik i "
 "tabellen."
-
-msgid "{user} accepted your project group invite"
-msgstr "{user} aksepterte invitasjonen til din prosjektgruppe"
-
-msgid "{user} rejected your project group invite"
-msgstr "{user} avslo invitasjonen til din prosjektgruppe"
```

### Comparing `devilry-6.0.0rc1/devilry/locale/nb/LC_MESSAGES/django.po` & `devilry-6.0.0rc2/devilry/locale/nb/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 # Translators:
 # Espen Angell Kristiansen <espen@appresso.no>, 2015
 # Tone Angell Kristiansen <tone@appresso.no>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: Devilry\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-07 08:34+0200\n"
-"PO-Revision-Date: 2022-06-07 08:38+0200\n"
+"POT-Creation-Date: 2023-07-19 14:06+0200\n"
+"PO-Revision-Date: 2023-07-19 13:23+0200\n"
 "Last-Translator: Espen Angell Kristiansen <espen@appresso.no>\n"
 "Language-Team: Norwegian Bokmål (http://www.transifex.com/projects/p/devilry/"
 "language/nb/)\n"
 "Language: nb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 3.0.1\n"
+"X-Generator: Poedit 3.2\n"
 
 #: devilry/apps/core/admin.py:66
 msgid "Admins"
 msgstr "Admins"
 
 #: devilry/apps/core/admin.py:97 devilry/apps/core/admin.py:125
 #: devilry/apps/core/admin.py:189 devilry/apps/core/models/period.py:196
@@ -362,36 +362,36 @@
 msgid "Closed without feedback"
 msgstr "Lukket uten tilbakemelding"
 
 #: devilry/apps/core/models/assignment_group.py:1009
 msgid "Waiting for something"
 msgstr "Venter på noe"
 
-#: devilry/apps/core/models/assignment_group.py:1215
+#: devilry/apps/core/models/assignment_group.py:1226
 #: devilry/apps/core/templates/devilry_core/templatetags/multiple-candidates-long-displayname.django.html:8
 #: devilry/apps/core/templates/devilry_core/templatetags/multiple-candidates-short-displayname.django.html:8
 msgctxt "core assignmentgroup"
 msgid "no students in group"
 msgstr "ingen studenter i gruppen"
 
-#: devilry/apps/core/models/assignment_group.py:1219
+#: devilry/apps/core/models/assignment_group.py:1230
 #, python-format
 msgctxt "core assignmentgroup"
 msgid "group#%(groupid)s - no students in group"
 msgstr "gruppe#%(groupid)s - ingen studenter i gruppen"
 
-#: devilry/apps/core/models/assignment_group.py:1580
+#: devilry/apps/core/models/assignment_group.py:1591
 msgid ""
 "Cannot merge self into target, self and target is not part of same "
 "AssignmentGroup"
 msgstr ""
 "Kan ikke flette seg selv med målet, seg selv og målet er ikke en del av "
 "samme oppgave gruppe (AssignmentGroup)"
 
-#: devilry/apps/core/models/assignment_group.py:1633
+#: devilry/apps/core/models/assignment_group.py:1644
 msgid "Cannot merge less than 2 groups"
 msgstr "Kan ikke flette mindre enn 2 grupper"
 
 #: devilry/apps/core/models/basenode.py:53
 msgid "Path"
 msgstr "Vei"
 
@@ -403,26 +403,26 @@
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:37
 #: devilry/devilry_admin/views/dashboard/overview.py:107
 msgid "Short name"
 msgstr "Kort navn"
 
 #: devilry/apps/core/models/custom_db_fields.py:22
 msgid ""
-"Up to 20 letters of lowercase english letters (a-z), numbers, underscore (\"_"
-"\") and hyphen (\"-\"). Used when the name takes too much space."
+"Up to 20 letters of lowercase english letters (a-z), numbers, underscore "
+"(\"_\") and hyphen (\"-\"). Used when the name takes too much space."
 msgstr ""
 "Opp til 20 bokstaver med engelske bokstaver (a-z), tall, understrek(\"_\") "
 "og bindestrek(\"-\"). Benyttes når navn tar for mye plass."
 
 #: devilry/apps/core/models/custom_db_fields.py:33
 msgid "Can only contain numbers, lowercase letters, '_' and '-'. "
 msgstr "Kan kun bestå av nummer, små bokstaver, '_' og '-'. "
 
 #: devilry/apps/core/models/custom_db_fields.py:40
-#: devilry/devilry_account/models.py:926
+#: devilry/devilry_account/models.py:934
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:28
 #: devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py:24
 #: devilry/devilry_cradmin/devilry_listfilter/assignment.py:17
 #: devilry/devilry_cradmin/devilry_listfilter/assignment.py:63
 #: devilry/devilry_header/templates/devilry_header/about_me.django.html:20
 #: devilry/devilry_student/templates/devilry_student/cradmin_group/projectgroupapp/projectgroup_overview.django.html:70
 msgid "Name"
@@ -444,92 +444,77 @@
 #: devilry/apps/core/models/delivery.py:156
 #: devilry/devilry_cradmin/templates/devilry_cradmin/devilry_listbuilder/assignmentgroup/include/groupdetails.django.html:52
 #: devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/feedbackset_info_item_value.django.html:14
 #: devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_details.django.html:89
 msgid "Deadline"
 msgstr "Innleveringsfrist"
 
-#: devilry/apps/core/models/groupinvite.py:146
+#: devilry/apps/core/models/groupinvite.py:148
 msgid "The selected student is not eligible to join the group."
 msgstr "Den valgte studenten er ikke kvalifisert til å bli med i gruppen."
 
-#: devilry/apps/core/models/groupinvite.py:152
+#: devilry/apps/core/models/groupinvite.py:154
 msgid "The user sending an invite must be a Candiate on the group."
 msgstr "Brukeren som sender en invitasjon må være en Kandidat for gruppen."
 
-#: devilry/apps/core/models/groupinvite.py:154
+#: devilry/apps/core/models/groupinvite.py:156
 msgid "The student is already a member of the group."
 msgstr "Studenten er allerede medlem av gruppen."
 
-#: devilry/apps/core/models/groupinvite.py:159
+#: devilry/apps/core/models/groupinvite.py:161
 msgid ""
 "The student is already invited to join the group, but they have not "
 "responded yet."
 msgstr ""
 "Studenten har allerede blitt invitert til gruppen, men har ikke svart enda."
 
-#: devilry/apps/core/models/groupinvite.py:166
+#: devilry/apps/core/models/groupinvite.py:168
 #: devilry/devilry_student/views/group/projectgroupapp.py:281
 msgid ""
 "Creating project groups without administrator approval is not allowed on "
 "this assignment anymore. Please contact you course administrator if you "
 "think this is wrong."
 msgstr ""
 "Å lage prosjektgrupper uten godkjenning fra administrator er ikke lenger "
 "mulig på denne oppgaven. Vennligst ta kontakt med din kursadministrator "
 "dersom du tror dette er feil."
 
-#: devilry/apps/core/models/groupinvite.py:171
+#: devilry/apps/core/models/groupinvite.py:173
 #: devilry/devilry_student/views/group/projectgroupapp.py:286
 msgid ""
 "This assignment does not allow students to form project groups on their own."
 msgstr "Denne oppgaven lar ikke studenter lage prosjektgrupper på egenhånd."
 
-#: devilry/apps/core/models/groupinvite.py:174
+#: devilry/apps/core/models/groupinvite.py:176
 msgid "The invited student is not registered on this assignment."
 msgstr "Den inviterte studenten er ikke registrert på denne oppgaven."
 
-#: devilry/apps/core/models/groupinvite.py:182
+#: devilry/apps/core/models/groupinvite.py:184
 msgid ""
 "The invited student is already in a project group with more than 1 students."
 msgstr ""
 "Den inviterte studenten er allerede med i en prosjektgruppe med mer enn 1 "
 "student."
 
-#: devilry/apps/core/models/groupinvite.py:198
+#: devilry/apps/core/models/groupinvite.py:200
 msgid "This invite has already been accepted."
 msgstr "Invitasjonen har tidligere blitt akseptert."
 
-#: devilry/apps/core/models/groupinvite.py:200
+#: devilry/apps/core/models/groupinvite.py:202
 msgid "This invite has already been declined."
 msgstr "Invitasjonen har tidligere blitt avvist."
 
-#: devilry/apps/core/models/groupinvite.py:222
-#, python-brace-format
-msgid "{user} accepted your project group invite"
-msgstr "{user} aksepterte invitasjonen til din prosjektgruppe"
-
-#: devilry/apps/core/models/groupinvite.py:225
-#, python-brace-format
-msgid "{user} rejected your project group invite"
-msgstr "{user} avslo invitasjonen til din prosjektgruppe"
-
 #: devilry/apps/core/models/groupinvite.py:251
 msgid "Can not send notification for an accepted GroupInvite."
 msgstr "Kan ikke send en melding til en akseptert gruppeinvitasjon."
 
 #: devilry/apps/core/models/groupinvite.py:253
 msgid "Can not send notification for an unsaved GroupInvite."
 msgstr "Kan ikke sende en melding til en gruppe invitasjon som ikke er lagret."
 
-#: devilry/apps/core/models/groupinvite.py:256
-#, python-brace-format
-msgid "Project group invite for {assignment}"
-msgstr "Invitasjon til prosjektgruppe for {assignment}"
-
 #: devilry/apps/core/models/period.py:190
 msgid "semester"
 msgstr "semester"
 
 #: devilry/apps/core/models/period.py:191
 msgid "semesters"
 msgstr "semestre"
@@ -598,43 +583,14 @@
 msgstr "kurs"
 
 #: devilry/apps/core/models/subject.py:123
 #: devilry/devilry_admin/views/dashboard/overview.py:61
 msgid "courses"
 msgstr "kurs"
 
-#: devilry/apps/core/templates/devilry_core/groupinvite_accepted.django.txt:1
-#, python-format
-msgid ""
-"%(sent_to_displayname)s accepted the invite to join your project\n"
-"group for %(subject)s %(assignment)s"
-msgstr ""
-"%(sent_to_displayname)s godtok invitasjonen til din prosjektgruppe\n"
-"for %(subject)s %(assignment)s"
-
-#: devilry/apps/core/templates/devilry_core/groupinvite_invite.django.txt:1
-#, python-format
-msgid ""
-"%(sent_by_displayname)s invited you to join their project\n"
-"group for %(subject)s %(assignment)s.\n"
-"Accept or reject the offer here:"
-msgstr ""
-"%(sent_by_displayname)s har invitert deg til sin prosjektgruppe\n"
-"for %(subject)s %(assignment)s.\n"
-"Godta eller avslå tilbudet her:"
-
-#: devilry/apps/core/templates/devilry_core/groupinvite_rejected.django.txt:1
-#, python-format
-msgid ""
-"%(sent_to_displayname)s rejected the invite to join your project\n"
-"group for %(subject)s %(assignment)s"
-msgstr ""
-"%(sent_to_displayname)s avslo invitasjonen til din prosjektgruppe\n"
-"for %(subject)s %(assignment)s"
-
 #: devilry/apps/core/templates/devilry_core/templatetags/comment-summary.django.html:6
 #, python-format
 msgid "%(commentcount)s comment from student."
 msgstr "%(commentcount)s kommentar fra student."
 
 #: devilry/apps/core/templates/devilry_core/templatetags/comment-summary.django.html:10
 #, python-format
@@ -746,307 +702,307 @@
 "password, but you can change the password using <a href=\"password/\">this "
 "form</a>."
 msgstr ""
 "Rå passord lagers ikke, så det er ingen måte å se denne brukerens passord, "
 "men du kan endre passordet ved å gå til <a href=\"password/\">dette "
 "skjemaet</a>."
 
-#: devilry/devilry_account/admin.py:209 devilry/devilry_account/models.py:470
+#: devilry/devilry_account/admin.py:209 devilry/devilry_account/models.py:478
 msgid "Users"
 msgstr "Brukere"
 
 #: devilry/devilry_account/apps.py:7
 msgid "Devilry account"
 msgstr "Devilry konto"
 
 #: devilry/devilry_account/cradminextensions/devilry_crmenu_account.py:10
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:17
 msgid "Account"
 msgstr "Konto"
 
-#: devilry/devilry_account/models.py:413
+#: devilry/devilry_account/models.py:421
 msgid "superuser status"
 msgstr "superbrukerstatus"
 
-#: devilry/devilry_account/models.py:415
+#: devilry/devilry_account/models.py:423
 msgid ""
 "Designates that this user has all permissions without explicitly assigning "
 "them."
 msgstr ""
 "Tilordner alle tillatelser til denne brukeren uten å tilordne tillatelsene "
 "eksplisitt."
 
-#: devilry/devilry_account/models.py:427
+#: devilry/devilry_account/models.py:435
 msgid ""
 "The short name for the user. This is set automatically to the email or "
 "username depending on the method used for authentication."
 msgstr ""
 "Det korte navnet til brukeren. Dette settes automatisk til enten e-post "
 "eller brukernavn, avhengig av autentifikasjonsmetode."
 
-#: devilry/devilry_account/models.py:433
+#: devilry/devilry_account/models.py:441
 msgid "Full name"
 msgstr "Fullt navn"
 
-#: devilry/devilry_account/models.py:439
+#: devilry/devilry_account/models.py:447
 #: devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py:34
 msgid "Last name"
 msgstr "Etternavn"
 
-#: devilry/devilry_account/models.py:444
+#: devilry/devilry_account/models.py:452
 msgid "date joined"
 msgstr "innmeldt dato"
 
-#: devilry/devilry_account/models.py:450
+#: devilry/devilry_account/models.py:458
 msgid "Suspension time"
 msgstr "Suspensasjon tidspunkt"
 
-#: devilry/devilry_account/models.py:451
+#: devilry/devilry_account/models.py:459
 msgid "Time when the account was suspended"
 msgstr "Tidspunkt for når kontoen ble suspendert"
 
-#: devilry/devilry_account/models.py:456
+#: devilry/devilry_account/models.py:464
 msgid "Reason for suspension"
 msgstr "Årsak til suspensjon"
 
-#: devilry/devilry_account/models.py:462
+#: devilry/devilry_account/models.py:470
 msgid "Preferred language"
 msgstr "Foretrukket språk"
 
-#: devilry/devilry_account/models.py:469
+#: devilry/devilry_account/models.py:477
 msgid "User"
 msgstr "Bruker"
 
-#: devilry/devilry_account/models.py:533
+#: devilry/devilry_account/models.py:541
 msgid "Can not provide a reason for suspension when suspension time is blank."
 msgstr ""
 "Kan ikke angi en årsak for suspensjonen når tidspunktet for supensasjonen er "
 "blankt."
 
-#: devilry/devilry_account/models.py:535
+#: devilry/devilry_account/models.py:543
 msgid "Short name is required."
 msgstr "Kort navn er påkrevd."
 
-#: devilry/devilry_account/models.py:683
+#: devilry/devilry_account/models.py:691
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:70
 msgid "Email address"
 msgstr "E-postadresse"
 
-#: devilry/devilry_account/models.py:684
+#: devilry/devilry_account/models.py:692
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:68
 msgid "Email addresses"
 msgstr "E-postadresser"
 
-#: devilry/devilry_account/models.py:692
+#: devilry/devilry_account/models.py:700
 #: devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py:14
 msgid "Email"
 msgstr "Epost"
 
-#: devilry/devilry_account/models.py:700
+#: devilry/devilry_account/models.py:708
 msgid "Send notifications to this email address?"
 msgstr "Send melding til denne e-postadressen?"
 
-#: devilry/devilry_account/models.py:707
+#: devilry/devilry_account/models.py:715
 msgid "Is this your primary email?"
 msgstr "Er dette din primære e-post?"
 
-#: devilry/devilry_account/models.py:709 devilry/devilry_account/models.py:768
+#: devilry/devilry_account/models.py:717 devilry/devilry_account/models.py:776
 #: devilry/devilry_student/cradminextensions/columntypes.py:79
 msgid "No"
 msgstr "Nei"
 
-#: devilry/devilry_account/models.py:710 devilry/devilry_account/models.py:769
+#: devilry/devilry_account/models.py:718 devilry/devilry_account/models.py:777
 #: devilry/devilry_student/cradminextensions/columntypes.py:78
 msgid "Yes"
 msgstr "Ja"
 
-#: devilry/devilry_account/models.py:712
+#: devilry/devilry_account/models.py:720
 msgid ""
 "Your primary email is the email address used when we need to display a "
 "single email address."
 msgstr ""
 "Din primære e-post er e-postadressen som benyttes hvis vi trener å vise en "
 "enkel e-postadresse."
 
-#: devilry/devilry_account/models.py:732
+#: devilry/devilry_account/models.py:740
 #, python-format
 msgid "%(email)s - User%(userid)s#%(userhortname)s"
 msgstr "%(email)s - Bruker%(userid)s#%(userhortname)s"
 
-#: devilry/devilry_account/models.py:748 devilry/devilry_account/models.py:757
+#: devilry/devilry_account/models.py:756 devilry/devilry_account/models.py:765
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:54
 #: devilry/devilry_admin/cradminextensions/listfilter/listfilter_relateduser.py:17
 #: devilry/devilry_header/templates/devilry_header/about_me.django.html:29
 msgid "Username"
 msgstr "Brukernavn"
 
-#: devilry/devilry_account/models.py:749
+#: devilry/devilry_account/models.py:757
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:52
 msgid "Usernames"
 msgstr "Brukernavn"
 
-#: devilry/devilry_account/models.py:766
+#: devilry/devilry_account/models.py:774
 msgid "Is this your primary username?"
 msgstr "Er dette ditt primære brukernavn?"
 
-#: devilry/devilry_account/models.py:771
+#: devilry/devilry_account/models.py:779
 msgid ""
 "Your primary username is shown alongside your full name to identify you to "
 "teachers, examiners and other students."
 msgstr ""
 "Ditt primære brukernavn vises ved siden av ditt fulle navn for å "
 "identifisere deg for lærere, rettere og andre studenter."
 
-#: devilry/devilry_account/models.py:794
+#: devilry/devilry_account/models.py:802
 #, python-format
 msgid "%(username)s - User%(userid)s"
 msgstr "%(username)s - Bruker%(userid)s"
 
-#: devilry/devilry_account/models.py:807
+#: devilry/devilry_account/models.py:815
 msgid "Permission group user"
 msgstr "Tillatelsesgruppe bruker"
 
-#: devilry/devilry_account/models.py:808
+#: devilry/devilry_account/models.py:816
 msgid "Permission group users"
 msgstr "Tillatelsesgruppe brukere"
 
-#: devilry/devilry_account/models.py:820
+#: devilry/devilry_account/models.py:828
 #, python-format
 msgid "%(user)s in group %(permissiongroup)s"
 msgstr "%(user)s i gruppe %(permissiongroup)s"
 
-#: devilry/devilry_account/models.py:913
+#: devilry/devilry_account/models.py:921
 msgid "Department administrator group"
 msgstr "Avdelingadministratorgruppe"
 
-#: devilry/devilry_account/models.py:914
+#: devilry/devilry_account/models.py:922
 msgid "Course administrator group"
 msgstr "Kurseadministratorgruppe"
 
-#: devilry/devilry_account/models.py:915
+#: devilry/devilry_account/models.py:923
 msgid "Semester administrator group"
 msgstr "Semesteradministratorgruppe"
 
-#: devilry/devilry_account/models.py:919 devilry/devilry_account/models.py:920
+#: devilry/devilry_account/models.py:927 devilry/devilry_account/models.py:928
 msgid "Permission group"
 msgstr "Tillatelsesgruppe"
 
-#: devilry/devilry_account/models.py:927
+#: devilry/devilry_account/models.py:935
 msgid "A unique name for this group."
 msgstr "Et unikt navn for den gruppen."
 
-#: devilry/devilry_account/models.py:933
+#: devilry/devilry_account/models.py:941
 msgid "Created time"
 msgstr "Opprettet tidspunkt"
 
-#: devilry/devilry_account/models.py:934
+#: devilry/devilry_account/models.py:942
 msgid "The time when this group was created."
 msgstr "Tidspunktet for når gruppen ble opprettet."
 
-#: devilry/devilry_account/models.py:940
+#: devilry/devilry_account/models.py:948
 msgid "Last updated time"
 msgstr "Tidspunkt for siste oppdatering"
 
-#: devilry/devilry_account/models.py:941
+#: devilry/devilry_account/models.py:949
 msgid "The time when this group last updated."
 msgstr "Tidspunktet for når gruppen sist ble oppdatert."
 
-#: devilry/devilry_account/models.py:947
+#: devilry/devilry_account/models.py:955
 msgid "Last updated from syncsystem time"
 msgstr "Sist oppdater fra synkroniserings-systemet sin tid"
 
-#: devilry/devilry_account/models.py:948
+#: devilry/devilry_account/models.py:956
 msgid "The time when this group last updated from a third party sync system."
 msgstr ""
 "Tidspunktet for når gruppen sist ble oppdatert fra et tredjeparts-"
 "synkroniseringssystem."
 
-#: devilry/devilry_account/models.py:959
+#: devilry/devilry_account/models.py:967
 msgid "Permission group type"
 msgstr "Tillatelsesgruppe type"
 
-#: devilry/devilry_account/models.py:960
+#: devilry/devilry_account/models.py:968
 msgid ""
 "Course and semester administrator groups can only be assigned to a single "
 "course or semester. Department administrator groups can be assigned to "
 "multiple courses. You can not change this for existing permission groups."
 msgstr ""
 "Grupper av kurs- og semesteradministratorer kan bare tildeles til ett enkelt "
 "kurs eller semester. Grupper av avdelingsadministratorer kan tildeles flere "
 "kurs. Du kan ikke endre dette for eksisterende tillatelsesgrupper."
 
-#: devilry/devilry_account/models.py:976
+#: devilry/devilry_account/models.py:984
 msgid "Custom manageable?"
 msgstr "Tilpasset redigering?"
 
-#: devilry/devilry_account/models.py:977
+#: devilry/devilry_account/models.py:985
 msgid ""
 "Is this group mageable by non-superusers. Can not be enabled for department "
 "administrator groups."
 msgstr ""
 "Er denne gruppen administrert av ikke-superbrukere? Kan ikke aktiveres for "
 "grupper av avdelingsadministratorer."
 
-#: devilry/devilry_account/models.py:985
+#: devilry/devilry_account/models.py:993
 msgid "Users in this group"
 msgstr "Brukere i denne gruppen"
 
-#: devilry/devilry_account/models.py:996
+#: devilry/devilry_account/models.py:1004
 msgid "Department administrator groups can not be custom manageable."
 msgstr "Administratorgrupper for avdeling kan ikke tilpasses ytterlig."
 
-#: devilry/devilry_account/models.py:1001
+#: devilry/devilry_account/models.py:1009
 msgid "Permission group type can not be changed."
 msgstr "Type tilgangsgruppe kan ikke endres."
 
-#: devilry/devilry_account/models.py:1092
+#: devilry/devilry_account/models.py:1100
 msgid "Semester permission group"
 msgstr "Tillatelsesgruppe for semester"
 
-#: devilry/devilry_account/models.py:1093
+#: devilry/devilry_account/models.py:1101
 msgid "Semester permission groups"
 msgstr "Tillatelsesgrupper for semester"
 
-#: devilry/devilry_account/models.py:1106
+#: devilry/devilry_account/models.py:1114
 #, python-format
 msgid "Semester administrators for %(period)s"
 msgstr "Semesteradministratorer for %(period)s"
 
-#: devilry/devilry_account/models.py:1115
+#: devilry/devilry_account/models.py:1123
 msgid ""
 "Only semesters can be added to semester administrator permission groups."
 msgstr ""
 "Kun semestre kan legges til i tillatelsesgruppen for semesteradministratorer."
 
-#: devilry/devilry_account/models.py:1122
+#: devilry/devilry_account/models.py:1130
 msgid "Only a single editable permission group is allowed for a semester."
 msgstr "Kun en redigerbar tillatelsesgruppe er tillat for et semster."
 
-#: devilry/devilry_account/models.py:1244
+#: devilry/devilry_account/models.py:1252
 msgid "Course permission group"
 msgstr "Tillatelsesgruppe for kurs"
 
-#: devilry/devilry_account/models.py:1245
+#: devilry/devilry_account/models.py:1253
 msgid "Course permission groups"
 msgstr "Tillatelsesgruppe for kurs"
 
-#: devilry/devilry_account/models.py:1258
+#: devilry/devilry_account/models.py:1266
 #, python-format
 msgid "Course administrators for %(subject)s"
 msgstr "Kursadministratorer for %(subject)s"
 
-#: devilry/devilry_account/models.py:1268
+#: devilry/devilry_account/models.py:1276
 msgid ""
 "Courses can only be added to course and department administrator permission "
 "groups."
 msgstr ""
 "Kurs kan kun bli lagt til kurs og tillatelsesgrupper for "
 "avdelingsadministrator."
 
-#: devilry/devilry_account/models.py:1276
+#: devilry/devilry_account/models.py:1284
 msgid "Only a single editable permission group is allowed for a course."
 msgstr "Kun en redigerbar tillatelsesgruppe er tillat for et kurs."
 
 #: devilry/devilry_account/templates/devilry_account/crapps/account/index.django.html:21
 msgid "Account overview"
 msgstr "Kontooversikt"
 
@@ -3411,16 +3367,16 @@
 #: devilry/devilry_admin/views/assignment/deadline_handling.py:87
 #, python-format
 msgctxt "assignment config"
 msgid ""
 "Changed deadline handling from \"%(old_deadline_handling_text)s\" to "
 "\"%(new_deadline_handling_text)s\"."
 msgstr ""
-"Endret håndtering av innleveringsfrist fra \"%(old_deadline_handling_text)s"
-"\" til \"%(new_deadline_handling_text)s\"."
+"Endret håndtering av innleveringsfrist fra "
+"\"%(old_deadline_handling_text)s\" til \"%(new_deadline_handling_text)s\"."
 
 #: devilry/devilry_admin/views/assignment/examiner_selfassign.py:16
 msgctxt "admin examiner selfassign setting"
 msgid "Edit examiner self-assign"
 msgstr "Rediger selv-tilordning for rettere"
 
 #: devilry/devilry_admin/views/assignment/examiner_selfassign.py:42
@@ -4328,16 +4284,16 @@
 
 #: devilry/devilry_admin/views/period/createassignment.py:50
 msgid "Type the name of your assignment."
 msgstr "Skriv inn navnet for din oppgave."
 
 #: devilry/devilry_admin/views/period/createassignment.py:52
 msgid ""
-"Up to 20 letters of lowercase english letters (a-z), numbers, underscore (\"_"
-"\") and hyphen (\"-\")."
+"Up to 20 letters of lowercase english letters (a-z), numbers, underscore "
+"(\"_\") and hyphen (\"-\")."
 msgstr ""
 "Opp til 20 bokstaver med engelske bokstaver (a-z), tall, understrek(\"_\") "
 "og bindestrek(\"-\")."
 
 #: devilry/devilry_admin/views/period/createassignment.py:56
 #: devilry/devilry_admin/views/period/createassignment.py:319
 msgid ""
@@ -5064,16 +5020,16 @@
 #: devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html:265
 msgid "Switching diff styles does not work in markdown preview window/tab."
 msgstr ""
 "Bytting av diff stiler fungerer ikke i markdown forhåndvisning vindu/tab."
 
 #: devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html:273
 msgid ""
-"You can add latex math using the <code>$math$ $/math$</code> or <code>"
-"$mathblock$ $/mathblock$</code> tags."
+"You can add latex math using the <code>$math$ $/math$</code> or "
+"<code>$mathblock$ $/mathblock$</code> tags."
 msgstr ""
 "Du kan legge til latex matte ved å bruke <code>$math$ $/math$</code> eller "
 "<code>$mathblock$ $/mathblock$</code> taggene."
 
 #: devilry/devilry_comment/templates/devilry_comment/markdown_help.django.html:297
 msgid ""
 "Make an unordered list by preceding one or more lines of text with * symbol."
@@ -5702,14 +5658,32 @@
 msgstr "Tilbakemelding for %(assignment_name)s"
 
 #: devilry/devilry_email/feedback_email/feedback_email.py:24
 #, python-format
 msgid "Feedback updated for %(assignment_name)s"
 msgstr "Tilbakemelding oppdatert for %(assignment_name)s"
 
+#: devilry/devilry_email/groupinvite_email/groupinvite_email.py:52
+#, python-brace-format
+msgctxt "group invite"
+msgid "{user} accepted your project group invite"
+msgstr "{user} aksepterte invitasjonen til din prosjektgruppe"
+
+#: devilry/devilry_email/groupinvite_email/groupinvite_email.py:90
+#, python-brace-format
+msgctxt "group invite"
+msgid "{user} rejected your project group invite"
+msgstr "{user} avslo invitasjonen til din prosjektgruppe"
+
+#: devilry/devilry_email/groupinvite_email/groupinvite_email.py:128
+#, python-brace-format
+msgctxt "group invite"
+msgid "Project group invite for {assignment}"
+msgstr "Invitasjon til prosjektgruppe for {assignment}"
+
 #: devilry/devilry_email/templates/devilry_email/comment_email/comment.txt:4
 msgctxt "devilry comment email"
 msgid "Assignment"
 msgstr "Oppgave"
 
 #: devilry/devilry_email/templates/devilry_email/comment_email/comment.txt:6
 msgctxt "devilry comment email"
@@ -5784,14 +5758,45 @@
 msgstr "Kurs"
 
 #: devilry/devilry_email/templates/devilry_email/feedback_email/assignment_feedback_student.txt:30
 msgctxt "devilry email feedback"
 msgid "See the delivery feed for more details"
 msgstr "Se leveringsoversikten for flere detaljer"
 
+#: devilry/devilry_email/templates/devilry_email/groupinvite_email/accepted.txt:3
+#, python-format
+msgctxt "group invite"
+msgid ""
+"%(sent_to_displayname)s accepted the invite to join your project group for "
+"%(subject)s %(assignment)s"
+msgstr ""
+"%(sent_to_displayname)s aksepterte invitasjonen til din prosjektgruppe for "
+"%(subject)s %(assignment)s"
+
+#: devilry/devilry_email/templates/devilry_email/groupinvite_email/invite.txt:3
+#, python-format
+msgctxt "group invite"
+msgid ""
+"%(sent_by_displayname)s invited you to join their project group for "
+"%(subject)s %(assignment)s. Accept or reject the offer here:"
+msgstr ""
+"%(sent_by_displayname)s har invitert deg til sin prosjektgruppe\n"
+"for %(subject)s %(assignment)s.\n"
+"Godta eller avslå tilbudet her:"
+
+#: devilry/devilry_email/templates/devilry_email/groupinvite_email/rejected.txt:3
+#, python-format
+msgctxt "group invite"
+msgid ""
+"%(sent_to_displayname)s rejected the invite to join your project group for "
+"%(subject)s %(assignment)s"
+msgstr ""
+"%(sent_to_displayname)s avslo invitasjonen til din prosjektgruppe\n"
+"for %(subject)s %(assignment)s"
+
 #: devilry/devilry_examiner/cradminextensions/devilry_crmenu_examiner.py:15
 msgctxt "breadcrumb"
 msgid "Examiner"
 msgstr "Retter"
 
 #: devilry/devilry_examiner/templates/devilry_examiner/assignment/grouplist.django.html:17
 msgid "Bulk feedback"
@@ -5819,15 +5824,15 @@
 #: devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html:4
 #: devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html:11
 msgid "Passed"
 msgstr "Bestått"
 
 #: devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/grade_cell_value.django.html:9
 #: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:47
-#: devilry/devilry_message/models/base.py:353
+#: devilry/devilry_message/models/base.py:358
 #: devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html:6
 #: devilry/devilry_student/templates/devilry_student/devilry_student_shortgrade_tag.django.html:13
 msgid "Failed"
 msgstr "Ikke bestått"
 
 #: devilry/devilry_examiner/templates/devilry_examiner/assignment/simple_group_bulk_feedback/simple_group_bulk_feedbackview.django.html:27
 msgid ""
@@ -5936,21 +5941,21 @@
 msgstr "Gi tilbakemelding"
 
 #: devilry/devilry_examiner/templatetags/devilry_examiner_tags.py:57
 msgid "Show feedback"
 msgstr "Vis tilbakemelding"
 
 #: devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py:52
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:359
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:358
 msgctxt "grading"
 msgid "Passed?"
 msgstr "Bestått?"
 
 #: devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py:53
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:360
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:359
 msgctxt "grading"
 msgid "Check to provide a passing grade."
 msgstr "Huk av for å gi en bestått karakter."
 
 #: devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback.py:97
 msgid "Bulk create feedback"
 msgstr "Opprett tilbakemelding i bulk"
@@ -5961,16 +5966,16 @@
 msgstr "Tilbakemelding lagt til med bulk for %(group_names)s"
 
 #: devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py:90
 msgid "Students in groups"
 msgstr "Studenter i grupper"
 
 #: devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py:91
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:341
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:364
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:340
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:363
 msgid "Grading"
 msgstr "Karaktersetting"
 
 #: devilry/devilry_examiner/views/assignment/bulkoperations/bulk_feedback_simple.py:92
 msgid "Comment text"
 msgstr "Kommentar tekst"
 
@@ -6727,15 +6732,15 @@
 
 #: devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html:16
 msgid "Back to feed"
 msgstr "Tilbake til feed"
 
 #: devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html:21
 #: devilry/devilry_group/templates/devilry_group/listbuilder_feedbackfeed/feedbackset_info_item_value.django.html:67
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:396
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:395
 msgid "Edit grade"
 msgstr "Rediger karakter"
 
 #: devilry/devilry_group/templates/devilry_group/feedbackfeed_examiner/feedbackfeed_examiner_edit_grade.django.html:29
 msgid "Current result"
 msgstr "Nåværende resultat"
 
@@ -7028,15 +7033,15 @@
 msgstr "niende"
 
 #: devilry/devilry_group/templatetags/devilry_group_tags.py:73
 msgid "tenth"
 msgstr "tiende"
 
 #: devilry/devilry_group/views/admin/feedbackfeed_admin.py:114
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:300
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:299
 msgid "Add note"
 msgstr "Legg til notat"
 
 #: devilry/devilry_group/views/cradmin_comment_history.py:26
 msgctxt "comment edit history item"
 msgid "Only visible to you"
 msgstr "Kun synlig for deg"
@@ -7056,128 +7061,128 @@
 msgid "Comment edit history"
 msgstr "Historikk for kommentarredigering"
 
 #: devilry/devilry_group/views/cradmin_comment_history.py:62
 msgid "No items"
 msgstr "Ingen elementer"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:80
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:90
 msgid ""
 "A comment must have either text or a file attached, or both. An empty "
 "comment is not allowed."
 msgstr ""
 "En kommentar må enten innehold tekst, vedlegg eller begge. Tomme kommentarer "
 "er ikke tillatt."
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:98
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:108
 msgid "Post comment"
 msgstr "Post kommentar"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:414
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:425
 msgid "Upload files by dragging and dropping them here"
 msgstr "Last opp filer ved å dra og slippe de her"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:417
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:428
 msgid "... or select files"
 msgstr "... eller velg filer"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:420
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:431
 msgid "Select files for upload"
 msgstr "Velg filer for opplasting"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:423
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:434
 msgid "Files queued for upload:"
 msgstr "Filer køet for opplasting:"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:426
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:437
 msgid ""
 "You can browse the upload queue and check upload status further down on the "
 "page."
 msgstr ""
 "Du kan bla i opplastingskøen og sjekke status på opplasting lengre ned på "
 "siden."
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:429
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:440
 msgid "Invalid filetype"
 msgstr "Ugyldig filtype"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:431
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:442
 msgctxt "devilry_fileupload"
 msgid "Uploading"
 msgstr "Laster opp filer"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:432
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:443
 msgctxt "devilry_fileupload"
 msgid "Uploaded"
 msgstr "Filer opplastet"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:433
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:444
 msgctxt "devilry_fileupload"
 msgid "Failed"
 msgstr "Feilet"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:434
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:445
 msgctxt "devilry_fileupload"
 msgid "Deleting"
 msgstr "Sletter"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:435
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:446
 msgctxt "devilry_fileupload"
 msgid "Delete failed, try again"
 msgstr "Sletting feilet, prøv igjen"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:436
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:447
 msgctxt "devilry_fileupload"
 msgid "Upload status:"
 msgstr "Opplastingsstatus:"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:437
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:448
 msgctxt "devilry_fileupload"
 msgid "Dismiss/close error message"
 msgstr "Ignorer/lukk feilmelding"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:438
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:449
 msgctxt "devilry_fileupload"
 msgid "Remove file"
 msgstr "Fjern fil"
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:440
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:451
 #, python-format
 msgid ""
 "Filename is too long. Please use file names shorter than "
 "%(max_filename_length)s characters."
 msgstr ""
 "Filnavn er for langt. Vennligst bruk filnavn kortere enn "
 "%(max_filename_length)s tegn."
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:444
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:455
 msgid ""
 "Server timeout while uploading the file. This may be caused by a poor upload "
 "link and/or a too large file."
 msgstr ""
 "Server ble tidsavbrutt ved opplasting av fil. Dette kan være forårsaket av "
 "dårlig nettforbindelse og/eller en for stor fil."
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:447
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:458
 msgid ""
 "Unknown error. May be a server glitch or a bug. Please try again, and report "
 "the error if it happens multiple times."
 msgstr ""
 "Ukjent feil. Dette kan være en systemfeil. Vennligst prøv igjen, og "
 "rapporter feilen hvis det skjer flere ganger."
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:450
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:461
 msgid ""
 "We could not delete the file. This may be a server glitch or bug. Please try "
 "again, and report if the error happens multiple times."
 msgstr ""
 "Filen kunne ikke bli slettet. Dette kan være en systemfeil. Vennligst prøv "
 "igjen, og rapporter feilen hvis det skjer flere ganger."
 
-#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:563
+#: devilry/devilry_group/views/cradmin_feedbackfeed_base.py:574
 msgid "Comment added!"
 msgstr "Lagt til kommentar!"
 
 #: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:49
 msgctxt "grading"
 msgid "Grade"
 msgstr "Karakter"
@@ -7201,27 +7206,27 @@
 msgid "Publish feedback"
 msgstr "Publiser tilbakemelding"
 
 #: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:228
 msgid "Feedback is already published!"
 msgstr "Tilbakemelding er allerede publisert!"
 
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:344
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:343
 msgid ""
 "Give a score between {} to {} where {} is the minimum amount of points "
 "needed to pass."
 msgstr ""
 "Sett en poengsum mellom {} og {}, hvor {} er minimum antall poeng som kreves "
 "for å bestå."
 
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:365
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:364
 msgid "Check the box to give a passing grade"
 msgstr "Velg denne for å gi bestått karakter"
 
-#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:494
+#: devilry/devilry_group/views/examiner/feedbackfeed_examiner.py:493
 msgid "Groupcomment"
 msgstr "Gruppekommentar"
 
 #: devilry/devilry_group/views/group_comment_edit_base.py:55
 #: devilry/devilry_group/views/group_comment_edit_base.py:58
 msgid "Edit comment"
 msgstr "Rediger kommentar"
@@ -7326,24 +7331,24 @@
 msgstr "Bygger listen over brukere det skal sendes til."
 
 #: devilry/devilry_message/models/base.py:78
 msgid "Sending"
 msgstr "Sender"
 
 #: devilry/devilry_message/models/base.py:80
-#: devilry/devilry_message/models/base.py:355
+#: devilry/devilry_message/models/base.py:360
 msgid "Error"
 msgstr "Feil"
 
 #: devilry/devilry_message/models/base.py:82
-#: devilry/devilry_message/models/base.py:357
+#: devilry/devilry_message/models/base.py:362
 msgid "Sent"
 msgstr "Sendt"
 
-#: devilry/devilry_message/models/base.py:351
+#: devilry/devilry_message/models/base.py:356
 msgid "Not sent"
 msgstr "Ikke sent"
 
 #: devilry/devilry_qualifiesforexam/models.py:93
 msgid "Ready for export"
 msgstr "Klar for eksportering"
 
@@ -7579,15 +7584,15 @@
 #: devilry/devilry_qualifiesforexam_plugin_students/plugin.py:13
 msgid "Manually select the students that qualifies for exam."
 msgstr "Manuelt velg studenter som kvalifiserer for eksamen."
 
 #: devilry/devilry_report/templates/devilry_report/download_report.django.html:11
 msgid ""
 "The download will start automatically as soon as the report is finished."
-msgstr "Nedlastingen vil starte så for rapporten er ferdig."
+msgstr "Nedlastingen vil starte så fort rapporten er ferdig."
 
 #: devilry/devilry_student/cradminextensions/columntypes.py:13
 #: devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_details.django.html:8
 #: devilry/devilry_student/templates/devilry_student/cradmin_group/deliveriesapp/delivery_details.django.html:18
 msgid "Delivery"
 msgstr "Innlevering"
 
@@ -7932,25 +7937,51 @@
 "eller laste opp innleveringer etter fristen."
 
 #: devilry/project/common/projectspecific_settings.py:222
 msgid ""
 "This assignment uses hard deadlines. Students will not be able to write "
 "comments or upload files after the deadline has expired."
 msgstr ""
-"Denne oppdaven bruker harde frister. Studenter vil ikke kunne skrive "
+"Denne oppgaven bruker harde frister. Studenter vil ikke kunne skrive "
 "kommentarer eller laste opp innleveringer etter fristen."
 
 #: devilry/project/common/settings.py:174
 msgid "English"
 msgstr "Engelsk"
 
 #: devilry/project/common/settings.py:175
 msgid "Norwegian Bokmal"
 msgstr "Norsk bokmål"
 
+#, python-format
+#~ msgid ""
+#~ "%(sent_to_displayname)s accepted the invite to join your project\n"
+#~ "group for %(subject)s %(assignment)s"
+#~ msgstr ""
+#~ "%(sent_to_displayname)s godtok invitasjonen til din prosjektgruppe\n"
+#~ "for %(subject)s %(assignment)s"
+
+#, python-format
+#~ msgid ""
+#~ "%(sent_by_displayname)s invited you to join their project\n"
+#~ "group for %(subject)s %(assignment)s.\n"
+#~ "Accept or reject the offer here:"
+#~ msgstr ""
+#~ "%(sent_by_displayname)s har invitert deg til sin prosjektgruppe\n"
+#~ "for %(subject)s %(assignment)s.\n"
+#~ "Godta eller avslå tilbudet her:"
+
+#, python-format
+#~ msgid ""
+#~ "%(sent_to_displayname)s rejected the invite to join your project\n"
+#~ "group for %(subject)s %(assignment)s"
+#~ msgstr ""
+#~ "%(sent_to_displayname)s avslo invitasjonen til din prosjektgruppe\n"
+#~ "for %(subject)s %(assignment)s"
+
 #~ msgctxt "examiner dashboard"
 #~ msgid "Self-assign available"
 #~ msgstr "Selv-tilordning tilgjengelig"
 
 #~ msgid ""
 #~ "Semesters where assigning yourself as examiner is available. This list is "
 #~ "available as long as there are projectgroups open for selfassigning or "
```

### Comparing `devilry-6.0.0rc1/devilry/locale/nb/LC_MESSAGES/djangojs.po` & `devilry-6.0.0rc2/devilry/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/log.py` & `devilry-6.0.0rc2/devilry/project/log.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/settingsproxy.py` & `devilry-6.0.0rc2/devilry/project/settingsproxy.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/common/cradmin_legacy_settings.py` & `devilry-6.0.0rc2/devilry/project/common/cradmin_legacy_settings.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/common/default_urls.py` & `devilry-6.0.0rc2/devilry/project/common/default_urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/common/projectspecific_settings.py` & `devilry-6.0.0rc2/devilry/project/common/projectspecific_settings.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/common/settings.py` & `devilry-6.0.0rc2/devilry/project/common/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,16 @@
 MIDDLEWARE = [
     'django.middleware.common.CommonMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'devilry.devilry_i18n.middleware.LocaleMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'devilry.utils.logexceptionsmiddleware.TracebackLoggingMiddleware',
-    'devilry.devilry_account.middleware.LocalMiddleware'
+    'devilry.devilry_account.middleware.LocalMiddleware',
+    'django.middleware.csrf.CsrfViewMiddleware'
 ]
 
 ##################################################################################
 # Django Cradmin settings (Auth backend, forgotten password and sitename)
 ##################################################################################
 AUTHENTICATION_BACKENDS = [
     'devilry.devilry_account.authbackend.default.EmailAuthBackend',
```

### Comparing `devilry-6.0.0rc1/devilry/project/common/templatecontext.py` & `devilry-6.0.0rc2/devilry/project/common/templatecontext.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/common/management/commands/devilry_common_merge_candidates.py` & `devilry-6.0.0rc2/devilry/project/common/management/commands/devilry_common_merge_candidates.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/dev_urls.py` & `devilry-6.0.0rc2/devilry/project/develop/dev_urls.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/fabrictasks.py` & `devilry-6.0.0rc2/devilry/project/develop/fabrictasks.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/middleware.py` & `devilry-6.0.0rc2/devilry/project/develop/middleware.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/dumps/old_default.sql` & `devilry-6.0.0rc2/devilry/project/develop/dumps/old_default.sql`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/management/commands/devilry_developer_create_deliveries_from_filesystemtree.py` & `devilry-6.0.0rc2/devilry/project/develop/management/commands/devilry_developer_create_deliveries_from_filesystemtree.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/management/commands/devilry_developer_delete_all_except_users.py` & `devilry-6.0.0rc2/devilry/project/develop/management/commands/devilry_developer_delete_all_except_users.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/management/commands/devilry_developer_performance_test_db.py` & `devilry-6.0.0rc2/devilry/project/develop/management/commands/devilry_developer_performance_test_db.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/settings/base.py` & `devilry-6.0.0rc2/devilry/project/develop/settings/base.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/settings/develop.py` & `devilry-6.0.0rc2/devilry/project/develop/settings/develop.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/settings/test.py` & `devilry-6.0.0rc2/devilry/project/develop/settings/test.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/testhelpers/corebuilder.py` & `devilry-6.0.0rc2/devilry/project/develop/testhelpers/corebuilder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/testhelpers/datebuilder.py` & `devilry-6.0.0rc2/devilry/project/develop/testhelpers/datebuilder.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/testhelpers/login.py` & `devilry-6.0.0rc2/devilry/project/develop/testhelpers/login.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/project/develop/testhelpers/soupselect.py` & `devilry-6.0.0rc2/devilry/project/develop/testhelpers/soupselect.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/GroupAssignments.py` & `devilry-6.0.0rc2/devilry/utils/GroupAssignments.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/GroupNodes.py` & `devilry-6.0.0rc2/devilry/utils/GroupNodes.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/OrderedDictFallback.py` & `devilry-6.0.0rc2/devilry/utils/OrderedDictFallback.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/anonymize_database.py` & `devilry-6.0.0rc2/devilry/utils/anonymize_database.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/datetimeutils.py` & `devilry-6.0.0rc2/devilry/utils/datetimeutils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/delivery_collection.py` & `devilry-6.0.0rc2/devilry/utils/delivery_collection.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/devilry_djangoaggregate_functions.py` & `devilry-6.0.0rc2/devilry/utils/devilry_djangoaggregate_functions.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/devilry_email.py` & `devilry-6.0.0rc2/devilry/utils/devilry_email.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/filewrapperwithexplicitclose.py` & `devilry-6.0.0rc2/devilry/utils/filewrapperwithexplicitclose.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/groups_groupedby_relatedstudent_and_assignment.py` & `devilry-6.0.0rc2/devilry/utils/groups_groupedby_relatedstudent_and_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/importutils.py` & `devilry-6.0.0rc2/devilry/utils/importutils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/management.py` & `devilry-6.0.0rc2/devilry/utils/management.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/migrationutils.py` & `devilry-6.0.0rc2/devilry/utils/migrationutils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/nodenamesuggestor.py` & `devilry-6.0.0rc2/devilry/utils/nodenamesuggestor.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/passed_in_previous_period.py` & `devilry-6.0.0rc2/devilry/utils/passed_in_previous_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/profile.py` & `devilry-6.0.0rc2/devilry/utils/profile.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/rq_setup.py` & `devilry-6.0.0rc2/devilry/utils/rq_setup.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/setting_utils.py` & `devilry-6.0.0rc2/devilry/utils/setting_utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/stream_archives.py` & `devilry-6.0.0rc2/devilry/utils/stream_archives.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/api/api_test_mixin.py` & `devilry-6.0.0rc2/devilry/utils/api/api_test_mixin.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/demodb/demousers.py` & `devilry-6.0.0rc2/devilry/utils/demodb/demousers.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/graphviz/djangomodels.py` & `devilry-6.0.0rc2/devilry/utils/graphviz/djangomodels.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/graphviz/dot.py` & `devilry-6.0.0rc2/devilry/utils/graphviz/dot.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/tests/delivery_collection_tests.py` & `devilry-6.0.0rc2/devilry/utils/tests/delivery_collection_tests.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/tests/importutils.py` & `devilry-6.0.0rc2/devilry/utils/tests/importutils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/tests/streamable_archive_tests.py` & `devilry-6.0.0rc2/devilry/utils/tests/streamable_archive_tests.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/tests/test_anonymize_db.py` & `devilry-6.0.0rc2/devilry/utils/tests/test_anonymize_db.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/tests/test_datetimeutils.py` & `devilry-6.0.0rc2/devilry/utils/tests/test_datetimeutils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/tests/test_groups_groupedby_relatedstudent_and_assignment.py` & `devilry-6.0.0rc2/devilry/utils/tests/test_groups_groupedby_relatedstudent_and_assignment.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/tests/test_nodenamesuggestor.py` & `devilry-6.0.0rc2/devilry/utils/tests/test_nodenamesuggestor.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/tests/test_passed_in_previous_period.py` & `devilry-6.0.0rc2/devilry/utils/tests/test_passed_in_previous_period.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/tests/test_setting_utils.py` & `devilry-6.0.0rc2/devilry/utils/tests/test_setting_utils.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/devilry/utils/tests/test_url_datetime.py` & `devilry-6.0.0rc2/devilry/utils/tests/test_url_datetime.py`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/.gitignore` & `devilry-6.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/LICENSE` & `devilry-6.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `devilry-6.0.0rc1/README.md` & `devilry-6.0.0rc2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 ### Create or re-create a devdatabase
 You should always clear the database before recreating it. The easiest way is just to clear the docker resources (and volumes) and start it again.
 ```
 $ docker-compose down -v
 $ docker-compose up
 ```
 
-Run dev server (in a new terminal) 
+Run dev server (in a new terminal)
 ```
 $ source .venv/bin/activate   # activate virtualenv
 $ ievv devrun
 ```
 
 Load devdatabase SQL-file (in a new terminal)
 ```
@@ -148,17 +148,28 @@
 
 ```
 $ docker-compose down -v
 ```
 
 ## Documentation
 
-http://ievv-opensource.readthedocs.org/
+https://devilry.readthedocs.io
 
-## How to release devilry
+## Release
+
+### Translations
+
+To translate new texts, do the following:
+
+- ``ievv makemessages``
+- Translate the .po files. Poedit is a great tool for this.
+- ``ievv compilemessages``
+- Commit the changes
+
+### Set version and build staticfiles
 
 First make sure you have NO UNCOMITTED CHANGES!
 
 Release (create changelog, increment version, build staticfiles, commit and tag the change) with:
 
 ```bash
 $ nvm use 14
@@ -181,14 +192,19 @@
   commit.
 - The `cz` command comes from `commitizen` (install documented above).
 
 ### What if the release fails?
 
 See _How to revert a bump_ in the [commitizen FAQ](https://commitizen-tools.github.io/commitizen/faq/#how-to-revert-a-bump).
 
+
+### Migrationguide and changelog (for official readthedocs)
+- Add a migration guide to not_for_deploy/docs/sysadmin/migrationguides/
+- Add a changelog to not_for_deploy/docs/user/changelog/
+
 ### Release to pypi:
 
 ```bash
 $ hatch build -t sdist
 $ hatch publish
 $ rm dist/*              # optional cleanup
 ```
```

### Comparing `devilry-6.0.0rc1/pyproject.toml` & `devilry-6.0.0rc2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "devilry"
-requires-python = ">=3.10.0"
+requires-python = ">=3.9.0"
 dynamic = ["version"]
 description = "A system for handling electronic deliveries. See https://github.com/devilry/devilry-django."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     { name = "Espen Angell Kristiansen", email = "post@appresso.no" },
     { name = "Tor Johansen" },
@@ -29,15 +29,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
 ]
 dependencies = [
     "Django>=4.2.0,<4.3.0",
     "pyyaml>=5.4.0,<5.5.0",
     "Markdown>=3.3.0,<3.4.0",
-    "Pygments>=2.7.0,<2.8.0",
+    "Pygments>=2.15.0,<2.16.0",
     "flup>=1.0.0,<1.1.0",
     "gunicorn>=19.9.0,<19.10.0",
     "django-crispy-forms>=1.14.0,<1.15.0",
     "openpyxl",
     "URLObject>=2.4.0,<2.5.0",
     "mimeparse>=0.1.0,<0.2.0",
     "numpy",
@@ -74,25 +74,25 @@
 
 [project.optional-dependencies]
 dev = [
     "django-debug-toolbar",
     "model-bakery",
     "BeautifulSoup4==4.7.1",
     "htmls==1.0.0",
-    "Sphinx==1.7.0",
-    "sphinx_rtd_theme==0.2.4",
-    "sphinxcontrib-napoleon==0.6.1",
+    "sphinx==6.2.1",
+    "sphinx_rtd_theme==1.2.2",
     "flake8==2.2.2",
     "tox==1.7.2",
     "pyflakes==0.8.1",
     "Fabric3==1.14.post1",
     "doc2dash==3.0.0",
     "django-storages==1.1.5",
     "boto==2.32.1",
-    "django-auth-ldap"
+    "django-auth-ldap",
+    "pip-tools",
 ]
 test = [
     "htmls",
     "pytest",
     "pytest-django",
     "pytest-env",
     "model-bakery",
@@ -114,13 +114,13 @@
     "node_modules",
     "/devilry/devilry_theme3/staticsources",
     "/devilry/project/develop/dumps/default.sql"
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "6.0.0rc1"
+version = "6.0.0rc2"
 version_files = [
     "devilry/__init__.py:__version__"
 ]
 tag_format = "$version"
 update_changelog_on_bump = true
```

### Comparing `devilry-6.0.0rc1/PKG-INFO` & `devilry-6.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devilry
-Version: 6.0.0rc1
+Version: 6.0.0rc2
 Summary: A system for handling electronic deliveries. See https://github.com/devilry/devilry-django.
 Author: Tor Johansen, Bendik Opstad, Vegard Angell, Magne Westlie, Ilya Kostolomov, Christian Tryti, Rebekka Mørken, Stian Julseth
 Author-email: Espen Angell Kristiansen <post@appresso.no>
 License: Copyright (c) 2010, Devilry contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -32,15 +32,15 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Requires-Python: >=3.10.0
+Requires-Python: >=3.9.0
 Requires-Dist: arrow<0.13.0,>=0.12.0
 Requires-Dist: certifi<2017.12.0,>=2017.11.0
 Requires-Dist: chardet<3.1.0,>=3.0.0
 Requires-Dist: cradmin-legacy<6.0.0,>=5.0.0
 Requires-Dist: detektor==1.1.0-beta.012
 Requires-Dist: dj-database-url<0.4.0,>=0.3.0
 Requires-Dist: dj-static<0.1.0,>=0.0.0
@@ -60,15 +60,15 @@
 Requires-Dist: markdown<3.4.0,>=3.3.0
 Requires-Dist: mimeparse<0.2.0,>=0.1.0
 Requires-Dist: numpy
 Requires-Dist: oauthlib<2.1.0,>=2.0.0
 Requires-Dist: openpyxl
 Requires-Dist: psycopg2
 Requires-Dist: pycountry<17.10.0,>=17.9.0
-Requires-Dist: pygments<2.8.0,>=2.7.0
+Requires-Dist: pygments<2.16.0,>=2.15.0
 Requires-Dist: python-dateutil<2.9.0,>=2.8.0
 Requires-Dist: python-openid<2.3.0,>=2.2.0
 Requires-Dist: pytz<2018.10.0,>=2018.9.0
 Requires-Dist: pyyaml<5.5.0,>=5.4.0
 Requires-Dist: redis<3.6.0,>=3.5.0
 Requires-Dist: requests
 Requires-Dist: requests-oauthlib<0.9.0,>=0.8.0
@@ -84,18 +84,18 @@
 Requires-Dist: django-debug-toolbar; extra == 'dev'
 Requires-Dist: django-storages==1.1.5; extra == 'dev'
 Requires-Dist: doc2dash==3.0.0; extra == 'dev'
 Requires-Dist: fabric3==1.14.post1; extra == 'dev'
 Requires-Dist: flake8==2.2.2; extra == 'dev'
 Requires-Dist: htmls==1.0.0; extra == 'dev'
 Requires-Dist: model-bakery; extra == 'dev'
+Requires-Dist: pip-tools; extra == 'dev'
 Requires-Dist: pyflakes==0.8.1; extra == 'dev'
-Requires-Dist: sphinx-rtd-theme==0.2.4; extra == 'dev'
-Requires-Dist: sphinx==1.7.0; extra == 'dev'
-Requires-Dist: sphinxcontrib-napoleon==0.6.1; extra == 'dev'
+Requires-Dist: sphinx-rtd-theme==1.2.2; extra == 'dev'
+Requires-Dist: sphinx==6.2.1; extra == 'dev'
 Requires-Dist: tox==1.7.2; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: htmls; extra == 'test'
 Requires-Dist: mock==3.0.5; extra == 'test'
 Requires-Dist: model-bakery; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
@@ -203,15 +203,15 @@
 ### Create or re-create a devdatabase
 You should always clear the database before recreating it. The easiest way is just to clear the docker resources (and volumes) and start it again.
 ```
 $ docker-compose down -v
 $ docker-compose up
 ```
 
-Run dev server (in a new terminal) 
+Run dev server (in a new terminal)
 ```
 $ source .venv/bin/activate   # activate virtualenv
 $ ievv devrun
 ```
 
 Load devdatabase SQL-file (in a new terminal)
 ```
@@ -253,17 +253,28 @@
 
 ```
 $ docker-compose down -v
 ```
 
 ## Documentation
 
-http://ievv-opensource.readthedocs.org/
+https://devilry.readthedocs.io
 
-## How to release devilry
+## Release
+
+### Translations
+
+To translate new texts, do the following:
+
+- ``ievv makemessages``
+- Translate the .po files. Poedit is a great tool for this.
+- ``ievv compilemessages``
+- Commit the changes
+
+### Set version and build staticfiles
 
 First make sure you have NO UNCOMITTED CHANGES!
 
 Release (create changelog, increment version, build staticfiles, commit and tag the change) with:
 
 ```bash
 $ nvm use 14
@@ -286,14 +297,19 @@
   commit.
 - The `cz` command comes from `commitizen` (install documented above).
 
 ### What if the release fails?
 
 See _How to revert a bump_ in the [commitizen FAQ](https://commitizen-tools.github.io/commitizen/faq/#how-to-revert-a-bump).
 
+
+### Migrationguide and changelog (for official readthedocs)
+- Add a migration guide to not_for_deploy/docs/sysadmin/migrationguides/
+- Add a changelog to not_for_deploy/docs/user/changelog/
+
 ### Release to pypi:
 
 ```bash
 $ hatch build -t sdist
 $ hatch publish
 $ rm dist/*              # optional cleanup
 ```
```

