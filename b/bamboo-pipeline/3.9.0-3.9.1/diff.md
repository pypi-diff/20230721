# Comparing `tmp/bamboo-pipeline-3.9.0.tar.gz` & `tmp/bamboo-pipeline-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bamboo-pipeline-3.9.0.tar", max compression
+gzip compressed data, was "bamboo-pipeline-3.9.1.tar", max compression
```

## Comparing `bamboo-pipeline-3.9.0.tar` & `bamboo-pipeline-3.9.1.tar`

### file list

```diff
@@ -1,363 +1,363 @@
--rw-r--r--   0        0        0     1069 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/LICENSE
--rw-r--r--   0        0        0      826 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/__init__.py
--rw-r--r--   0        0        0     1469 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/admin.py
--rw-r--r--   0        0        0     3559 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/apps.py
--rw-r--r--   0        0        0      810 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/builder/__init__.py
--rw-r--r--   0        0        0     6968 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/builder/builder.py
--rw-r--r--   0        0        0      871 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/builder/flow/__init__.py
--rw-r--r--   0        0        0     2479 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/builder/flow/activity.py
--rw-r--r--   0        0        0     2415 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/builder/flow/base.py
--rw-r--r--   0        0        0     3009 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/builder/flow/data.py
--rw-r--r--   0        0        0     1251 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/builder/flow/event.py
--rw-r--r--   0        0        0     1788 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/builder/flow/gateway.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/celery/__init__.py
--rw-r--r--   0        0        0     1297 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/celery/queues.py
--rw-r--r--   0        0        0     6975 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/celery/settings.py
--rw-r--r--   0        0        0      833 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/__init__.py
--rw-r--r--   0        0        0     1037 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/admin.py
--rw-r--r--   0        0        0     2732 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/apps.py
--rw-r--r--   0        0        0     3971 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/base.py
--rw-r--r--   0        0        0     2685 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/component.py
--rw-r--r--   0        0        0     3866 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/constant.py
--rw-r--r--   0        0        0      785 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/constants.py
--rw-r--r--   0        0        0     1104 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/context.py
--rw-r--r--   0        0        0     2626 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/library.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/management/__init__.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/management/commands/__init__.py
--rw-r--r--   0        0        0     2506 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/management/commands/run_component.py
--rw-r--r--   0        0        0     1001 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/management/commands/update_component_models.py
--rw-r--r--   0        0        0     1557 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0001_initial.py
--rw-r--r--   0        0        0      993 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0002_delete_componentmodel.py
--rw-r--r--   0        0        0     1694 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0003_componentmodel.py
--rw-r--r--   0        0        0     1225 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0004_auto_20180413_1800.py
--rw-r--r--   0        0        0     1409 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0005_auto_20190723_1806.py
--rw-r--r--   0        0        0      520 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0006_auto_20200213_0743.py
--rw-r--r--   0        0        0     1523 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0007_auto_20201112_2244.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/__init__.py
--rw-r--r--   0        0        0     3313 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/models.py
--rw-r--r--   0        0        0     3597 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/runner.py
--rw-r--r--   0        0        0    13151 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/component_framework/test.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/components/__init__.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/components/collections/__init__.py
--rw-r--r--   0        0        0     1697 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/components/collections/examples.py
--rw-r--r--   0        0        0     1205 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/conf/__init__.py
--rw-r--r--   0        0        0     4596 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/conf/default_settings.py
--rw-r--r--   0        0        0      837 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/constants.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/__init__.py
--rw-r--r--   0        0        0      835 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/__init__.py
--rw-r--r--   0        0        0     1669 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/admin.py
--rw-r--r--   0        0        0     2746 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/apps.py
--rw-r--r--   0        0        0      805 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/exceptions.py
--rw-r--r--   0        0        0     1633 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/loader.py
--rw-r--r--   0        0        0     4333 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/migrations/0001_initial.py
--rw-r--r--   0        0        0      465 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/migrations/0002_s3source_source_dir.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/migrations/__init__.py
--rw-r--r--   0        0        0      906 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/models/__init__.py
--rw-r--r--   0        0        0     5337 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/models/base.py
--rw-r--r--   0        0        0     1253 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/models/fields.py
--rw-r--r--   0        0        0     1299 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/models/forms.py
--rw-r--r--   0        0        0     3271 2021-11-23 09:21:36.882749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/models/source.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/__init__.py
--rw-r--r--   0        0        0     1116 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/importer/__init__.py
--rw-r--r--   0        0        0     6635 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/importer/base.py
--rw-r--r--   0        0        0     3201 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/importer/fs.py
--rw-r--r--   0        0        0     3502 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/importer/git.py
--rw-r--r--   0        0        0     4391 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/importer/s3.py
--rw-r--r--   0        0        0     1430 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/importer/utils.py
--rw-r--r--   0        0        0     1024 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/requirement.py
--rw-r--r--   0        0        0      829 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/__init__.py
--rw-r--r--   0        0        0     1371 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/admin.py
--rw-r--r--   0        0        0     1034 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/apps.py
--rw-r--r--   0        0        0     1353 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/context.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/__init__.py
--rw-r--r--   0        0        0     1341 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/compat.py
--rw-r--r--   0        0        0     2796 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/db.py
--rw-r--r--   0        0        0     7118 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/managers.py
--rw-r--r--   0        0        0     3689 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/migrate.py
--rw-r--r--   0        0        0     8361 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/models.py
--rw-r--r--   0        0        0     4112 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/tzcrontab.py
--rw-r--r--   0        0        0     1344 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/utils.py
--rw-r--r--   0        0        0    10344 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/0001_initial.py
--rw-r--r--   0        0        0     1136 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/0002_auto_20190103_1918.py
--rw-r--r--   0        0        0     3390 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/0003_auto_20191213_0819.py
--rw-r--r--   0        0        0      721 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/0004_auto_20191213_0828.py
--rw-r--r--   0        0        0      523 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/0005_migrate_task.py
--rw-r--r--   0        0        0      632 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/0006_change_task_ref_table.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/__init__.py
--rw-r--r--   0        0        0     7856 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/models.py
--rw-r--r--   0        0        0     1045 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/signals/__init__.py
--rw-r--r--   0        0        0     6794 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/tasks.py
--rw-r--r--   0        0        0     4090 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/tests.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/views.py
--rw-r--r--   0        0        0      824 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/__init__.py
--rw-r--r--   0        0        0     2324 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/admin.py
--rw-r--r--   0        0        0     1097 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/apps.py
--rw-r--r--   0        0        0     4178 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0001_initial.py
--rw-r--r--   0        0        0     1044 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0002_auto_20180817_1212.py
--rw-r--r--   0        0        0     1510 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0003_auto_20180821_2015.py
--rw-r--r--   0        0        0     2849 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0004_instanceinpipeline_templateinpipeline.py
--rw-r--r--   0        0        0      908 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0005_init_pipeline_data.py
--rw-r--r--   0        0        0     1389 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0006_auto_20181115_1208.py
--rw-r--r--   0        0        0     3123 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0007_init_pipeline_data.py
--rw-r--r--   0        0        0     2563 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0008_auto_20181116_1448.py
--rw-r--r--   0        0        0     1828 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0009_auto_20181116_1627.py
--rw-r--r--   0        0        0     2857 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0010_auto_20190304_1747.py
--rw-r--r--   0        0        0     1212 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0011_auto_20200217_0822.py
--rw-r--r--   0        0        0      724 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0012_auto_20201123_1552.py
--rw-r--r--   0        0        0      734 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0013_auto_20201201_1506.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/__init__.py
--rw-r--r--   0        0        0     4080 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/models.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/signals/__init__.py
--rw-r--r--   0        0        0     5006 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/signals/handlers.py
--rw-r--r--   0        0        0     7773 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/tasks.py
--rw-r--r--   0        0        0     1184 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/contrib/statistics/utils.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/core/__init__.py
--rw-r--r--   0        0        0     2781 2021-11-23 09:21:36.886749 bamboo-pipeline-3.9.0/pipeline/core/constants.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/data/__init__.py
--rw-r--r--   0        0        0     3109 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/data/base.py
--rw-r--r--   0        0        0     5375 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/data/context.py
--rw-r--r--   0        0        0     1641 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/data/converter.py
--rw-r--r--   0        0        0     6055 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/data/expression.py
--rw-r--r--   0        0        0     1640 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/data/hydration.py
--rw-r--r--   0        0        0     1131 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/data/library.py
--rw-r--r--   0        0        0     2103 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/data/mako_safety.py
--rw-r--r--   0        0        0     2536 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/data/sandbox.py
--rw-r--r--   0        0        0      910 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/data/schemas.py
--rw-r--r--   0        0        0     5002 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/data/var.py
--rw-r--r--   0        0        0     3012 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/flow/__init__.py
--rw-r--r--   0        0        0     1001 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/flow/activity/__init__.py
--rw-r--r--   0        0        0     1432 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/flow/activity/base.py
--rw-r--r--   0        0        0     8859 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/flow/activity/service_activity.py
--rw-r--r--   0        0        0     1849 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/flow/activity/subprocess.py
--rw-r--r--   0        0        0     5219 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/flow/base.py
--rw-r--r--   0        0        0     1966 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/flow/event.py
--rw-r--r--   0        0        0     7271 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/flow/gateway.py
--rw-r--r--   0        0        0     3847 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/flow/io.py
--rw-r--r--   0        0        0      866 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/flow/signals.py
--rw-r--r--   0        0        0     4266 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/pipeline.py
--rw-r--r--   0        0        0      852 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/core/signals/__init__.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/django_signal_valve/__init__.py
--rw-r--r--   0        0        0     1012 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/django_signal_valve/admin.py
--rw-r--r--   0        0        0     1465 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/django_signal_valve/migrations/0001_initial.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/django_signal_valve/migrations/__init__.py
--rw-r--r--   0        0        0     1885 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/django_signal_valve/models.py
--rw-r--r--   0        0        0     2119 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/django_signal_valve/valve.py
--rw-r--r--   0        0        0      807 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/__init__.py
--rw-r--r--   0        0        0     5392 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/admin.py
--rw-r--r--   0        0        0    19655 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/api.py
--rw-r--r--   0        0        0     1210 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/apps.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/conf/__init__.py
--rw-r--r--   0        0        0     1048 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/conf/function_switch.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/__init__.py
--rw-r--r--   0        0        0     3819 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/api.py
--rw-r--r--   0        0        0     1123 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/context.py
--rw-r--r--   0        0        0      803 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/data/__init__.py
--rw-r--r--   0        0        0     4149 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/data/api.py
--rw-r--r--   0        0        0     1304 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/data/base_backend.py
--rw-r--r--   0        0        0     1369 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/data/mysql_backend.py
--rw-r--r--   0        0        0     1785 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/data/redis_backend.py
--rw-r--r--   0        0        0     2463 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/__init__.py
--rw-r--r--   0        0        0     1496 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/base.py
--rw-r--r--   0        0        0     2540 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/conditional_parallel.py
--rw-r--r--   0        0        0     1956 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/converge_gateway.py
--rw-r--r--   0        0        0     1854 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/empty_start_event.py
--rw-r--r--   0        0        0      877 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/endevent/__init__.py
--rw-r--r--   0        0        0     2570 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/endevent/base.py
--rw-r--r--   0        0        0      954 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/endevent/empty_end_event.py
--rw-r--r--   0        0        0     1748 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/endevent/executable_end_event.py
--rw-r--r--   0        0        0     2157 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/exclusive_gateway.py
--rw-r--r--   0        0        0     1994 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/parallel_gateway.py
--rw-r--r--   0        0        0     6166 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/service_activity.py
--rw-r--r--   0        0        0     2145 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/subprocess.py
--rw-r--r--   0        0        0     5588 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/runtime.py
--rw-r--r--   0        0        0    11133 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/core/schedule.py
--rw-r--r--   0        0        0     1461 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/exceptions.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/health/__init__.py
--rw-r--r--   0        0        0      817 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/health/zombie/__init__.py
--rw-r--r--   0        0        0     5158 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/health/zombie/doctors.py
--rw-r--r--   0        0        0     2420 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/health/zombie/heal.py
--rw-r--r--   0        0        0      849 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/logging.py
--rw-r--r--   0        0        0    10805 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0001_initial.py
--rw-r--r--   0        0        0     1210 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0002_auto_20180109_1825.py
--rw-r--r--   0        0        0     2850 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0003_auto_20180717_1148.py
--rw-r--r--   0        0        0     1041 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0004_auto_20180717_1411.py
--rw-r--r--   0        0        0     1148 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0005_auto_20180717_1433.py
--rw-r--r--   0        0        0     1149 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0006_auto_20180717_1543.py
--rw-r--r--   0        0        0     1270 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0007_auto_20180717_2022.py
--rw-r--r--   0        0        0     1470 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0008_schedulecelerytask.py
--rw-r--r--   0        0        0     1199 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0009_status_error_ignorable.py
--rw-r--r--   0        0        0     1217 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0010_auto_20180830_1203.py
--rw-r--r--   0        0        0     1466 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0010_nodecelerytask.py
--rw-r--r--   0        0        0     1209 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0011_auto_20180830_1205.py
--rw-r--r--   0        0        0     1447 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0015_datasnapshot.py
--rw-r--r--   0        0        0     1313 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0016_auto_20181228_0345.py
--rw-r--r--   0        0        0     1158 2021-11-23 09:21:36.890749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0017_auto_20190719_1010.py
--rw-r--r--   0        0        0     3113 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0018_auto_20190729_1041.py
--rw-r--r--   0        0        0     1441 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0019_auto_20190729_1044.py
--rw-r--r--   0        0        0      467 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0020_pipelinemodel_priority.py
--rw-r--r--   0        0        0     2710 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0021_auto_20191213_0725.py
--rw-r--r--   0        0        0      518 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0022_scheduleservice_multi_callback_enabled.py
--rw-r--r--   0        0        0      523 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0023_status_state_refresh_at.py
--rw-r--r--   0        0        0     1558 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0024_auto_20200224_0308.py
--rw-r--r--   0        0        0      748 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0025_multicallbackdata.py
--rw-r--r--   0        0        0     1551 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0026_auto_20200610_1442.py
--rw-r--r--   0        0        0     1520 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0027_sendfailedcelerytask.py
--rw-r--r--   0        0        0      462 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/0028_auto_20210812_0906.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/migrations/__init__.py
--rw-r--r--   0        0        0      905 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/models/__init__.py
--rw-r--r--   0        0        0    51167 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/models/core.py
--rw-r--r--   0        0        0     1788 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/models/data.py
--rw-r--r--   0        0        0     1984 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/models/fields.py
--rw-r--r--   0        0        0     2368 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/models/function.py
--rw-r--r--   0        0        0    55112 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/models/nr_pickle.py
--rw-r--r--   0        0        0     2115 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/signals/__init__.py
--rw-r--r--   0        0        0     3791 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/signals/dispatch.py
--rw-r--r--   0        0        0     5836 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/signals/handlers.py
--rw-r--r--   0        0        0     3209 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/states.py
--rw-r--r--   0        0        0    13579 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/tasks.py
--rw-r--r--   0        0        0     2043 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/engine/utils.py
--rw-r--r--   0        0        0      801 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/__init__.py
--rw-r--r--   0        0        0     3115 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/admin.py
--rw-r--r--   0        0        0     1055 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/apps.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/celery/__init__.py
--rw-r--r--   0        0        0     2196 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/celery/queues.py
--rw-r--r--   0        0        0     1030 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/celery/step.py
--rw-r--r--   0        0        0     1893 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/celery/tasks.py
--rw-r--r--   0        0        0     1659 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/codec.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/__init__.py
--rw-r--r--   0        0        0     5701 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/context.py
--rw-r--r--   0        0        0     9364 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/data.py
--rw-r--r--   0        0        0     1496 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/executable_event.py
--rw-r--r--   0        0        0     4728 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/execution_history.py
--rw-r--r--   0        0        0     8266 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/hooks.py
--rw-r--r--   0        0        0     4209 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/node.py
--rw-r--r--   0        0        0     2796 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/plugin_manager.py
--rw-r--r--   0        0        0    11584 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/process.py
--rw-r--r--   0        0        0     5233 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/schedule.py
--rw-r--r--   0        0        0     1511 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/serializer.py
--rw-r--r--   0        0        0     5964 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/service.py
--rw-r--r--   0        0        0    11516 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/state.py
--rw-r--r--   0        0        0     5848 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/task.py
--rw-r--r--   0        0        0     1762 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/imp/variable.py
--rw-r--r--   0        0        0     2064 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/log.py
--rw-r--r--   0        0        0    10007 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/migrations/0001_initial.py
--rw-r--r--   0        0        0      427 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/migrations/0002_auto_20210322_0233.py
--rw-r--r--   0        0        0      425 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/migrations/0003_logentry_version.py
--rw-r--r--   0        0        0      401 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/migrations/0004_state_inner_loop_.py
--rw-r--r--   0        0        0        0 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/migrations/__init__.py
--rw-r--r--   0        0        0     7840 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/models.py
--rw-r--r--   0        0        0    21326 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/runtime.py
--rw-r--r--   0        0        0      894 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/eri/signals.py
--rw-r--r--   0        0        0     3460 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/exceptions.py
--rw-r--r--   0        0        0     1356 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/__init__.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/admin.py
--rw-r--r--   0        0        0     1042 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/apps.py
--rw-r--r--   0        0        0     1778 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/handlers.py
--rw-r--r--   0        0        0     1487 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/migrations/0001_initial.py
--rw-r--r--   0        0        0     1135 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/migrations/0002_auto_20180810_1054.py
--rw-r--r--   0        0        0     1043 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/migrations/0003_logentry_history_id.py
--rw-r--r--   0        0        0     2343 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/migrations/0004_auto_20180814_1555.py
--rw-r--r--   0        0        0     1125 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/migrations/0005_auto_20190729_1041.py
--rw-r--r--   0        0        0     1182 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/migrations/0006_auto_20201201_1638.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/migrations/__init__.py
--rw-r--r--   0        0        0     2393 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/models.py
--rw-r--r--   0        0        0     1414 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/tasks.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.894749 bamboo-pipeline-3.9.0/pipeline/log/views.py
--rw-r--r--   0        0        0      876 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/logging.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/management/__init__.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/management/commands/__init__.py
--rw-r--r--   0        0        0      916 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/management/commands/app.py
--rw-r--r--   0        0        0     5733 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/management/commands/base.py
--rw-r--r--   0        0        0     1853 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/management/commands/celery.py
--rw-r--r--   0        0        0     1103 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/management/commands/celerybeat.py
--rw-r--r--   0        0        0     4163 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/management/commands/create_atoms_app.py
--rw-r--r--   0        0        0      791 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/management/commands/create_plugins_app.py
--rw-r--r--   0        0        0     2859 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/management/commands/generate_config.py
--rw-r--r--   0        0        0     7748 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0001_initial.py
--rw-r--r--   0        0        0     1640 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0002_auto_20180109_1825.py
--rw-r--r--   0        0        0     2898 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0003_auto_20180206_1955.py
--rw-r--r--   0        0        0     1169 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0004_auto_20180516_1708.py
--rw-r--r--   0        0        0     1371 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0005_pipelineinstance_tree_info.py
--rw-r--r--   0        0        0     1711 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0006_auto_20180814_1622.py
--rw-r--r--   0        0        0     1562 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0007_templaterelationship.py
--rw-r--r--   0        0        0     2104 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0007_templateversion.py
--rw-r--r--   0        0        0     1492 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0008_auto_20180824_1115.py
--rw-r--r--   0        0        0     1801 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0011_auto_20180906_1045.py
--rw-r--r--   0        0        0     1471 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0012_templatecurrentversion.py
--rw-r--r--   0        0        0     2906 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0013_old_template_process.py
--rw-r--r--   0        0        0     1463 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0014_auto_20181127_1053.py
--rw-r--r--   0        0        0     2650 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0015_auto_20181214_1453.py
--rw-r--r--   0        0        0     1308 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0016_auto_20181220_0958.py
--rw-r--r--   0        0        0     1168 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0017_pipelinetemplate_has_subprocess.py
--rw-r--r--   0        0        0     1471 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0018_set_has_subprocess.py
--rw-r--r--   0        0        0      984 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0019_delete_variablemodel.py
--rw-r--r--   0        0        0     1356 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0020_auto_20190906_1119.py
--rw-r--r--   0        0        0     2486 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0021_auto_20190906_1143.py
--rw-r--r--   0        0        0     1198 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0022_pipelineinstance_is_revoked.py
--rw-r--r--   0        0        0     1670 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0023_set_is_revoked.py
--rw-r--r--   0        0        0     2148 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0024_auto_20200213_0738.py
--rw-r--r--   0        0        0      511 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0025_auto_20200813_1216.py
--rw-r--r--   0        0        0      534 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0026_auto_20201028_1049.py
--rw-r--r--   0        0        0      521 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0027_auto_20201123_1552.py
--rw-r--r--   0        0        0      734 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0028_auto_20201227_1952.py
--rw-r--r--   0        0        0      461 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0029_templaterelationship_always_use_latest.py
--rw-r--r--   0        0        0      487 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0030_auto_20210607_1210.py
--rw-r--r--   0        0        0      708 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/0031_auto_20210624_2317.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/migrations/__init__.py
--rw-r--r--   0        0        0    28771 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/models.py
--rw-r--r--   0        0        0      803 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/parser/__init__.py
--rw-r--r--   0        0        0     1692 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/parser/context.py
--rw-r--r--   0        0        0    13629 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/parser/pipeline_parser.py
--rw-r--r--   0        0        0     1835 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/parser/schemas.py
--rw-r--r--   0        0        0     9229 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/parser/utils.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/service/__init__.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/service/pipeline_engine_adapter/__init__.py
--rw-r--r--   0        0        0     5003 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/service/pipeline_engine_adapter/adapter_api.py
--rw-r--r--   0        0        0     2743 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/service/task_service.py
--rw-r--r--   0        0        0      911 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/signals/__init__.py
--rw-r--r--   0        0        0     3302 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/signals/handlers.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/templates/__init__.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/templates/create_plugins_app/__init__.py
--rw-r--r--   0        0        0     1513 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/templates/create_plugins_app/js_file.py
--rw-r--r--   0        0        0     1636 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/templates/create_plugins_app/plugins.py
--rw-r--r--   0        0        0     1725 2021-11-23 09:21:36.898749 bamboo-pipeline-3.9.0/pipeline/templates/create_plugins_app/py_file.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/__init__.py
--rw-r--r--   0        0        0      929 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/boolrule/__init__.py
--rw-r--r--   0        0        0     9062 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/boolrule/boolrule.py
--rw-r--r--   0        0        0     1277 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/collections.py
--rw-r--r--   0        0        0      987 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/crypt.py
--rw-r--r--   0        0        0      816 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/dj.py
--rw-r--r--   0        0        0     1227 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/env.py
--rw-r--r--   0        0        0    15401 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/graph.py
--rw-r--r--   0        0        0     2179 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/http.py
--rw-r--r--   0        0        0      975 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/imoports.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/mako_utils/__init__.py
--rw-r--r--   0        0        0     2358 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/mako_utils/checker.py
--rw-r--r--   0        0        0     1807 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/mako_utils/code_extract.py
--rw-r--r--   0        0        0      810 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/mako_utils/exceptions.py
--rw-r--r--   0        0        0     4177 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/mako_utils/visitors.py
--rw-r--r--   0        0        0     2421 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/register.py
--rw-r--r--   0        0        0     1105 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/uniqid.py
--rw-r--r--   0        0        0     3171 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/utils/utils.py
--rw-r--r--   0        0        0      800 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/validators/__init__.py
--rw-r--r--   0        0        0     1710 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/validators/base.py
--rw-r--r--   0        0        0     2877 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/validators/connection.py
--rw-r--r--   0        0        0    15855 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/validators/gateway.py
--rw-r--r--   0        0        0     1186 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/validators/handlers.py
--rw-r--r--   0        0        0     1993 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/validators/rules.py
--rw-r--r--   0        0        0     2935 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/validators/utils.py
--rw-r--r--   0        0        0      831 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/variable_framework/__init__.py
--rw-r--r--   0        0        0     1018 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/variable_framework/admin.py
--rw-r--r--   0        0        0     2053 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/variable_framework/apps.py
--rw-r--r--   0        0        0     1101 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/variable_framework/context.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/variable_framework/management/__init__.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/variable_framework/management/commands/__init__.py
--rw-r--r--   0        0        0     1000 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/variable_framework/management/commands/update_variable_models.py
--rw-r--r--   0        0        0     1470 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/variable_framework/migrations/0001_initial.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/variable_framework/migrations/__init__.py
--rw-r--r--   0        0        0     1737 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/variable_framework/models.py
--rw-r--r--   0        0        0      750 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/variable_framework/signals/__init__.py
--rw-r--r--   0        0        0     1713 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pipeline/variable_framework/signals/handlers.py
--rw-r--r--   0        0        0     1139 2021-11-23 09:21:36.906749 bamboo-pipeline-3.9.0/pyproject.toml
--rw-r--r--   0        0        0     3166 2021-11-23 09:21:51.473248 bamboo-pipeline-3.9.0/setup.py
--rw-r--r--   0        0        0     1127 2021-11-23 09:21:51.473610 bamboo-pipeline-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/LICENSE
+-rw-r--r--   0        0        0      826 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/__init__.py
+-rw-r--r--   0        0        0     1469 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/admin.py
+-rw-r--r--   0        0        0     3559 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/apps.py
+-rw-r--r--   0        0        0      810 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/builder/__init__.py
+-rw-r--r--   0        0        0     6968 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/builder/builder.py
+-rw-r--r--   0        0        0      871 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/builder/flow/__init__.py
+-rw-r--r--   0        0        0     2479 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/builder/flow/activity.py
+-rw-r--r--   0        0        0     2415 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/builder/flow/base.py
+-rw-r--r--   0        0        0     3009 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/builder/flow/data.py
+-rw-r--r--   0        0        0     1251 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/builder/flow/event.py
+-rw-r--r--   0        0        0     1788 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/builder/flow/gateway.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/celery/__init__.py
+-rw-r--r--   0        0        0     1297 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/celery/queues.py
+-rw-r--r--   0        0        0     6975 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/celery/settings.py
+-rw-r--r--   0        0        0      833 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/component_framework/__init__.py
+-rw-r--r--   0        0        0     1037 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/component_framework/admin.py
+-rw-r--r--   0        0        0     2732 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/component_framework/apps.py
+-rw-r--r--   0        0        0     3971 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/component_framework/base.py
+-rw-r--r--   0        0        0     2685 2021-12-03 08:06:34.902762 bamboo-pipeline-3.9.1/pipeline/component_framework/component.py
+-rw-r--r--   0        0        0     3866 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/constant.py
+-rw-r--r--   0        0        0      785 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/constants.py
+-rw-r--r--   0        0        0     1104 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/context.py
+-rw-r--r--   0        0        0     2626 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/library.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/management/__init__.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/management/commands/__init__.py
+-rw-r--r--   0        0        0     2506 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/management/commands/run_component.py
+-rw-r--r--   0        0        0     1001 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/management/commands/update_component_models.py
+-rw-r--r--   0        0        0     1557 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0001_initial.py
+-rw-r--r--   0        0        0      993 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0002_delete_componentmodel.py
+-rw-r--r--   0        0        0     1694 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0003_componentmodel.py
+-rw-r--r--   0        0        0     1225 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0004_auto_20180413_1800.py
+-rw-r--r--   0        0        0     1409 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0005_auto_20190723_1806.py
+-rw-r--r--   0        0        0      520 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0006_auto_20200213_0743.py
+-rw-r--r--   0        0        0     1523 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0007_auto_20201112_2244.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/__init__.py
+-rw-r--r--   0        0        0     3313 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/models.py
+-rw-r--r--   0        0        0     3597 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/runner.py
+-rw-r--r--   0        0        0    13151 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/component_framework/test.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/components/__init__.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/components/collections/__init__.py
+-rw-r--r--   0        0        0     1697 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/components/collections/examples.py
+-rw-r--r--   0        0        0     1205 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/conf/__init__.py
+-rw-r--r--   0        0        0     4596 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/conf/default_settings.py
+-rw-r--r--   0        0        0      837 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/constants.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/__init__.py
+-rw-r--r--   0        0        0      835 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/__init__.py
+-rw-r--r--   0        0        0     1669 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/admin.py
+-rw-r--r--   0        0        0     2746 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/apps.py
+-rw-r--r--   0        0        0      805 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/exceptions.py
+-rw-r--r--   0        0        0     1633 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/loader.py
+-rw-r--r--   0        0        0     4333 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/migrations/0001_initial.py
+-rw-r--r--   0        0        0      465 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/migrations/0002_s3source_source_dir.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/migrations/__init__.py
+-rw-r--r--   0        0        0      906 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/models/__init__.py
+-rw-r--r--   0        0        0     5337 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/models/base.py
+-rw-r--r--   0        0        0     1253 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/models/fields.py
+-rw-r--r--   0        0        0     1299 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/models/forms.py
+-rw-r--r--   0        0        0     3271 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/models/source.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/__init__.py
+-rw-r--r--   0        0        0     1116 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/importer/__init__.py
+-rw-r--r--   0        0        0     6635 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/importer/base.py
+-rw-r--r--   0        0        0     3201 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/importer/fs.py
+-rw-r--r--   0        0        0     3502 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/importer/git.py
+-rw-r--r--   0        0        0     4391 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/importer/s3.py
+-rw-r--r--   0        0        0     1430 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/importer/utils.py
+-rw-r--r--   0        0        0     1024 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/requirement.py
+-rw-r--r--   0        0        0      829 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/__init__.py
+-rw-r--r--   0        0        0     1371 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/admin.py
+-rw-r--r--   0        0        0     1034 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/apps.py
+-rw-r--r--   0        0        0     1353 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/context.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/__init__.py
+-rw-r--r--   0        0        0     1341 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/compat.py
+-rw-r--r--   0        0        0     2796 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/db.py
+-rw-r--r--   0        0        0     7118 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/managers.py
+-rw-r--r--   0        0        0     3689 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/migrate.py
+-rw-r--r--   0        0        0     8361 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/models.py
+-rw-r--r--   0        0        0     4112 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/tzcrontab.py
+-rw-r--r--   0        0        0     1344 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/utils.py
+-rw-r--r--   0        0        0    10344 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1136 2021-12-03 08:06:34.906762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/0002_auto_20190103_1918.py
+-rw-r--r--   0        0        0     3390 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/0003_auto_20191213_0819.py
+-rw-r--r--   0        0        0      721 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/0004_auto_20191213_0828.py
+-rw-r--r--   0        0        0      523 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/0005_migrate_task.py
+-rw-r--r--   0        0        0      632 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/0006_change_task_ref_table.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/__init__.py
+-rw-r--r--   0        0        0     7856 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/models.py
+-rw-r--r--   0        0        0     1045 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/signals/__init__.py
+-rw-r--r--   0        0        0     6794 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/tasks.py
+-rw-r--r--   0        0        0     4090 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/tests.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/views.py
+-rw-r--r--   0        0        0      824 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/__init__.py
+-rw-r--r--   0        0        0     2324 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/admin.py
+-rw-r--r--   0        0        0     1097 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/apps.py
+-rw-r--r--   0        0        0     4178 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1044 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0002_auto_20180817_1212.py
+-rw-r--r--   0        0        0     1510 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0003_auto_20180821_2015.py
+-rw-r--r--   0        0        0     2849 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0004_instanceinpipeline_templateinpipeline.py
+-rw-r--r--   0        0        0      908 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0005_init_pipeline_data.py
+-rw-r--r--   0        0        0     1389 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0006_auto_20181115_1208.py
+-rw-r--r--   0        0        0     3123 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0007_init_pipeline_data.py
+-rw-r--r--   0        0        0     2563 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0008_auto_20181116_1448.py
+-rw-r--r--   0        0        0     1828 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0009_auto_20181116_1627.py
+-rw-r--r--   0        0        0     2857 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0010_auto_20190304_1747.py
+-rw-r--r--   0        0        0     1212 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0011_auto_20200217_0822.py
+-rw-r--r--   0        0        0      724 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0012_auto_20201123_1552.py
+-rw-r--r--   0        0        0      734 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0013_auto_20201201_1506.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/__init__.py
+-rw-r--r--   0        0        0     4080 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/models.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/signals/__init__.py
+-rw-r--r--   0        0        0     5006 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/signals/handlers.py
+-rw-r--r--   0        0        0     7773 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/tasks.py
+-rw-r--r--   0        0        0     1184 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/contrib/statistics/utils.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/__init__.py
+-rw-r--r--   0        0        0     2781 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/constants.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/data/__init__.py
+-rw-r--r--   0        0        0     3109 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/data/base.py
+-rw-r--r--   0        0        0     5375 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/data/context.py
+-rw-r--r--   0        0        0     1641 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/data/converter.py
+-rw-r--r--   0        0        0     6055 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/data/expression.py
+-rw-r--r--   0        0        0     1640 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/data/hydration.py
+-rw-r--r--   0        0        0     1131 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/data/library.py
+-rw-r--r--   0        0        0     2103 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/data/mako_safety.py
+-rw-r--r--   0        0        0     2536 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/data/sandbox.py
+-rw-r--r--   0        0        0      910 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/data/schemas.py
+-rw-r--r--   0        0        0     5002 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/data/var.py
+-rw-r--r--   0        0        0     3012 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/flow/__init__.py
+-rw-r--r--   0        0        0     1001 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/flow/activity/__init__.py
+-rw-r--r--   0        0        0     1432 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/flow/activity/base.py
+-rw-r--r--   0        0        0     8859 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/flow/activity/service_activity.py
+-rw-r--r--   0        0        0     1849 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/flow/activity/subprocess.py
+-rw-r--r--   0        0        0     5219 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/flow/base.py
+-rw-r--r--   0        0        0     1966 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/flow/event.py
+-rw-r--r--   0        0        0     7271 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/flow/gateway.py
+-rw-r--r--   0        0        0     3847 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/flow/io.py
+-rw-r--r--   0        0        0      866 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/flow/signals.py
+-rw-r--r--   0        0        0     4266 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/pipeline.py
+-rw-r--r--   0        0        0      852 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/core/signals/__init__.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/django_signal_valve/__init__.py
+-rw-r--r--   0        0        0     1012 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/django_signal_valve/admin.py
+-rw-r--r--   0        0        0     1465 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/django_signal_valve/migrations/0001_initial.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/django_signal_valve/migrations/__init__.py
+-rw-r--r--   0        0        0     1885 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/django_signal_valve/models.py
+-rw-r--r--   0        0        0     2119 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/django_signal_valve/valve.py
+-rw-r--r--   0        0        0      807 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/__init__.py
+-rw-r--r--   0        0        0     5392 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/admin.py
+-rw-r--r--   0        0        0    19655 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/api.py
+-rw-r--r--   0        0        0     1210 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/apps.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/conf/__init__.py
+-rw-r--r--   0        0        0     1048 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/conf/function_switch.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/__init__.py
+-rw-r--r--   0        0        0     3819 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/api.py
+-rw-r--r--   0        0        0     1123 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/context.py
+-rw-r--r--   0        0        0      803 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/data/__init__.py
+-rw-r--r--   0        0        0     4149 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/data/api.py
+-rw-r--r--   0        0        0     1304 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/data/base_backend.py
+-rw-r--r--   0        0        0     1369 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/data/mysql_backend.py
+-rw-r--r--   0        0        0     1785 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/data/redis_backend.py
+-rw-r--r--   0        0        0     2463 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/__init__.py
+-rw-r--r--   0        0        0     1496 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/base.py
+-rw-r--r--   0        0        0     2540 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/conditional_parallel.py
+-rw-r--r--   0        0        0     1956 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/converge_gateway.py
+-rw-r--r--   0        0        0     1854 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/empty_start_event.py
+-rw-r--r--   0        0        0      877 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/endevent/__init__.py
+-rw-r--r--   0        0        0     2570 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/endevent/base.py
+-rw-r--r--   0        0        0      954 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/endevent/empty_end_event.py
+-rw-r--r--   0        0        0     1748 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/endevent/executable_end_event.py
+-rw-r--r--   0        0        0     2157 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/exclusive_gateway.py
+-rw-r--r--   0        0        0     1994 2021-12-03 08:06:34.910762 bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/parallel_gateway.py
+-rw-r--r--   0        0        0     6166 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/service_activity.py
+-rw-r--r--   0        0        0     2145 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/subprocess.py
+-rw-r--r--   0        0        0     5588 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/core/runtime.py
+-rw-r--r--   0        0        0    11133 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/core/schedule.py
+-rw-r--r--   0        0        0     1461 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/exceptions.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/health/__init__.py
+-rw-r--r--   0        0        0      817 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/health/zombie/__init__.py
+-rw-r--r--   0        0        0     5158 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/health/zombie/doctors.py
+-rw-r--r--   0        0        0     2420 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/health/zombie/heal.py
+-rw-r--r--   0        0        0      849 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/logging.py
+-rw-r--r--   0        0        0    10805 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1210 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0002_auto_20180109_1825.py
+-rw-r--r--   0        0        0     2850 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0003_auto_20180717_1148.py
+-rw-r--r--   0        0        0     1041 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0004_auto_20180717_1411.py
+-rw-r--r--   0        0        0     1148 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0005_auto_20180717_1433.py
+-rw-r--r--   0        0        0     1149 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0006_auto_20180717_1543.py
+-rw-r--r--   0        0        0     1270 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0007_auto_20180717_2022.py
+-rw-r--r--   0        0        0     1470 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0008_schedulecelerytask.py
+-rw-r--r--   0        0        0     1199 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0009_status_error_ignorable.py
+-rw-r--r--   0        0        0     1217 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0010_auto_20180830_1203.py
+-rw-r--r--   0        0        0     1466 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0010_nodecelerytask.py
+-rw-r--r--   0        0        0     1209 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0011_auto_20180830_1205.py
+-rw-r--r--   0        0        0     1447 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0015_datasnapshot.py
+-rw-r--r--   0        0        0     1313 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0016_auto_20181228_0345.py
+-rw-r--r--   0        0        0     1158 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0017_auto_20190719_1010.py
+-rw-r--r--   0        0        0     3113 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0018_auto_20190729_1041.py
+-rw-r--r--   0        0        0     1441 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0019_auto_20190729_1044.py
+-rw-r--r--   0        0        0      467 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0020_pipelinemodel_priority.py
+-rw-r--r--   0        0        0     2710 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0021_auto_20191213_0725.py
+-rw-r--r--   0        0        0      518 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0022_scheduleservice_multi_callback_enabled.py
+-rw-r--r--   0        0        0      523 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0023_status_state_refresh_at.py
+-rw-r--r--   0        0        0     1558 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0024_auto_20200224_0308.py
+-rw-r--r--   0        0        0      748 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0025_multicallbackdata.py
+-rw-r--r--   0        0        0     1551 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0026_auto_20200610_1442.py
+-rw-r--r--   0        0        0     1520 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0027_sendfailedcelerytask.py
+-rw-r--r--   0        0        0      462 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/0028_auto_20210812_0906.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/migrations/__init__.py
+-rw-r--r--   0        0        0      905 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/models/__init__.py
+-rw-r--r--   0        0        0    51167 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/models/core.py
+-rw-r--r--   0        0        0     1788 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/models/data.py
+-rw-r--r--   0        0        0     1984 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/models/fields.py
+-rw-r--r--   0        0        0     2368 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/models/function.py
+-rw-r--r--   0        0        0    55112 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/models/nr_pickle.py
+-rw-r--r--   0        0        0     2115 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/signals/__init__.py
+-rw-r--r--   0        0        0     3791 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/signals/dispatch.py
+-rw-r--r--   0        0        0     5836 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/signals/handlers.py
+-rw-r--r--   0        0        0     3209 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/states.py
+-rw-r--r--   0        0        0    13579 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/tasks.py
+-rw-r--r--   0        0        0     2043 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/engine/utils.py
+-rw-r--r--   0        0        0      801 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/__init__.py
+-rw-r--r--   0        0        0     3267 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/admin.py
+-rw-r--r--   0        0        0     1055 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/apps.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/celery/__init__.py
+-rw-r--r--   0        0        0     2196 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/celery/queues.py
+-rw-r--r--   0        0        0     1030 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/celery/step.py
+-rw-r--r--   0        0        0     1893 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/celery/tasks.py
+-rw-r--r--   0        0        0     1659 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/codec.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/__init__.py
+-rw-r--r--   0        0        0     5701 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/context.py
+-rw-r--r--   0        0        0     9364 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/data.py
+-rw-r--r--   0        0        0     1496 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/executable_event.py
+-rw-r--r--   0        0        0     4728 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/execution_history.py
+-rw-r--r--   0        0        0     8266 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/hooks.py
+-rw-r--r--   0        0        0     4209 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/node.py
+-rw-r--r--   0        0        0     2796 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/plugin_manager.py
+-rw-r--r--   0        0        0    11584 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/process.py
+-rw-r--r--   0        0        0     5233 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/schedule.py
+-rw-r--r--   0        0        0     1511 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/serializer.py
+-rw-r--r--   0        0        0     5964 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/service.py
+-rw-r--r--   0        0        0    11516 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/state.py
+-rw-r--r--   0        0        0     5848 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/task.py
+-rw-r--r--   0        0        0     1762 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/imp/variable.py
+-rw-r--r--   0        0        0     2064 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/log.py
+-rw-r--r--   0        0        0    10007 2021-12-03 08:06:34.914762 bamboo-pipeline-3.9.1/pipeline/eri/migrations/0001_initial.py
+-rw-r--r--   0        0        0      427 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/eri/migrations/0002_auto_20210322_0233.py
+-rw-r--r--   0        0        0      425 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/eri/migrations/0003_logentry_version.py
+-rw-r--r--   0        0        0      401 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/eri/migrations/0004_state_inner_loop_.py
+-rw-r--r--   0        0        0        0 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/eri/migrations/__init__.py
+-rw-r--r--   0        0        0     7840 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/eri/models.py
+-rw-r--r--   0        0        0    21326 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/eri/runtime.py
+-rw-r--r--   0        0        0      894 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/eri/signals.py
+-rw-r--r--   0        0        0     3460 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/exceptions.py
+-rw-r--r--   0        0        0     1356 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/__init__.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/admin.py
+-rw-r--r--   0        0        0     1042 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/apps.py
+-rw-r--r--   0        0        0     1778 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/handlers.py
+-rw-r--r--   0        0        0     1487 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1135 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/migrations/0002_auto_20180810_1054.py
+-rw-r--r--   0        0        0     1043 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/migrations/0003_logentry_history_id.py
+-rw-r--r--   0        0        0     2343 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/migrations/0004_auto_20180814_1555.py
+-rw-r--r--   0        0        0     1125 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/migrations/0005_auto_20190729_1041.py
+-rw-r--r--   0        0        0     1182 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/migrations/0006_auto_20201201_1638.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/migrations/__init__.py
+-rw-r--r--   0        0        0     2393 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/models.py
+-rw-r--r--   0        0        0     1414 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/tasks.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/log/views.py
+-rw-r--r--   0        0        0      876 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/logging.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/management/__init__.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/management/commands/__init__.py
+-rw-r--r--   0        0        0      916 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/management/commands/app.py
+-rw-r--r--   0        0        0     5733 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/management/commands/base.py
+-rw-r--r--   0        0        0     1853 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/management/commands/celery.py
+-rw-r--r--   0        0        0     1103 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/management/commands/celerybeat.py
+-rw-r--r--   0        0        0     4163 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/management/commands/create_atoms_app.py
+-rw-r--r--   0        0        0      791 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/management/commands/create_plugins_app.py
+-rw-r--r--   0        0        0     2859 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/management/commands/generate_config.py
+-rw-r--r--   0        0        0     7748 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1640 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0002_auto_20180109_1825.py
+-rw-r--r--   0        0        0     2898 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0003_auto_20180206_1955.py
+-rw-r--r--   0        0        0     1169 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0004_auto_20180516_1708.py
+-rw-r--r--   0        0        0     1371 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0005_pipelineinstance_tree_info.py
+-rw-r--r--   0        0        0     1711 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0006_auto_20180814_1622.py
+-rw-r--r--   0        0        0     1562 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0007_templaterelationship.py
+-rw-r--r--   0        0        0     2104 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0007_templateversion.py
+-rw-r--r--   0        0        0     1492 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0008_auto_20180824_1115.py
+-rw-r--r--   0        0        0     1801 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0011_auto_20180906_1045.py
+-rw-r--r--   0        0        0     1471 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0012_templatecurrentversion.py
+-rw-r--r--   0        0        0     2906 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0013_old_template_process.py
+-rw-r--r--   0        0        0     1463 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0014_auto_20181127_1053.py
+-rw-r--r--   0        0        0     2650 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0015_auto_20181214_1453.py
+-rw-r--r--   0        0        0     1308 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0016_auto_20181220_0958.py
+-rw-r--r--   0        0        0     1168 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0017_pipelinetemplate_has_subprocess.py
+-rw-r--r--   0        0        0     1471 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0018_set_has_subprocess.py
+-rw-r--r--   0        0        0      984 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0019_delete_variablemodel.py
+-rw-r--r--   0        0        0     1356 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0020_auto_20190906_1119.py
+-rw-r--r--   0        0        0     2486 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0021_auto_20190906_1143.py
+-rw-r--r--   0        0        0     1198 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0022_pipelineinstance_is_revoked.py
+-rw-r--r--   0        0        0     1670 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0023_set_is_revoked.py
+-rw-r--r--   0        0        0     2148 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0024_auto_20200213_0738.py
+-rw-r--r--   0        0        0      511 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0025_auto_20200813_1216.py
+-rw-r--r--   0        0        0      534 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0026_auto_20201028_1049.py
+-rw-r--r--   0        0        0      521 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0027_auto_20201123_1552.py
+-rw-r--r--   0        0        0      734 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0028_auto_20201227_1952.py
+-rw-r--r--   0        0        0      461 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0029_templaterelationship_always_use_latest.py
+-rw-r--r--   0        0        0      487 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0030_auto_20210607_1210.py
+-rw-r--r--   0        0        0      708 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/0031_auto_20210624_2317.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/migrations/__init__.py
+-rw-r--r--   0        0        0    28771 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/models.py
+-rw-r--r--   0        0        0      803 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/parser/__init__.py
+-rw-r--r--   0        0        0     1692 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/parser/context.py
+-rw-r--r--   0        0        0    13629 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/parser/pipeline_parser.py
+-rw-r--r--   0        0        0     1835 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/parser/schemas.py
+-rw-r--r--   0        0        0     9229 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/parser/utils.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/service/__init__.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/service/pipeline_engine_adapter/__init__.py
+-rw-r--r--   0        0        0     5003 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/service/pipeline_engine_adapter/adapter_api.py
+-rw-r--r--   0        0        0     2743 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/service/task_service.py
+-rw-r--r--   0        0        0      911 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/signals/__init__.py
+-rw-r--r--   0        0        0     3302 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/signals/handlers.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/templates/__init__.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/templates/create_plugins_app/__init__.py
+-rw-r--r--   0        0        0     1513 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/templates/create_plugins_app/js_file.py
+-rw-r--r--   0        0        0     1636 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/templates/create_plugins_app/plugins.py
+-rw-r--r--   0        0        0     1725 2021-12-03 08:06:34.918763 bamboo-pipeline-3.9.1/pipeline/templates/create_plugins_app/py_file.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/__init__.py
+-rw-r--r--   0        0        0      929 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/boolrule/__init__.py
+-rw-r--r--   0        0        0     9062 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/boolrule/boolrule.py
+-rw-r--r--   0        0        0     1277 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/collections.py
+-rw-r--r--   0        0        0      987 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/crypt.py
+-rw-r--r--   0        0        0      816 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/dj.py
+-rw-r--r--   0        0        0     1227 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/env.py
+-rw-r--r--   0        0        0    15401 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/graph.py
+-rw-r--r--   0        0        0     2179 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/http.py
+-rw-r--r--   0        0        0      975 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/imoports.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/mako_utils/__init__.py
+-rw-r--r--   0        0        0     2358 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/mako_utils/checker.py
+-rw-r--r--   0        0        0     1807 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/mako_utils/code_extract.py
+-rw-r--r--   0        0        0      810 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/mako_utils/exceptions.py
+-rw-r--r--   0        0        0     4177 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/mako_utils/visitors.py
+-rw-r--r--   0        0        0     2421 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/register.py
+-rw-r--r--   0        0        0     1105 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/uniqid.py
+-rw-r--r--   0        0        0     3171 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/utils/utils.py
+-rw-r--r--   0        0        0      800 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/validators/__init__.py
+-rw-r--r--   0        0        0     1710 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/validators/base.py
+-rw-r--r--   0        0        0     2877 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/validators/connection.py
+-rw-r--r--   0        0        0    15855 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/validators/gateway.py
+-rw-r--r--   0        0        0     1186 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/validators/handlers.py
+-rw-r--r--   0        0        0     1993 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/validators/rules.py
+-rw-r--r--   0        0        0     2935 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/validators/utils.py
+-rw-r--r--   0        0        0      831 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/variable_framework/__init__.py
+-rw-r--r--   0        0        0     1018 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/variable_framework/admin.py
+-rw-r--r--   0        0        0     2053 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/variable_framework/apps.py
+-rw-r--r--   0        0        0     1101 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/variable_framework/context.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/variable_framework/management/__init__.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/variable_framework/management/commands/__init__.py
+-rw-r--r--   0        0        0     1000 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/variable_framework/management/commands/update_variable_models.py
+-rw-r--r--   0        0        0     1470 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/variable_framework/migrations/0001_initial.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/variable_framework/migrations/__init__.py
+-rw-r--r--   0        0        0     1737 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/variable_framework/models.py
+-rw-r--r--   0        0        0      750 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/variable_framework/signals/__init__.py
+-rw-r--r--   0        0        0     1713 2021-12-03 08:06:34.926763 bamboo-pipeline-3.9.1/pipeline/variable_framework/signals/handlers.py
+-rw-r--r--   0        0        0     1139 2021-12-03 08:06:34.930763 bamboo-pipeline-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3166 2021-12-03 08:06:50.030454 bamboo-pipeline-3.9.1/setup.py
+-rw-r--r--   0        0        0     1127 2021-12-03 08:06:50.030875 bamboo-pipeline-3.9.1/PKG-INFO
```

### Comparing `bamboo-pipeline-3.9.0/LICENSE` & `bamboo-pipeline-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/admin.py` & `bamboo-pipeline-3.9.1/pipeline/admin.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/apps.py` & `bamboo-pipeline-3.9.1/pipeline/apps.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/builder/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/builder/builder.py` & `bamboo-pipeline-3.9.1/pipeline/builder/builder.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/builder/flow/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/builder/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/builder/flow/activity.py` & `bamboo-pipeline-3.9.1/pipeline/builder/flow/activity.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/builder/flow/base.py` & `bamboo-pipeline-3.9.1/pipeline/builder/flow/base.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/builder/flow/data.py` & `bamboo-pipeline-3.9.1/pipeline/builder/flow/data.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/builder/flow/event.py` & `bamboo-pipeline-3.9.1/pipeline/builder/flow/event.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/builder/flow/gateway.py` & `bamboo-pipeline-3.9.1/pipeline/builder/flow/gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/celery/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/celery/queues.py` & `bamboo-pipeline-3.9.1/pipeline/celery/queues.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/celery/settings.py` & `bamboo-pipeline-3.9.1/pipeline/celery/settings.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/admin.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/admin.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/apps.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/apps.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/base.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/base.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/component.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/component.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/constant.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/constant.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/constants.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/constants.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/context.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/context.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/library.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/library.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/management/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/management/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/management/commands/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/management/commands/run_component.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/management/commands/run_component.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/management/commands/update_component_models.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/management/commands/update_component_models.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0001_initial.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0002_delete_componentmodel.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0002_delete_componentmodel.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0003_componentmodel.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0003_componentmodel.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0004_auto_20180413_1800.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0004_auto_20180413_1800.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0005_auto_20190723_1806.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0005_auto_20190723_1806.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0006_auto_20200213_0743.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0006_auto_20200213_0743.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/0007_auto_20201112_2244.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/0007_auto_20201112_2244.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/migrations/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/models.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/models.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/runner.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/runner.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/component_framework/test.py` & `bamboo-pipeline-3.9.1/pipeline/component_framework/test.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/components/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/components/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/components/collections/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/components/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/components/collections/examples.py` & `bamboo-pipeline-3.9.1/pipeline/components/collections/examples.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/conf/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/conf/default_settings.py` & `bamboo-pipeline-3.9.1/pipeline/conf/default_settings.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/constants.py` & `bamboo-pipeline-3.9.1/pipeline/constants.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/admin.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/admin.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/apps.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/apps.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/exceptions.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/exceptions.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/loader.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/loader.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/migrations/0001_initial.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/migrations/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/models/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/models/base.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/models/base.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/models/fields.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/models/fields.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/models/forms.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/models/forms.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/models/source.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/models/source.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/importer/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/importer/base.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/importer/base.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/importer/fs.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/importer/fs.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/importer/git.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/importer/git.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/importer/s3.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/importer/s3.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/importer/utils.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/importer/utils.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/external_plugins/utils/requirement.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/external_plugins/utils/requirement.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/admin.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/admin.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/apps.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/apps.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/context.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/context.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/compat.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/compat.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/db.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/db.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/managers.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/managers.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/migrate.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/migrate.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/models.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/models.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/tzcrontab.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/tzcrontab.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/djcelery/utils.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/djcelery/utils.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/0001_initial.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/0002_auto_20190103_1918.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/0002_auto_20190103_1918.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/0003_auto_20191213_0819.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/0003_auto_20191213_0819.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/0004_auto_20191213_0828.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/0004_auto_20191213_0828.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/0005_migrate_task.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/0005_migrate_task.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/0006_change_task_ref_table.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/0006_change_task_ref_table.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/migrations/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/models.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/models.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/signals/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/tasks.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/tasks.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/tests.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/tests.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/periodic_task/views.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/periodic_task/views.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/admin.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/admin.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/apps.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/apps.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0001_initial.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0002_auto_20180817_1212.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0002_auto_20180817_1212.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0003_auto_20180821_2015.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0003_auto_20180821_2015.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0004_instanceinpipeline_templateinpipeline.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0004_instanceinpipeline_templateinpipeline.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0005_init_pipeline_data.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0005_init_pipeline_data.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0006_auto_20181115_1208.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0006_auto_20181115_1208.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0007_init_pipeline_data.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0007_init_pipeline_data.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0008_auto_20181116_1448.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0008_auto_20181116_1448.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0009_auto_20181116_1627.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0009_auto_20181116_1627.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0010_auto_20190304_1747.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0010_auto_20190304_1747.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0011_auto_20200217_0822.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0011_auto_20200217_0822.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0012_auto_20201123_1552.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0012_auto_20201123_1552.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/0013_auto_20201201_1506.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/0013_auto_20201201_1506.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/migrations/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/models.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/models.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/signals/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/signals/handlers.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/tasks.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/tasks.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/contrib/statistics/utils.py` & `bamboo-pipeline-3.9.1/pipeline/contrib/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/constants.py` & `bamboo-pipeline-3.9.1/pipeline/core/constants.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/data/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/data/base.py` & `bamboo-pipeline-3.9.1/pipeline/core/data/base.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/data/context.py` & `bamboo-pipeline-3.9.1/pipeline/core/data/context.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/data/converter.py` & `bamboo-pipeline-3.9.1/pipeline/core/data/converter.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/data/expression.py` & `bamboo-pipeline-3.9.1/pipeline/core/data/expression.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/data/hydration.py` & `bamboo-pipeline-3.9.1/pipeline/core/data/hydration.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/data/library.py` & `bamboo-pipeline-3.9.1/pipeline/core/data/library.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/data/mako_safety.py` & `bamboo-pipeline-3.9.1/pipeline/core/data/mako_safety.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/data/sandbox.py` & `bamboo-pipeline-3.9.1/pipeline/core/data/sandbox.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/data/schemas.py` & `bamboo-pipeline-3.9.1/pipeline/core/data/schemas.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/data/var.py` & `bamboo-pipeline-3.9.1/pipeline/core/data/var.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/flow/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/core/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/flow/activity/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/core/flow/activity/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/flow/activity/base.py` & `bamboo-pipeline-3.9.1/pipeline/core/flow/activity/base.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/flow/activity/service_activity.py` & `bamboo-pipeline-3.9.1/pipeline/core/flow/activity/service_activity.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/flow/activity/subprocess.py` & `bamboo-pipeline-3.9.1/pipeline/core/flow/activity/subprocess.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/flow/base.py` & `bamboo-pipeline-3.9.1/pipeline/core/flow/base.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/flow/event.py` & `bamboo-pipeline-3.9.1/pipeline/core/flow/event.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/flow/gateway.py` & `bamboo-pipeline-3.9.1/pipeline/core/flow/gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/flow/io.py` & `bamboo-pipeline-3.9.1/pipeline/core/flow/io.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/flow/signals.py` & `bamboo-pipeline-3.9.1/pipeline/core/flow/signals.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/pipeline.py` & `bamboo-pipeline-3.9.1/pipeline/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/core/signals/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/core/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/django_signal_valve/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/django_signal_valve/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/django_signal_valve/admin.py` & `bamboo-pipeline-3.9.1/pipeline/django_signal_valve/admin.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/django_signal_valve/migrations/0001_initial.py` & `bamboo-pipeline-3.9.1/pipeline/django_signal_valve/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/django_signal_valve/migrations/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/django_signal_valve/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/django_signal_valve/models.py` & `bamboo-pipeline-3.9.1/pipeline/django_signal_valve/models.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/django_signal_valve/valve.py` & `bamboo-pipeline-3.9.1/pipeline/django_signal_valve/valve.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/admin.py` & `bamboo-pipeline-3.9.1/pipeline/engine/admin.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/api.py` & `bamboo-pipeline-3.9.1/pipeline/engine/api.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/apps.py` & `bamboo-pipeline-3.9.1/pipeline/engine/apps.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/conf/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/engine/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/conf/function_switch.py` & `bamboo-pipeline-3.9.1/pipeline/engine/conf/function_switch.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/api.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/api.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/context.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/context.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/data/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/data/api.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/data/api.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/data/base_backend.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/data/base_backend.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/data/mysql_backend.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/data/mysql_backend.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/data/redis_backend.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/data/redis_backend.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/base.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/base.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/conditional_parallel.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/conditional_parallel.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/converge_gateway.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/converge_gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/empty_start_event.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/empty_start_event.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/endevent/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/endevent/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/endevent/base.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/endevent/base.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/endevent/empty_end_event.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/endevent/empty_end_event.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/endevent/executable_end_event.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/endevent/executable_end_event.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/exclusive_gateway.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/exclusive_gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/parallel_gateway.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/parallel_gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/service_activity.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/service_activity.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/handlers/subprocess.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/handlers/subprocess.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/runtime.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/runtime.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/core/schedule.py` & `bamboo-pipeline-3.9.1/pipeline/engine/core/schedule.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/exceptions.py` & `bamboo-pipeline-3.9.1/pipeline/engine/exceptions.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/health/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/engine/health/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/health/zombie/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/engine/health/zombie/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/health/zombie/doctors.py` & `bamboo-pipeline-3.9.1/pipeline/engine/health/zombie/doctors.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/health/zombie/heal.py` & `bamboo-pipeline-3.9.1/pipeline/engine/health/zombie/heal.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/logging.py` & `bamboo-pipeline-3.9.1/pipeline/engine/logging.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0001_initial.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0002_auto_20180109_1825.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0002_auto_20180109_1825.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0003_auto_20180717_1148.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0003_auto_20180717_1148.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0004_auto_20180717_1411.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0004_auto_20180717_1411.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0005_auto_20180717_1433.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0005_auto_20180717_1433.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0006_auto_20180717_1543.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0006_auto_20180717_1543.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0007_auto_20180717_2022.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0007_auto_20180717_2022.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0008_schedulecelerytask.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0008_schedulecelerytask.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0009_status_error_ignorable.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0009_status_error_ignorable.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0010_auto_20180830_1203.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0010_auto_20180830_1203.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0010_nodecelerytask.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0010_nodecelerytask.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0011_auto_20180830_1205.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0011_auto_20180830_1205.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0015_datasnapshot.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0015_datasnapshot.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0016_auto_20181228_0345.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0016_auto_20181228_0345.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0017_auto_20190719_1010.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0017_auto_20190719_1010.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0018_auto_20190729_1041.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0018_auto_20190729_1041.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0019_auto_20190729_1044.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0019_auto_20190729_1044.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0021_auto_20191213_0725.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0021_auto_20191213_0725.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0022_scheduleservice_multi_callback_enabled.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0022_scheduleservice_multi_callback_enabled.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0023_status_state_refresh_at.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0023_status_state_refresh_at.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0024_auto_20200224_0308.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0024_auto_20200224_0308.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0025_multicallbackdata.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0025_multicallbackdata.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0026_auto_20200610_1442.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0026_auto_20200610_1442.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/0027_sendfailedcelerytask.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/0027_sendfailedcelerytask.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/migrations/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/engine/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/models/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/engine/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/models/core.py` & `bamboo-pipeline-3.9.1/pipeline/engine/models/core.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/models/data.py` & `bamboo-pipeline-3.9.1/pipeline/engine/models/data.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/models/fields.py` & `bamboo-pipeline-3.9.1/pipeline/engine/models/fields.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/models/function.py` & `bamboo-pipeline-3.9.1/pipeline/engine/models/function.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/models/nr_pickle.py` & `bamboo-pipeline-3.9.1/pipeline/engine/models/nr_pickle.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/signals/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/engine/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/signals/dispatch.py` & `bamboo-pipeline-3.9.1/pipeline/engine/signals/dispatch.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/signals/handlers.py` & `bamboo-pipeline-3.9.1/pipeline/engine/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/states.py` & `bamboo-pipeline-3.9.1/pipeline/engine/states.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/tasks.py` & `bamboo-pipeline-3.9.1/pipeline/engine/tasks.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/engine/utils.py` & `bamboo-pipeline-3.9.1/pipeline/engine/utils.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/eri/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/admin.py` & `bamboo-pipeline-3.9.1/pipeline/eri/admin.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,21 +14,32 @@
 from django.contrib import admin
 
 from pipeline.eri import models
 
 
 @admin.register(models.Process)
 class ProcessAdmin(admin.ModelAdmin):
-    list_display = ["id", "parent_id", "ack_num", "need_ack", "asleep", "suspended", "frozen", "dead"]
-    search_fields = ["id___exact", "parent_id____exact", "current_node_id____exact", "suspended_by____exact"]
+    list_display = [
+        "id",
+        "parent_id",
+        "ack_num",
+        "need_ack",
+        "asleep",
+        "suspended",
+        "frozen",
+        "dead",
+        "root_pipeline_id",
+        "current_node_id",
+    ]
+    search_fields = ["root_pipeline_id__exact", "current_node_id__exact", "suspended_by__exact"]
 
 
 @admin.register(models.Node)
 class NodeAdmin(admin.ModelAdmin):
-    list_display = ["id", "node_id"]
+    list_display = ["id", "node_id", "detail"]
     search_fields = ["node_id__exact"]
 
 
 @admin.register(models.State)
 class StateAdmin(admin.ModelAdmin):
     list_display = [
         "id",
@@ -44,26 +55,26 @@
     ]
     search_fields = ["node_id__exact", "root_id__exact", "parent_id__exact"]
 
 
 @admin.register(models.Schedule)
 class ScheduleAdmin(admin.ModelAdmin):
     list_display = ["id", "type", "process_id", "node_id", "finished", "expired", "version", "schedule_times"]
-    search_fields = ["id__exact", "node_id__exact"]
+    search_fields = ["node_id__exact"]
 
 
 @admin.register(models.Data)
 class DataAdmin(admin.ModelAdmin):
-    list_display = ["id", "node_id"]
+    list_display = ["id", "node_id", "inputs", "outputs"]
     search_fields = ["node_id__exact"]
 
 
 @admin.register(models.ExecutionData)
 class ExecutionDataAdmin(admin.ModelAdmin):
-    list_display = ["id", "node_id"]
+    list_display = ["id", "node_id", "inputs", "outputs"]
     search_fields = ["node_id__exact"]
 
 
 @admin.register(models.CallbackData)
 class CallbackDataAdmin(admin.ModelAdmin):
     list_display = ["id", "node_id", "version", "data"]
     search_fields = ["id__exact"]
```

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/apps.py` & `bamboo-pipeline-3.9.1/pipeline/eri/apps.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/celery/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/eri/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/celery/queues.py` & `bamboo-pipeline-3.9.1/pipeline/eri/celery/queues.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/celery/step.py` & `bamboo-pipeline-3.9.1/pipeline/eri/celery/step.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/celery/tasks.py` & `bamboo-pipeline-3.9.1/pipeline/eri/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/codec.py` & `bamboo-pipeline-3.9.1/pipeline/eri/codec.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/context.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/context.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/data.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/data.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/executable_event.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/executable_event.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/execution_history.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/execution_history.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/hooks.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/hooks.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/node.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/node.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/plugin_manager.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/process.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/process.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/schedule.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/schedule.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/serializer.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/serializer.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/service.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/service.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/state.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/state.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/task.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/task.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/imp/variable.py` & `bamboo-pipeline-3.9.1/pipeline/eri/imp/variable.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/log.py` & `bamboo-pipeline-3.9.1/pipeline/eri/log.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/migrations/0001_initial.py` & `bamboo-pipeline-3.9.1/pipeline/eri/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/models.py` & `bamboo-pipeline-3.9.1/pipeline/eri/models.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/runtime.py` & `bamboo-pipeline-3.9.1/pipeline/eri/runtime.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/eri/signals.py` & `bamboo-pipeline-3.9.1/pipeline/eri/signals.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/exceptions.py` & `bamboo-pipeline-3.9.1/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/log/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/admin.py` & `bamboo-pipeline-3.9.1/pipeline/log/admin.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/apps.py` & `bamboo-pipeline-3.9.1/pipeline/log/apps.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/handlers.py` & `bamboo-pipeline-3.9.1/pipeline/log/handlers.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/migrations/0001_initial.py` & `bamboo-pipeline-3.9.1/pipeline/log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/migrations/0002_auto_20180810_1054.py` & `bamboo-pipeline-3.9.1/pipeline/log/migrations/0002_auto_20180810_1054.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/migrations/0003_logentry_history_id.py` & `bamboo-pipeline-3.9.1/pipeline/log/migrations/0003_logentry_history_id.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/migrations/0004_auto_20180814_1555.py` & `bamboo-pipeline-3.9.1/pipeline/log/migrations/0004_auto_20180814_1555.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/migrations/0005_auto_20190729_1041.py` & `bamboo-pipeline-3.9.1/pipeline/log/migrations/0005_auto_20190729_1041.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/migrations/0006_auto_20201201_1638.py` & `bamboo-pipeline-3.9.1/pipeline/log/migrations/0006_auto_20201201_1638.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/migrations/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/log/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/models.py` & `bamboo-pipeline-3.9.1/pipeline/log/models.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/tasks.py` & `bamboo-pipeline-3.9.1/pipeline/log/tasks.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/log/views.py` & `bamboo-pipeline-3.9.1/pipeline/log/views.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/logging.py` & `bamboo-pipeline-3.9.1/pipeline/logging.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/management/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/management/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/management/commands/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/management/commands/app.py` & `bamboo-pipeline-3.9.1/pipeline/management/commands/app.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/management/commands/base.py` & `bamboo-pipeline-3.9.1/pipeline/management/commands/base.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/management/commands/celery.py` & `bamboo-pipeline-3.9.1/pipeline/management/commands/celery.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/management/commands/celerybeat.py` & `bamboo-pipeline-3.9.1/pipeline/management/commands/celerybeat.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/management/commands/create_atoms_app.py` & `bamboo-pipeline-3.9.1/pipeline/management/commands/create_atoms_app.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/management/commands/create_plugins_app.py` & `bamboo-pipeline-3.9.1/pipeline/management/commands/create_plugins_app.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/management/commands/generate_config.py` & `bamboo-pipeline-3.9.1/pipeline/management/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0001_initial.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0002_auto_20180109_1825.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0002_auto_20180109_1825.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0003_auto_20180206_1955.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0003_auto_20180206_1955.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0004_auto_20180516_1708.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0004_auto_20180516_1708.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0005_pipelineinstance_tree_info.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0005_pipelineinstance_tree_info.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0006_auto_20180814_1622.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0006_auto_20180814_1622.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0007_templaterelationship.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0007_templaterelationship.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0007_templateversion.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0007_templateversion.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0008_auto_20180824_1115.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0008_auto_20180824_1115.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0011_auto_20180906_1045.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0011_auto_20180906_1045.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0012_templatecurrentversion.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0012_templatecurrentversion.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0013_old_template_process.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0013_old_template_process.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0014_auto_20181127_1053.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0014_auto_20181127_1053.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0015_auto_20181214_1453.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0015_auto_20181214_1453.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0016_auto_20181220_0958.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0016_auto_20181220_0958.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0017_pipelinetemplate_has_subprocess.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0017_pipelinetemplate_has_subprocess.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0018_set_has_subprocess.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0018_set_has_subprocess.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0019_delete_variablemodel.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0019_delete_variablemodel.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0020_auto_20190906_1119.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0020_auto_20190906_1119.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0021_auto_20190906_1143.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0021_auto_20190906_1143.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0022_pipelineinstance_is_revoked.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0022_pipelineinstance_is_revoked.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0023_set_is_revoked.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0023_set_is_revoked.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0024_auto_20200213_0738.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0024_auto_20200213_0738.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0026_auto_20201028_1049.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0026_auto_20201028_1049.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0027_auto_20201123_1552.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0027_auto_20201123_1552.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0028_auto_20201227_1952.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0028_auto_20201227_1952.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/0031_auto_20210624_2317.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/0031_auto_20210624_2317.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/migrations/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/models.py` & `bamboo-pipeline-3.9.1/pipeline/models.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/parser/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/parser/context.py` & `bamboo-pipeline-3.9.1/pipeline/parser/context.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/parser/pipeline_parser.py` & `bamboo-pipeline-3.9.1/pipeline/parser/pipeline_parser.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/parser/schemas.py` & `bamboo-pipeline-3.9.1/pipeline/parser/schemas.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/parser/utils.py` & `bamboo-pipeline-3.9.1/pipeline/parser/utils.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/service/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/service/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/service/pipeline_engine_adapter/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/service/pipeline_engine_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/service/pipeline_engine_adapter/adapter_api.py` & `bamboo-pipeline-3.9.1/pipeline/service/pipeline_engine_adapter/adapter_api.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/service/task_service.py` & `bamboo-pipeline-3.9.1/pipeline/service/task_service.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/signals/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/signals/handlers.py` & `bamboo-pipeline-3.9.1/pipeline/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/templates/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/templates/create_plugins_app/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/templates/create_plugins_app/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/templates/create_plugins_app/js_file.py` & `bamboo-pipeline-3.9.1/pipeline/templates/create_plugins_app/js_file.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/templates/create_plugins_app/plugins.py` & `bamboo-pipeline-3.9.1/pipeline/templates/create_plugins_app/plugins.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/templates/create_plugins_app/py_file.py` & `bamboo-pipeline-3.9.1/pipeline/templates/create_plugins_app/py_file.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/boolrule/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/utils/boolrule/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/boolrule/boolrule.py` & `bamboo-pipeline-3.9.1/pipeline/utils/boolrule/boolrule.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/collections.py` & `bamboo-pipeline-3.9.1/pipeline/utils/collections.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/crypt.py` & `bamboo-pipeline-3.9.1/pipeline/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/dj.py` & `bamboo-pipeline-3.9.1/pipeline/utils/dj.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/env.py` & `bamboo-pipeline-3.9.1/pipeline/utils/env.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/graph.py` & `bamboo-pipeline-3.9.1/pipeline/utils/graph.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/http.py` & `bamboo-pipeline-3.9.1/pipeline/utils/http.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/imoports.py` & `bamboo-pipeline-3.9.1/pipeline/utils/imoports.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/mako_utils/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/utils/mako_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/mako_utils/checker.py` & `bamboo-pipeline-3.9.1/pipeline/utils/mako_utils/checker.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/mako_utils/code_extract.py` & `bamboo-pipeline-3.9.1/pipeline/utils/mako_utils/code_extract.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/mako_utils/exceptions.py` & `bamboo-pipeline-3.9.1/pipeline/utils/mako_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/mako_utils/visitors.py` & `bamboo-pipeline-3.9.1/pipeline/utils/mako_utils/visitors.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/register.py` & `bamboo-pipeline-3.9.1/pipeline/utils/register.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/uniqid.py` & `bamboo-pipeline-3.9.1/pipeline/utils/uniqid.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/utils/utils.py` & `bamboo-pipeline-3.9.1/pipeline/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/validators/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/validators/base.py` & `bamboo-pipeline-3.9.1/pipeline/validators/base.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/validators/connection.py` & `bamboo-pipeline-3.9.1/pipeline/validators/connection.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/validators/gateway.py` & `bamboo-pipeline-3.9.1/pipeline/validators/gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/validators/handlers.py` & `bamboo-pipeline-3.9.1/pipeline/validators/handlers.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/validators/rules.py` & `bamboo-pipeline-3.9.1/pipeline/validators/rules.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/validators/utils.py` & `bamboo-pipeline-3.9.1/pipeline/validators/utils.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/variable_framework/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/variable_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/variable_framework/admin.py` & `bamboo-pipeline-3.9.1/pipeline/variable_framework/admin.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/variable_framework/apps.py` & `bamboo-pipeline-3.9.1/pipeline/variable_framework/apps.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/variable_framework/context.py` & `bamboo-pipeline-3.9.1/pipeline/variable_framework/context.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/variable_framework/management/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/variable_framework/management/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/variable_framework/management/commands/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/variable_framework/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/variable_framework/management/commands/update_variable_models.py` & `bamboo-pipeline-3.9.1/pipeline/variable_framework/management/commands/update_variable_models.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/variable_framework/migrations/0001_initial.py` & `bamboo-pipeline-3.9.1/pipeline/variable_framework/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/variable_framework/migrations/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/variable_framework/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/variable_framework/models.py` & `bamboo-pipeline-3.9.1/pipeline/variable_framework/models.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/variable_framework/signals/__init__.py` & `bamboo-pipeline-3.9.1/pipeline/variable_framework/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pipeline/variable_framework/signals/handlers.py` & `bamboo-pipeline-3.9.1/pipeline/variable_framework/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `bamboo-pipeline-3.9.0/pyproject.toml` & `bamboo-pipeline-3.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bamboo-pipeline"
-version = "3.9.0"
+version = "3.9.1"
 description = "runtime for bamboo-engine base on Django and Celery"
 authors = ["homholueng <homholueng@gmail.com>"]
 license = "MIT"
 packages = [
   { include = "pipeline" },
 ]
```

### Comparing `bamboo-pipeline-3.9.0/setup.py` & `bamboo-pipeline-3.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
  'redis-py-cluster==2.1.0',
  'redis>=3.2.0,<4.0.0',
  'requests>=2.22.0,<3.0.0',
  'ujson>=4.1.0,<4.2.0']
 
 setup_kwargs = {
     'name': 'bamboo-pipeline',
-    'version': '3.9.0',
+    'version': '3.9.1',
     'description': 'runtime for bamboo-engine base on Django and Celery',
     'long_description': None,
     'author': 'homholueng',
     'author_email': 'homholueng@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `bamboo-pipeline-3.9.0/PKG-INFO` & `bamboo-pipeline-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamboo-pipeline
-Version: 3.9.0
+Version: 3.9.1
 Summary: runtime for bamboo-engine base on Django and Celery
 License: MIT
 Author: homholueng
 Author-email: homholueng@gmail.com
 Requires-Python: >=3.6,<3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

