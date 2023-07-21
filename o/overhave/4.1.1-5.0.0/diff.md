# Comparing `tmp/overhave-4.1.1.tar.gz` & `tmp/overhave-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overhave-4.1.1.tar", max compression
+gzip compressed data, was "overhave-5.0.0.tar", max compression
```

## Comparing `overhave-4.1.1.tar` & `overhave-5.0.0.tar`

### file list

```diff
@@ -1,245 +1,245 @@
--rw-r--r--   0        0        0    23136 2023-07-20 08:50:59.794347 overhave-4.1.1/README.rst
--rw-r--r--   0        0        0     3193 2023-07-20 08:50:59.806347 overhave-4.1.1/overhave/__init__.py
--rw-r--r--   0        0        0       63 2023-07-20 08:50:59.806347 overhave-4.1.1/overhave/admin/__init__.py
--rw-r--r--   0        0        0     5172 2023-07-20 08:50:59.806347 overhave-4.1.1/overhave/admin/app.py
--rw-r--r--   0        0        0   735118 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/files/ace-src/ace.js
--rw-r--r--   0        0        0     5426 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/files/ace-src/mode-gherkin.js
--rw-r--r--   0        0        0     1263 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/files/css/overhave.css
--rw-r--r--   0        0        0    38062 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/files/favicon.ico
--rw-r--r--   0        0        0      138 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/flask/__init__.py
--rw-r--r--   0        0        0     1893 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/flask/flask_admin.py
--rw-r--r--   0        0        0      287 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/flask/flask_app.py
--rw-r--r--   0        0        0     2112 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/flask/login_manager.py
--rw-r--r--   0        0        0      187 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/templates/draft_detail.html
--rw-r--r--   0        0        0      405 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/templates/emulation.html
--rw-r--r--   0        0        0      194 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/templates/emulation_create.html
--rw-r--r--   0        0        0      190 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/emulation_edit.html
--rw-r--r--   0        0        0      860 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/emulation_run_detail.html
--rw-r--r--   0        0        0    10071 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/feature.html
--rw-r--r--   0        0        0      404 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/feature_create.html
--rw-r--r--   0        0        0      465 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/feature_edit.html
--rw-r--r--   0        0        0      177 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/index.html
--rw-r--r--   0        0        0     2414 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/login.html
--rw-r--r--   0        0        0      149 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/overhave_master.html
--rw-r--r--   0        0        0     1696 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/test_run.html
--rw-r--r--   0        0        0     1535 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/test_run_detail.html
--rw-r--r--   0        0        0      189 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/test_run_list.html
--rw-r--r--   0        0        0      606 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/test_user.html
--rw-r--r--   0        0        0      210 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/test_user_create.html
--rw-r--r--   0        0        0      208 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/test_user_edit.html
--rw-r--r--   0        0        0      451 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/__init__.py
--rw-r--r--   0        0        0     1386 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/access.py
--rw-r--r--   0        0        0     2914 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/base.py
--rw-r--r--   0        0        0     1105 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/draft.py
--rw-r--r--   0        0        0     3407 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/emulation.py
--rw-r--r--   0        0        0     1620 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/emulation_run.py
--rw-r--r--   0        0        0    10257 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/feature.py
--rw-r--r--   0        0        0      306 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/formatters/__init__.py
--rw-r--r--   0        0        0     4997 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/formatters/formatters.py
--rw-r--r--   0        0        0      631 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/formatters/helpers.py
--rw-r--r--   0        0        0     1404 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/formatters/safe_formatter.py
--rw-r--r--   0        0        0       51 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/index/__init__.py
--rw-r--r--   0        0        0     1648 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/index/custom_page.py
--rw-r--r--   0        0        0     1578 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/index/login_form.py
--rw-r--r--   0        0        0     3023 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/index/view.py
--rw-r--r--   0        0        0     1794 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/scenario_test_run.py
--rw-r--r--   0        0        0     1329 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/tag.py
--rw-r--r--   0        0        0     3665 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/testing_users.py
--rw-r--r--   0        0        0       52 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/__init__.py
--rw-r--r--   0        0        0     5970 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/app.py
--rw-r--r--   0        0        0      216 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/asgi.py
--rw-r--r--   0        0        0      143 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/auth/__init__.py
--rw-r--r--   0        0        0      348 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/auth/models.py
--rw-r--r--   0        0        0     1395 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/auth/regular.py
--rw-r--r--   0        0        0      867 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/auth/token.py
--rw-r--r--   0        0        0     2422 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/deps.py
--rw-r--r--   0        0        0      848 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/settings.py
--rw-r--r--   0        0        0      580 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/__init__.py
--rw-r--r--   0        0        0     1416 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/auth_views.py
--rw-r--r--   0        0        0      550 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/emulation_views.py
--rw-r--r--   0        0        0      586 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/extra_views.py
--rw-r--r--   0        0        0      461 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/feature_type_views.py
--rw-r--r--   0        0        0     1184 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/feature_views.py
--rw-r--r--   0        0        0      969 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/tags_views.py
--rw-r--r--   0        0        0     2041 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/testrun_views.py
--rw-r--r--   0        0        0     4496 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/testuser_views.py
--rw-r--r--   0        0        0     4047 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/base_settings.py
--rw-r--r--   0        0        0      164 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/__init__.py
--rw-r--r--   0        0        0      557 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/admin.py
--rw-r--r--   0        0        0      534 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/api.py
--rw-r--r--   0        0        0      647 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/consumers.py
--rw-r--r--   0        0        0       84 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/db_cmds/__init__.py
--rw-r--r--   0        0        0      830 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/db_cmds/group.py
--rw-r--r--   0        0        0     1755 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/db_cmds/regular.py
--rw-r--r--   0        0        0      358 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/group.py
--rw-r--r--   0        0        0     3048 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/s3.py
--rw-r--r--   0        0        0     1573 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/synchronizer.py
--rw-r--r--   0        0        0      455 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/db/__init__.py
--rw-r--r--   0        0        0     3283 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/db/base.py
--rw-r--r--   0        0        0     1349 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/db/statuses.py
--rw-r--r--   0        0        0     8141 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/db/tables.py
--rw-r--r--   0        0        0      795 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/db/users.py
--rw-r--r--   0        0        0     1249 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/db/utils.py
--rw-r--r--   0        0        0       46 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/emulation/__init__.py
--rw-r--r--   0        0        0     4103 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/emulation/emulator.py
--rw-r--r--   0        0        0      897 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/__init__.py
--rw-r--r--   0        0        0     1231 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/archiver.py
--rw-r--r--   0        0        0      247 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/__init__.py
--rw-r--r--   0        0        0      316 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/abstract.py
--rw-r--r--   0        0        0      497 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/base.py
--rw-r--r--   0        0        0      754 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/default.py
--rw-r--r--   0        0        0      116 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/ldap/__init__.py
--rw-r--r--   0        0        0     3493 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/ldap/manager.py
--rw-r--r--   0        0        0      198 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/ldap/settings.py
--rw-r--r--   0        0        0     1487 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/secret_mixin.py
--rw-r--r--   0        0        0     1396 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/simple.py
--rw-r--r--   0        0        0      169 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/feature/__init__.py
--rw-r--r--   0        0        0      425 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/feature/abstract.py
--rw-r--r--   0        0        0      221 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/feature/errors.py
--rw-r--r--   0        0        0     2748 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/feature/extractor.py
--rw-r--r--   0        0        0     1098 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/file_extractor.py
--rw-r--r--   0        0        0     1760 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/git_initializer.py
--rw-r--r--   0        0        0       55 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/language/__init__.py
--rw-r--r--   0        0        0     1198 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/language/prefixes.py
--rw-r--r--   0        0        0      102 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/report_manager/__init__.py
--rw-r--r--   0        0        0      415 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/report_manager/models.py
--rw-r--r--   0        0        0     5825 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/report_manager/report_manager.py
--rw-r--r--   0        0        0     6700 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/settings.py
--rw-r--r--   0        0        0       54 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/extra/__init__.py
--rw-r--r--   0        0        0      386 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/extra/prefixes.py
--rw-r--r--   0        0        0      739 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/__init__.py
--rw-r--r--   0        0        0     7209 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/base_factory.py
--rw-r--r--   0        0        0      418 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/__init__.py
--rw-r--r--   0        0        0      306 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/abstract_consumer.py
--rw-r--r--   0        0        0     4555 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/admin_factory.py
--rw-r--r--   0        0        0     1312 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/emulation_factory.py
--rw-r--r--   0        0        0     3956 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/publication_factory.py
--rw-r--r--   0        0        0      486 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/s3_init_factory.py
--rw-r--r--   0        0        0     2184 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/synchronizer_factory.py
--rw-r--r--   0        0        0     1888 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/test_execution_factory.py
--rw-r--r--   0        0        0     2045 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/consumer_factory.py
--rw-r--r--   0        0        0      550 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/__init__.py
--rw-r--r--   0        0        0     2950 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/admin_context.py
--rw-r--r--   0        0        0     4028 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/base_context.py
--rw-r--r--   0        0        0      506 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/emulation_context.py
--rw-r--r--   0        0        0     2032 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/publication_context.py
--rw-r--r--   0        0        0     1288 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/synchronizer_context.py
--rw-r--r--   0        0        0     2519 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/test_execution_context.py
--rw-r--r--   0        0        0      769 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/getters.py
--rw-r--r--   0        0        0      353 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/metrics/__init__.py
--rw-r--r--   0        0        0      193 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/metrics/client/__init__.py
--rw-r--r--   0        0        0     3162 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/metrics/client/container.py
--rw-r--r--   0        0        0      983 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/metrics/getters.py
--rw-r--r--   0        0        0      342 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/__init__.py
--rw-r--r--   0        0        0      399 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/abstract_publisher.py
--rw-r--r--   0        0        0     4015 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/base_publisher.py
--rw-r--r--   0        0        0      532 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/errors.py
--rw-r--r--   0        0        0     4928 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/git_publisher.py
--rw-r--r--   0        0        0      224 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/gitlab/__init__.py
--rw-r--r--   0        0        0     4208 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/gitlab/gitlab_publisher.py
--rw-r--r--   0        0        0     1408 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/gitlab/settings.py
--rw-r--r--   0        0        0      171 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/gitlab/tokenizer/__init__.py
--rw-r--r--   0        0        0     2157 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/gitlab/tokenizer/client.py
--rw-r--r--   0        0        0     1015 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/gitlab/tokenizer/settings.py
--rw-r--r--   0        0        0      178 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/objects.py
--rw-r--r--   0        0        0      877 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/settings.py
--rw-r--r--   0        0        0      119 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/stash/__init__.py
--rw-r--r--   0        0        0     1672 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/stash/settings.py
--rw-r--r--   0        0        0     4323 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/stash/stash_publisher.py
--rw-r--r--   0        0        0      371 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/__init__.py
--rw-r--r--   0        0        0     3538 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/config_injector.py
--rw-r--r--   0        0        0      827 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/deps.py
--rw-r--r--   0        0        0      530 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/__init__.py
--rw-r--r--   0        0        0      305 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/__init__.py
--rw-r--r--   0        0        0      927 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/description_manager.py
--rw-r--r--   0        0        0     1102 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/links.py
--rw-r--r--   0        0        0     1260 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/severity.py
--rw-r--r--   0        0        0     2452 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py
--rw-r--r--   0        0        0     1638 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/bdd_item.py
--rw-r--r--   0        0        0      981 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/parsed_info.py
--rw-r--r--   0        0        0     2874 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/tag_controller.py
--rw-r--r--   0        0        0     6192 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/plugin.py
--rw-r--r--   0        0        0     2223 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/plugin_resolver.py
--rw-r--r--   0        0        0     3945 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/proxy_manager.py
--rw-r--r--   0        0        0      517 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/__init__.py
--rw-r--r--   0        0        0      157 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/compiler/__init__.py
--rw-r--r--   0        0        0     5100 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/compiler/compiler.py
--rw-r--r--   0        0        0      631 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/compiler/settings.py
--rw-r--r--   0        0        0      150 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/file_manager/__init__.py
--rw-r--r--   0        0        0     3495 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/file_manager/file_manager.py
--rw-r--r--   0        0        0     2820 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/file_manager/settings.py
--rw-r--r--   0        0        0      230 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/parser/__init__.py
--rw-r--r--   0        0        0      854 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/parser/models.py
--rw-r--r--   0        0        0     8442 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/parser/parser.py
--rw-r--r--   0        0        0      263 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/parser/settings.py
--rw-r--r--   0        0        0      235 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/prefix_mixin.py
--rw-r--r--   0        0        0       95 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/validator/__init__.py
--rw-r--r--   0        0        0      229 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/validator/abstract.py
--rw-r--r--   0        0        0     1441 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/validator/duplicate_id_mixin.py
--rw-r--r--   0        0        0      510 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/validator/errors.py
--rw-r--r--   0        0        0     2827 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/validator/validator.py
--rw-r--r--   0        0        0     1226 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/__init__.py
--rw-r--r--   0        0        0     1180 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/api_auth_storage.py
--rw-r--r--   0        0        0     3271 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/converters.py
--rw-r--r--   0        0        0     6178 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/draft_storage.py
--rw-r--r--   0        0        0     5323 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/emulation_storage.py
--rw-r--r--   0        0        0     4947 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/feature_storage.py
--rw-r--r--   0        0        0     1566 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/feature_tag_storage.py
--rw-r--r--   0        0        0     2176 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/feature_type_storage.py
--rw-r--r--   0        0        0     1902 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/scenario_storage.py
--rw-r--r--   0        0        0      589 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/system_user_group_storage.py
--rw-r--r--   0        0        0     1930 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/system_user_storage.py
--rw-r--r--   0        0        0     3054 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/test_run_storage.py
--rw-r--r--   0        0        0     3616 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/test_user_storage.py
--rw-r--r--   0        0        0      192 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/synchronization/__init__.py
--rw-r--r--   0        0        0      260 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/synchronization/abstract.py
--rw-r--r--   0        0        0     3728 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/synchronization/storage_manager.py
--rw-r--r--   0        0        0     7025 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/synchronization/synchronizer.py
--rw-r--r--   0        0        0      307 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/test_execution/__init__.py
--rw-r--r--   0        0        0     4256 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/test_execution/executor.py
--rw-r--r--   0        0        0     1056 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/test_execution/objects.py
--rw-r--r--   0        0        0     1750 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/test_execution/settings.py
--rw-r--r--   0        0        0     4106 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/test_execution/step_collector.py
--rw-r--r--   0        0        0     1617 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/test_execution/test_runner.py
--rw-r--r--   0        0        0      983 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/__init__.py
--rw-r--r--   0        0        0      623 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/__init__.py
--rw-r--r--   0        0        0      122 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/api_client/__init__.py
--rw-r--r--   0        0        0     1810 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/api_client/authenticator.py
--rw-r--r--   0        0        0      237 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/api_client/models.py
--rw-r--r--   0        0        0      499 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/api_client/settings.py
--rw-r--r--   0        0        0      208 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/base_client/__init__.py
--rw-r--r--   0        0        0      590 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/base_client/auth.py
--rw-r--r--   0        0        0     2139 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/base_client/client.py
--rw-r--r--   0        0        0      110 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/base_client/objects.py
--rw-r--r--   0        0        0     1287 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/base_client/settings.py
--rw-r--r--   0        0        0      258 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/gitlab_client/__init__.py
--rw-r--r--   0        0        0     2003 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/gitlab_client/client.py
--rw-r--r--   0        0        0      609 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/gitlab_client/models.py
--rw-r--r--   0        0        0      144 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/gitlab_client/objects.py
--rw-r--r--   0        0        0      377 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/gitlab_client/settings.py
--rw-r--r--   0        0        0      741 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/gitlab_client/utils.py
--rw-r--r--   0        0        0      326 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/stash_client/__init__.py
--rw-r--r--   0        0        0     2115 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/stash_client/client.py
--rw-r--r--   0        0        0     2757 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/stash_client/models.py
--rw-r--r--   0        0        0      569 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/stash_client/settings.py
--rw-r--r--   0        0        0      109 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/ldap/__init__.py
--rw-r--r--   0        0        0     1896 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/ldap/authenticator.py
--rw-r--r--   0        0        0      420 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/ldap/settings.py
--rw-r--r--   0        0        0      430 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/__init__.py
--rw-r--r--   0        0        0     2937 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/consumer.py
--rw-r--r--   0        0        0     1661 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/deps.py
--rw-r--r--   0        0        0     2439 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/objects.py
--rw-r--r--   0        0        0     1319 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/producer.py
--rw-r--r--   0        0        0     1384 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/runner.py
--rw-r--r--   0        0        0     1674 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/settings.py
--rw-r--r--   0        0        0      132 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/s3/__init__.py
--rw-r--r--   0        0        0     8494 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/s3/manager.py
--rw-r--r--   0        0        0     2082 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/s3/models.py
--rw-r--r--   0        0        0      181 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/s3/objects.py
--rw-r--r--   0        0        0      885 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/s3/settings.py
--rw-r--r--   0        0        0      103 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/utils/__init__.py
--rw-r--r--   0        0        0       84 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/utils/mocks.py
--rw-r--r--   0        0        0      139 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/utils/time.py
--rw-r--r--   0        0        0      148 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/utils/url.py
--rw-r--r--   0        0        0     3522 2023-07-20 08:50:59.822347 overhave-4.1.1/pyproject.toml
--rw-r--r--   0        0        0    25392 1970-01-01 00:00:00.000000 overhave-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0    23136 2023-07-21 08:56:59.151749 overhave-5.0.0/README.rst
+-rw-r--r--   0        0        0     3193 2023-07-21 08:56:59.163750 overhave-5.0.0/overhave/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-21 08:56:59.163750 overhave-5.0.0/overhave/admin/__init__.py
+-rw-r--r--   0        0        0     5172 2023-07-21 08:56:59.163750 overhave-5.0.0/overhave/admin/app.py
+-rw-r--r--   0        0        0   735118 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/files/ace-src/ace.js
+-rw-r--r--   0        0        0     5426 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/files/ace-src/mode-gherkin.js
+-rw-r--r--   0        0        0     1263 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/files/css/overhave.css
+-rw-r--r--   0        0        0    38062 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/files/favicon.ico
+-rw-r--r--   0        0        0      138 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/flask/__init__.py
+-rw-r--r--   0        0        0     1893 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/flask/flask_admin.py
+-rw-r--r--   0        0        0      287 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/flask/flask_app.py
+-rw-r--r--   0        0        0     2112 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/flask/login_manager.py
+-rw-r--r--   0        0        0      187 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/draft_detail.html
+-rw-r--r--   0        0        0      405 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/emulation.html
+-rw-r--r--   0        0        0      194 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/emulation_create.html
+-rw-r--r--   0        0        0      190 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/emulation_edit.html
+-rw-r--r--   0        0        0      860 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/emulation_run_detail.html
+-rw-r--r--   0        0        0    10071 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/feature.html
+-rw-r--r--   0        0        0      404 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/feature_create.html
+-rw-r--r--   0        0        0      465 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/feature_edit.html
+-rw-r--r--   0        0        0      177 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/index.html
+-rw-r--r--   0        0        0     2414 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/login.html
+-rw-r--r--   0        0        0      149 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/overhave_master.html
+-rw-r--r--   0        0        0     1696 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/test_run.html
+-rw-r--r--   0        0        0     1535 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/test_run_detail.html
+-rw-r--r--   0        0        0      189 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/test_run_list.html
+-rw-r--r--   0        0        0      606 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/test_user.html
+-rw-r--r--   0        0        0      210 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/test_user_create.html
+-rw-r--r--   0        0        0      208 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/templates/test_user_edit.html
+-rw-r--r--   0        0        0      451 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/views/__init__.py
+-rw-r--r--   0        0        0     1386 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/views/access.py
+-rw-r--r--   0        0        0     2914 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/views/base.py
+-rw-r--r--   0        0        0     1105 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/views/draft.py
+-rw-r--r--   0        0        0     3407 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/views/emulation.py
+-rw-r--r--   0        0        0     1620 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/views/emulation_run.py
+-rw-r--r--   0        0        0    10257 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/views/feature.py
+-rw-r--r--   0        0        0      306 2023-07-21 08:56:59.167750 overhave-5.0.0/overhave/admin/views/formatters/__init__.py
+-rw-r--r--   0        0        0     4997 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/admin/views/formatters/formatters.py
+-rw-r--r--   0        0        0      631 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/admin/views/formatters/helpers.py
+-rw-r--r--   0        0        0     1404 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/admin/views/formatters/safe_formatter.py
+-rw-r--r--   0        0        0       51 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/admin/views/index/__init__.py
+-rw-r--r--   0        0        0     1648 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/admin/views/index/custom_page.py
+-rw-r--r--   0        0        0     1578 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/admin/views/index/login_form.py
+-rw-r--r--   0        0        0     3023 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/admin/views/index/view.py
+-rw-r--r--   0        0        0     1794 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/admin/views/scenario_test_run.py
+-rw-r--r--   0        0        0     1329 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/admin/views/tag.py
+-rw-r--r--   0        0        0     3755 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/admin/views/testing_users.py
+-rw-r--r--   0        0        0       52 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/__init__.py
+-rw-r--r--   0        0        0     5960 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/app.py
+-rw-r--r--   0        0        0      216 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/asgi.py
+-rw-r--r--   0        0        0      143 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/auth/__init__.py
+-rw-r--r--   0        0        0      350 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/auth/models.py
+-rw-r--r--   0        0        0     1407 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/auth/regular.py
+-rw-r--r--   0        0        0      867 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/auth/token.py
+-rw-r--r--   0        0        0     2422 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/deps.py
+-rw-r--r--   0        0        0      844 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/settings.py
+-rw-r--r--   0        0        0      575 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/views/__init__.py
+-rw-r--r--   0        0        0     1422 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/views/auth_views.py
+-rw-r--r--   0        0        0      550 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/views/emulation_views.py
+-rw-r--r--   0        0        0      586 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/views/extra_views.py
+-rw-r--r--   0        0        0      461 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/views/feature_type_views.py
+-rw-r--r--   0        0        0     1184 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/views/feature_views.py
+-rw-r--r--   0        0        0      969 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/views/tags_views.py
+-rw-r--r--   0        0        0     2046 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/views/testrun_views.py
+-rw-r--r--   0        0        0     4531 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/api/views/testuser_views.py
+-rw-r--r--   0        0        0     3798 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/base_settings.py
+-rw-r--r--   0        0        0      164 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/cli/__init__.py
+-rw-r--r--   0        0        0      557 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/cli/admin.py
+-rw-r--r--   0        0        0      540 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/cli/api.py
+-rw-r--r--   0        0        0      647 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/cli/consumers.py
+-rw-r--r--   0        0        0       84 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/cli/db_cmds/__init__.py
+-rw-r--r--   0        0        0      830 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/cli/db_cmds/group.py
+-rw-r--r--   0        0        0     1755 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/cli/db_cmds/regular.py
+-rw-r--r--   0        0        0      358 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/cli/group.py
+-rw-r--r--   0        0        0     3048 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/cli/s3.py
+-rw-r--r--   0        0        0     1573 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/cli/synchronizer.py
+-rw-r--r--   0        0        0      455 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/db/__init__.py
+-rw-r--r--   0        0        0     3283 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/db/base.py
+-rw-r--r--   0        0        0     1349 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/db/statuses.py
+-rw-r--r--   0        0        0     8141 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/db/tables.py
+-rw-r--r--   0        0        0      795 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/db/users.py
+-rw-r--r--   0        0        0     1249 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/db/utils.py
+-rw-r--r--   0        0        0       46 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/emulation/__init__.py
+-rw-r--r--   0        0        0     4103 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/emulation/emulator.py
+-rw-r--r--   0        0        0      897 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/__init__.py
+-rw-r--r--   0        0        0     1231 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/archiver.py
+-rw-r--r--   0        0        0      247 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/auth_managers/__init__.py
+-rw-r--r--   0        0        0      316 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/auth_managers/abstract.py
+-rw-r--r--   0        0        0      497 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/auth_managers/base.py
+-rw-r--r--   0        0        0      760 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/auth_managers/default.py
+-rw-r--r--   0        0        0      116 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/auth_managers/ldap/__init__.py
+-rw-r--r--   0        0        0     3505 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/auth_managers/ldap/manager.py
+-rw-r--r--   0        0        0      198 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/auth_managers/ldap/settings.py
+-rw-r--r--   0        0        0     1487 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/auth_managers/secret_mixin.py
+-rw-r--r--   0        0        0     1402 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/auth_managers/simple.py
+-rw-r--r--   0        0        0      169 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/feature/__init__.py
+-rw-r--r--   0        0        0      425 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/feature/abstract.py
+-rw-r--r--   0        0        0      221 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/feature/errors.py
+-rw-r--r--   0        0        0     2748 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/feature/extractor.py
+-rw-r--r--   0        0        0     1098 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/file_extractor.py
+-rw-r--r--   0        0        0     1760 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/git_initializer.py
+-rw-r--r--   0        0        0       55 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/language/__init__.py
+-rw-r--r--   0        0        0     1198 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/language/prefixes.py
+-rw-r--r--   0        0        0      102 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/report_manager/__init__.py
+-rw-r--r--   0        0        0      439 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/report_manager/models.py
+-rw-r--r--   0        0        0     5916 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/report_manager/report_manager.py
+-rw-r--r--   0        0        0     6954 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/entities/settings.py
+-rw-r--r--   0        0        0       54 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/extra/__init__.py
+-rw-r--r--   0        0        0      386 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/extra/prefixes.py
+-rw-r--r--   0        0        0      739 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/__init__.py
+-rw-r--r--   0        0        0     7209 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/base_factory.py
+-rw-r--r--   0        0        0      418 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/components/__init__.py
+-rw-r--r--   0        0        0      306 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/components/abstract_consumer.py
+-rw-r--r--   0        0        0     4555 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/components/admin_factory.py
+-rw-r--r--   0        0        0     1312 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/components/emulation_factory.py
+-rw-r--r--   0        0        0     3956 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/components/publication_factory.py
+-rw-r--r--   0        0        0      486 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/components/s3_init_factory.py
+-rw-r--r--   0        0        0     2184 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/components/synchronizer_factory.py
+-rw-r--r--   0        0        0     1888 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/components/test_execution_factory.py
+-rw-r--r--   0        0        0     2045 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/consumer_factory.py
+-rw-r--r--   0        0        0      550 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/context/__init__.py
+-rw-r--r--   0        0        0     2950 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/context/admin_context.py
+-rw-r--r--   0        0        0     4037 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/context/base_context.py
+-rw-r--r--   0        0        0      506 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/context/emulation_context.py
+-rw-r--r--   0        0        0     2032 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/context/publication_context.py
+-rw-r--r--   0        0        0     1288 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/context/synchronizer_context.py
+-rw-r--r--   0        0        0     2519 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/context/test_execution_context.py
+-rw-r--r--   0        0        0      769 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/factory/getters.py
+-rw-r--r--   0        0        0      353 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/metrics/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/metrics/client/__init__.py
+-rw-r--r--   0        0        0     3162 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/metrics/client/container.py
+-rw-r--r--   0        0        0      983 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/metrics/getters.py
+-rw-r--r--   0        0        0      342 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/__init__.py
+-rw-r--r--   0        0        0      399 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/abstract_publisher.py
+-rw-r--r--   0        0        0     4015 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/base_publisher.py
+-rw-r--r--   0        0        0      532 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/errors.py
+-rw-r--r--   0        0        0     4928 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/git_publisher.py
+-rw-r--r--   0        0        0      224 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/gitlab/__init__.py
+-rw-r--r--   0        0        0     4219 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/gitlab/gitlab_publisher.py
+-rw-r--r--   0        0        0     1408 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/gitlab/settings.py
+-rw-r--r--   0        0        0      171 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/gitlab/tokenizer/__init__.py
+-rw-r--r--   0        0        0     2157 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/gitlab/tokenizer/client.py
+-rw-r--r--   0        0        0     1096 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/gitlab/tokenizer/settings.py
+-rw-r--r--   0        0        0      178 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/objects.py
+-rw-r--r--   0        0        0      877 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/settings.py
+-rw-r--r--   0        0        0      119 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/stash/__init__.py
+-rw-r--r--   0        0        0     1672 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/stash/settings.py
+-rw-r--r--   0        0        0     4334 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/publication/stash/stash_publisher.py
+-rw-r--r--   0        0        0      371 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/pytest_plugin/__init__.py
+-rw-r--r--   0        0        0     3538 2023-07-21 08:56:59.171750 overhave-5.0.0/overhave/pytest_plugin/config_injector.py
+-rw-r--r--   0        0        0      827 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/pytest_plugin/deps.py
+-rw-r--r--   0        0        0      530 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/pytest_plugin/helpers/__init__.py
+-rw-r--r--   0        0        0      305 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/pytest_plugin/helpers/allure_utils/__init__.py
+-rw-r--r--   0        0        0      927 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/pytest_plugin/helpers/allure_utils/description_manager.py
+-rw-r--r--   0        0        0     1102 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/pytest_plugin/helpers/allure_utils/links.py
+-rw-r--r--   0        0        0     1260 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/pytest_plugin/helpers/allure_utils/severity.py
+-rw-r--r--   0        0        0     2452 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py
+-rw-r--r--   0        0        0     1638 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/pytest_plugin/helpers/bdd_item.py
+-rw-r--r--   0        0        0      981 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/pytest_plugin/helpers/parsed_info.py
+-rw-r--r--   0        0        0     2874 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/pytest_plugin/helpers/tag_controller.py
+-rw-r--r--   0        0        0     6192 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/pytest_plugin/plugin.py
+-rw-r--r--   0        0        0     2223 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/pytest_plugin/plugin_resolver.py
+-rw-r--r--   0        0        0     3945 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/pytest_plugin/proxy_manager.py
+-rw-r--r--   0        0        0      517 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/__init__.py
+-rw-r--r--   0        0        0      157 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/compiler/__init__.py
+-rw-r--r--   0        0        0     5100 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/compiler/compiler.py
+-rw-r--r--   0        0        0      631 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/compiler/settings.py
+-rw-r--r--   0        0        0      150 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/file_manager/__init__.py
+-rw-r--r--   0        0        0     3495 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/file_manager/file_manager.py
+-rw-r--r--   0        0        0     2904 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/file_manager/settings.py
+-rw-r--r--   0        0        0      230 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/parser/__init__.py
+-rw-r--r--   0        0        0      985 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/parser/models.py
+-rw-r--r--   0        0        0     8474 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/parser/parser.py
+-rw-r--r--   0        0        0      263 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/parser/settings.py
+-rw-r--r--   0        0        0      235 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/prefix_mixin.py
+-rw-r--r--   0        0        0       95 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/validator/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/validator/abstract.py
+-rw-r--r--   0        0        0     1441 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/validator/duplicate_id_mixin.py
+-rw-r--r--   0        0        0      510 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/validator/errors.py
+-rw-r--r--   0        0        0     2827 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/scenario/validator/validator.py
+-rw-r--r--   0        0        0     1226 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/storage/__init__.py
+-rw-r--r--   0        0        0     1163 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/storage/api_auth_storage.py
+-rw-r--r--   0        0        0     3278 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/storage/converters.py
+-rw-r--r--   0        0        0     6184 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/storage/draft_storage.py
+-rw-r--r--   0        0        0     5297 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/storage/emulation_storage.py
+-rw-r--r--   0        0        0     4967 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/storage/feature_storage.py
+-rw-r--r--   0        0        0     1578 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/storage/feature_tag_storage.py
+-rw-r--r--   0        0        0     2182 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/storage/feature_type_storage.py
+-rw-r--r--   0        0        0     1914 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/storage/scenario_storage.py
+-rw-r--r--   0        0        0      589 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/storage/system_user_group_storage.py
+-rw-r--r--   0        0        0     1936 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/storage/system_user_storage.py
+-rw-r--r--   0        0        0     3066 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/storage/test_run_storage.py
+-rw-r--r--   0        0        0     3634 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/storage/test_user_storage.py
+-rw-r--r--   0        0        0      192 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/synchronization/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/synchronization/abstract.py
+-rw-r--r--   0        0        0     3708 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/synchronization/storage_manager.py
+-rw-r--r--   0        0        0     7057 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/synchronization/synchronizer.py
+-rw-r--r--   0        0        0      307 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/test_execution/__init__.py
+-rw-r--r--   0        0        0     4256 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/test_execution/executor.py
+-rw-r--r--   0        0        0     1068 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/test_execution/objects.py
+-rw-r--r--   0        0        0     1811 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/test_execution/settings.py
+-rw-r--r--   0        0        0     4112 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/test_execution/step_collector.py
+-rw-r--r--   0        0        0     1617 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/test_execution/test_runner.py
+-rw-r--r--   0        0        0      983 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/__init__.py
+-rw-r--r--   0        0        0      623 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/__init__.py
+-rw-r--r--   0        0        0      122 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/api_client/__init__.py
+-rw-r--r--   0        0        0     1821 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/api_client/authenticator.py
+-rw-r--r--   0        0        0      223 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/api_client/models.py
+-rw-r--r--   0        0        0      499 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/api_client/settings.py
+-rw-r--r--   0        0        0      208 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/base_client/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/base_client/auth.py
+-rw-r--r--   0        0        0     2169 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/base_client/client.py
+-rw-r--r--   0        0        0      110 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/base_client/objects.py
+-rw-r--r--   0        0        0     1333 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/base_client/settings.py
+-rw-r--r--   0        0        0      258 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/gitlab_client/__init__.py
+-rw-r--r--   0        0        0     2009 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/gitlab_client/client.py
+-rw-r--r--   0        0        0      609 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/gitlab_client/models.py
+-rw-r--r--   0        0        0      144 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/gitlab_client/objects.py
+-rw-r--r--   0        0        0      377 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/gitlab_client/settings.py
+-rw-r--r--   0        0        0      741 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/gitlab_client/utils.py
+-rw-r--r--   0        0        0      326 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/stash_client/__init__.py
+-rw-r--r--   0        0        0     2121 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/stash_client/client.py
+-rw-r--r--   0        0        0     2857 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/stash_client/models.py
+-rw-r--r--   0        0        0      569 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/http/stash_client/settings.py
+-rw-r--r--   0        0        0      109 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/ldap/__init__.py
+-rw-r--r--   0        0        0     1896 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/ldap/authenticator.py
+-rw-r--r--   0        0        0      416 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/ldap/settings.py
+-rw-r--r--   0        0        0      430 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/redis/__init__.py
+-rw-r--r--   0        0        0     2973 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/redis/consumer.py
+-rw-r--r--   0        0        0     1661 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/redis/deps.py
+-rw-r--r--   0        0        0     2456 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/redis/objects.py
+-rw-r--r--   0        0        0     1319 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/redis/producer.py
+-rw-r--r--   0        0        0     1384 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/redis/runner.py
+-rw-r--r--   0        0        0     1667 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/redis/settings.py
+-rw-r--r--   0        0        0      132 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/s3/__init__.py
+-rw-r--r--   0        0        0     8558 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/s3/manager.py
+-rw-r--r--   0        0        0     2336 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/s3/models.py
+-rw-r--r--   0        0        0      181 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/s3/objects.py
+-rw-r--r--   0        0        0     1026 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/transport/s3/settings.py
+-rw-r--r--   0        0        0      103 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/utils/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/utils/mocks.py
+-rw-r--r--   0        0        0      139 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/utils/time.py
+-rw-r--r--   0        0        0      148 2023-07-21 08:56:59.175750 overhave-5.0.0/overhave/utils/url.py
+-rw-r--r--   0        0        0     3551 2023-07-21 08:56:59.179750 overhave-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0    25442 1970-01-01 00:00:00.000000 overhave-5.0.0/PKG-INFO
```

### Comparing `overhave-4.1.1/README.rst` & `overhave-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/__init__.py` & `overhave-5.0.0/overhave/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/app.py` & `overhave-5.0.0/overhave/admin/app.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/files/ace-src/ace.js` & `overhave-5.0.0/overhave/admin/files/ace-src/ace.js`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/files/ace-src/mode-gherkin.js` & `overhave-5.0.0/overhave/admin/files/ace-src/mode-gherkin.js`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/files/css/overhave.css` & `overhave-5.0.0/overhave/admin/files/css/overhave.css`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/files/favicon.ico` & `overhave-5.0.0/overhave/admin/files/favicon.ico`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/flask/flask_admin.py` & `overhave-5.0.0/overhave/admin/flask/flask_admin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/flask/login_manager.py` & `overhave-5.0.0/overhave/admin/flask/login_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/templates/emulation_run_detail.html` & `overhave-5.0.0/overhave/admin/templates/emulation_run_detail.html`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/templates/feature.html` & `overhave-5.0.0/overhave/admin/templates/feature.html`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/templates/login.html` & `overhave-5.0.0/overhave/admin/templates/login.html`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/templates/test_run.html` & `overhave-5.0.0/overhave/admin/templates/test_run.html`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/templates/test_run_detail.html` & `overhave-5.0.0/overhave/admin/templates/test_run_detail.html`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/templates/test_user.html` & `overhave-5.0.0/overhave/admin/templates/test_user.html`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/access.py` & `overhave-5.0.0/overhave/admin/views/access.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/base.py` & `overhave-5.0.0/overhave/admin/views/base.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/draft.py` & `overhave-5.0.0/overhave/admin/views/draft.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/emulation.py` & `overhave-5.0.0/overhave/admin/views/emulation.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/emulation_run.py` & `overhave-5.0.0/overhave/admin/views/emulation_run.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/feature.py` & `overhave-5.0.0/overhave/admin/views/feature.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/formatters/formatters.py` & `overhave-5.0.0/overhave/admin/views/formatters/formatters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/formatters/helpers.py` & `overhave-5.0.0/overhave/admin/views/formatters/helpers.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/formatters/safe_formatter.py` & `overhave-5.0.0/overhave/admin/views/formatters/safe_formatter.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/index/custom_page.py` & `overhave-5.0.0/overhave/admin/views/index/custom_page.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/index/login_form.py` & `overhave-5.0.0/overhave/admin/views/index/login_form.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/index/view.py` & `overhave-5.0.0/overhave/admin/views/index/view.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/scenario_test_run.py` & `overhave-5.0.0/overhave/admin/views/scenario_test_run.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/tag.py` & `overhave-5.0.0/overhave/admin/views/tag.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/admin/views/testing_users.py` & `overhave-5.0.0/overhave/admin/views/testing_users.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from overhave.admin.views.base import ModelViewConfigured
 from overhave.factory import get_admin_factory
 from overhave.storage import FeatureTypeName
 from overhave.utils import get_current_time
 
 
 def _make_dict_from_model(model: type[BaseModel]) -> dict[str, int | str]:
-    return {key: value.type_.__name__ for key, value in model.__fields__.items()}
+    return {key: value.annotation.__name__ for key, value in model.model_fields.items() if value.annotation is not None}
 
 
 class TestUserView(ModelViewConfigured):
     """View for :class:`TestUser` table."""
 
     __test__ = False
 
@@ -64,18 +64,20 @@
             return _make_dict_from_model(parser)
         return None
 
     @staticmethod
     def _validate_json(model: db.TestUser) -> None:
         if not isinstance(model.specification, dict):
             raise ValidationError("Could not convert specified data into correct JSON!")
-        parser = get_admin_factory().context.project_settings.user_spec_template_mapping.get(model.feature_type.name)
+        parser: type[BaseModel] | None = get_admin_factory().context.project_settings.user_spec_template_mapping.get(
+            model.feature_type.name
+        )
         if parser is not None:
             try:
-                parser.parse_obj(model.specification)
+                parser.model_validate(model.specification)
             except ValueError:
                 raise ValidationError(f"Could not convert specified data into {parser.__name__} model!")
 
     def on_model_change(self, form: Form, model: db.TestUser, is_created: bool) -> None:
         self._feature_type = cast(FeatureTypeName, model.feature_type.name)
         self._validate_json(model)
         if is_created:
```

### Comparing `overhave-4.1.1/overhave/api/app.py` & `overhave-5.0.0/overhave/api/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import fastapi
 
 from overhave.api.auth import get_authorized_user
 from overhave.api.views import (
-    delete_test_user_handler,
+    delete_testuser_handler,
     docs,
     emulation_run_list_handler,
     favicon,
     feature_types_list_handler,
     get_features_handler,
     get_test_run_handler,
-    get_test_user_handler,
+    get_testuser_handler,
     login_for_access_token,
     run_tests_by_tag_handler,
     tags_item_handler,
     tags_list_handler,
-    test_user_get_spec_handler,
-    test_user_list_handler,
-    test_user_put_spec_handler,
+    testuser_get_spec_handler,
+    testuser_list_handler,
+    testuser_put_spec_handler,
 )
 from overhave.storage import (
     AuthToken,
     EmulationRunModel,
     FeatureModel,
     FeatureTypeModel,
     TagModel,
@@ -99,46 +99,46 @@
 
 
 def _get_testuser_router() -> fastapi.APIRouter:
     test_user_router = fastapi.APIRouter()
 
     test_user_router.add_api_route(
         "/",
-        get_test_user_handler,
+        get_testuser_handler,
         methods=["GET"],
         response_model=TestUserModel,
         summary="Get TestUser",
         description="Get test user full info by `user_id` or `user_key`",
     )
     test_user_router.add_api_route(
         "/list",
-        test_user_list_handler,
+        testuser_list_handler,
         methods=["GET"],
         response_model=list[TestUserModel],
         summary="Get list of TestUsers",
         description="Get list of test users with given `feature_type` and `allow_update`",
     )
     test_user_router.add_api_route(
         "/{user_id}",
-        delete_test_user_handler,
+        delete_testuser_handler,
         methods=["DELETE"],
         summary="Delete TestUser",
         description="Delete test user by `user_id`",
     )
     test_user_router.add_api_route(
         "/{user_id}/specification",
-        test_user_get_spec_handler,
+        testuser_get_spec_handler,
         methods=["GET"],
         response_model=TestUserSpecification,
         summary="Get TestUser specification",
         description="Get test user specification by `user_id`",
     )
     test_user_router.add_api_route(
         "/{user_id}/specification",
-        test_user_put_spec_handler,
+        testuser_put_spec_handler,
         methods=["PUT"],
         summary="Put test user specification",
         description="Update test user specification by `user_id` and given payload",
     )
     return test_user_router
```

### Comparing `overhave-4.1.1/overhave/api/auth/regular.py` & `overhave-5.0.0/overhave/api/auth/regular.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,20 +18,20 @@
     token: str = fastapi.Depends(oauth2_scheme),
     auth_settings: OverhaveApiAuthSettings = fastapi.Depends(get_api_auth_settings),
     storage: ISystemUserStorage = fastapi.Depends(get_system_user_storage),
 ) -> SystemUserModel:
     creds_exception = fastapi.HTTPException(
         status_code=HTTPStatus.UNAUTHORIZED,
         detail="Could not validate credentials",
-        headers=AUTH_HEADERS.dict(),
+        headers=AUTH_HEADERS.model_dump(),
     )
     try:
         token_data = get_token_data(auth_settings=auth_settings, token=token)
         if token_data is None:
             raise creds_exception
     except JWTError:
         raise creds_exception
     with db.create_session() as session:
         user = storage.get_user_by_credits(session=session, login=token_data.username)
         if user is None:
             raise creds_exception
-        return SystemUserModel.from_orm(user)
+        return SystemUserModel.model_validate(user)
```

### Comparing `overhave-4.1.1/overhave/api/auth/token.py` & `overhave-5.0.0/overhave/api/auth/token.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/api/deps.py` & `overhave-5.0.0/overhave/api/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/api/views/__init__.py` & `overhave-5.0.0/overhave/api/views/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from .emulation_views import emulation_run_list_handler
 from .extra_views import docs, favicon
 from .feature_type_views import feature_types_list_handler
 from .feature_views import get_features_handler
 from .tags_views import tags_item_handler, tags_list_handler
 from .testrun_views import get_test_run_handler, run_tests_by_tag_handler
 from .testuser_views import (
-    delete_test_user_handler,
-    get_test_user_handler,
-    test_user_get_spec_handler,
-    test_user_list_handler,
-    test_user_put_spec_handler,
+    delete_testuser_handler,
+    get_testuser_handler,
+    testuser_get_spec_handler,
+    testuser_list_handler,
+    testuser_put_spec_handler,
 )
```

### Comparing `overhave-4.1.1/overhave/api/views/auth_views.py` & `overhave-5.0.0/overhave/api/views/auth_views.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,12 +20,12 @@
     with db.create_session() as session:
         if not storage.get_user_by_credits(
             session=session, login=form_data.username, password=SecretStr(form_data.password)
         ):
             raise fastapi.HTTPException(
                 status_code=HTTPStatus.UNAUTHORIZED,
                 detail="Incorrect username or password",
-                headers=AUTH_HEADERS.dict(),
+                headers=AUTH_HEADERS.model_dump(),
             )
     expires_at = get_current_time() + auth_settings.access_token_expire_timedelta
     access_token = create_access_token(auth_settings=auth_settings, username=form_data.username, expires_at=expires_at)
     return AuthToken(access_token=access_token, expires_at=expires_at)
```

### Comparing `overhave-4.1.1/overhave/api/views/emulation_views.py` & `overhave-5.0.0/overhave/api/views/emulation_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/api/views/extra_views.py` & `overhave-5.0.0/overhave/api/views/extra_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/api/views/feature_views.py` & `overhave-5.0.0/overhave/api/views/feature_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/api/views/tags_views.py` & `overhave-5.0.0/overhave/api/views/tags_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/api/views/testrun_views.py` & `overhave-5.0.0/overhave/api/views/testrun_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 def run_tests_by_tag_handler(
     tag_value: str,
     feature_storage: IFeatureStorage = fastapi.Depends(get_feature_storage),
     tag_storage: IFeatureTagStorage = fastapi.Depends(get_feature_tag_storage),
     scenario_storage: IScenarioStorage = fastapi.Depends(get_scenario_storage),
     test_run_storage: TestRunStorage = fastapi.Depends(get_test_run_storage),
     redis_producer: RedisProducer = fastapi.Depends(get_redis_producer),
-) -> list[int]:
+) -> list[str]:
     tag_model = tags_item_handler(value=tag_value, feature_tag_storage=tag_storage)
     features = feature_storage.get_features_by_tag(tag_id=tag_model.id)
     if not features:
         raise fastapi.HTTPException(
             status_code=HTTPStatus.BAD_REQUEST, detail=f"Features with tag='{tag_value}' do not exist"
         )
-    test_run_ids: list[int] = []
+    test_run_ids: list[str] = []
     for feature in features:
         scenario = scenario_storage.get_scenario_by_feature_id(feature.id)
         test_run_id = test_run_storage.create_testrun(scenario_id=scenario.id, executed_by=feature.last_edited_by)
         redis_producer.add_task(TestRunTask(data=TestRunData(test_run_id=test_run_id)))
-        test_run_ids.append(test_run_id)
+        test_run_ids.append(str(test_run_id))
     return test_run_ids
```

### Comparing `overhave-4.1.1/overhave/api/views/testuser_views.py` & `overhave-5.0.0/overhave/api/views/testuser_views.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,61 +15,61 @@
     TestUserSpecification,
     TestUserUpdatingNotAllowedError,
 )
 
 logger = logging.getLogger(__name__)
 
 
-def _get_test_user_by_id_handler(user_id: int, test_user_storage: ITestUserStorage) -> TestUserModel:
+def _get_testuser_by_id_handler(user_id: int, test_user_storage: ITestUserStorage) -> TestUserModel:
     logger.info("Getting %s with user_id=%s...", TestUserModel.__name__, user_id)
     test_user = test_user_storage.get_testuser_model_by_id(user_id)
     if test_user is None:
         raise fastapi.HTTPException(
             status_code=HTTPStatus.BAD_REQUEST, detail=f"User with id={user_id} does not exist!"
         )
     return test_user
 
 
-def _get_test_user_by_key_handler(user_key: str, test_user_storage: ITestUserStorage) -> TestUserModel:
+def _get_testuser_by_key_handler(user_key: str, test_user_storage: ITestUserStorage) -> TestUserModel:
     logger.info("Getting %s with user_key='%s'...", TestUserModel.__name__, user_key)
     test_user = test_user_storage.get_testuser_model_by_key(user_key)
     if test_user is None:
         raise fastapi.HTTPException(
             status_code=HTTPStatus.BAD_REQUEST, detail=f"User with key='{user_key}' does not exist!"
         )
     return test_user
 
 
-def get_test_user_handler(
+def get_testuser_handler(
     user_id: int | None = None,
     user_key: str | None = None,
     test_user_storage: ITestUserStorage = fastapi.Depends(get_test_user_storage),
 ) -> TestUserModel:
     if user_id is not None:
-        return _get_test_user_by_id_handler(user_id=user_id, test_user_storage=test_user_storage)
+        return _get_testuser_by_id_handler(user_id=user_id, test_user_storage=test_user_storage)
     if user_key is not None:
-        return _get_test_user_by_key_handler(user_key=user_key, test_user_storage=test_user_storage)
+        return _get_testuser_by_key_handler(user_key=user_key, test_user_storage=test_user_storage)
     raise fastapi.HTTPException(
         status_code=HTTPStatus.BAD_REQUEST, detail="'user_id' or 'user_key' query parameter should be set!"
     )
 
 
-def delete_test_user_handler(
+def delete_testuser_handler(
     user_id: int,
     test_user_storage: ITestUserStorage = fastapi.Depends(get_test_user_storage),
 ) -> None:
     try:
         test_user_storage.delete_test_user(user_id)
     except TestUserDoesNotExistError:
         raise fastapi.HTTPException(
             status_code=HTTPStatus.BAD_REQUEST, detail=f"User with id={user_id} does not exist!"
         )
 
 
-def test_user_list_handler(
+def testuser_list_handler(
     feature_type: FeatureTypeName,
     allow_update: bool,
     feature_type_storage: IFeatureTypeStorage = fastapi.Depends(get_feature_type_storage),
     test_user_storage: ITestUserStorage = fastapi.Depends(get_test_user_storage),
 ) -> list[TestUserModel]:
     logger.info(
         "Getting %s list with feature_type=%s and allow_update=%s ...",
@@ -85,29 +85,31 @@
             )
     except FeatureTypeNotExistsError:
         raise fastapi.HTTPException(
             status_code=HTTPStatus.BAD_REQUEST, detail=f"FeatureType with name='{feature_type}' does not exist!"
         )
 
 
-def test_user_get_spec_handler(
+def testuser_get_spec_handler(
     user_id: int, test_user_storage: ITestUserStorage = fastapi.Depends(get_test_user_storage)
 ) -> TestUserSpecification:
-    test_user = _get_test_user_by_id_handler(user_id=user_id, test_user_storage=test_user_storage)
+    test_user = _get_testuser_by_id_handler(user_id=user_id, test_user_storage=test_user_storage)
     return test_user.specification
 
 
-def test_user_put_spec_handler(
+def testuser_put_spec_handler(
     user_id: int,
-    specification: TestUserSpecification,
+    specification: dict[str, str | None],
     test_user_storage: ITestUserStorage = fastapi.Depends(get_test_user_storage),
 ) -> None:
     logger.info("Updating %s for user_id=%s...", TestUserSpecification.__name__, user_id)
     try:
-        test_user_storage.update_test_user_specification(user_id=user_id, specification=specification)
+        test_user_storage.update_test_user_specification(
+            user_id=user_id, specification=TestUserSpecification(specification)
+        )
     except TestUserDoesNotExistError:
         raise fastapi.HTTPException(
             status_code=HTTPStatus.BAD_REQUEST, detail=f"User with id={user_id} does not exist!"
         )
     except TestUserUpdatingNotAllowedError:
         raise fastapi.HTTPException(
             status_code=HTTPStatus.BAD_REQUEST, detail=f"User's updating with id={user_id} not allowed!"
```

### Comparing `overhave-4.1.1/overhave/base_settings.py` & `overhave-5.0.0/overhave/base_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,59 +3,50 @@
 import socket
 from logging.config import DictConfigurator
 from typing import Any
 
 import sqlalchemy as sa
 import sqlalchemy.engine
 import sqlalchemy.exc
-from pydantic import BaseSettings, Field, validator
+from pydantic import field_validator
+from pydantic_settings import BaseSettings
 from sqlalchemy.pool import Pool, SingletonThreadPool
 
 OVERHAVE_ENV_PREFIX = "OVERHAVE_"
 
 
 class BaseOverhavePrefix(BaseSettings):
     """Possibility to change Overhave default settings from environment."""
 
     class Config:
         env_prefix = OVERHAVE_ENV_PREFIX
 
 
-class SAUrl(sqlalchemy.engine.URL):  # SQLAlchemy2.0 - sa.URL
-    """Custom URL for Pydantic BaseSettings validation."""
-
-    @classmethod
-    def __get_validators__(cls):  # type: ignore
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, v: str) -> sqlalchemy.engine.URL:  # SQLAlchemy2.0 - sa.URL
-        try:
-            return sqlalchemy.engine.make_url(v)  # SQLAlchemy2.0 - sa.make_url
-        except sqlalchemy.exc.ArgumentError as e:
-            raise ValueError from e
+def _as_alchemy_url(db_url: str) -> sqlalchemy.engine.URL:  # SQLAlchemy2.0 - sa.make_url
+    try:
+        return sqlalchemy.engine.make_url(db_url)  # SQLAlchemy2.0 - sa.make_url
+    except sqlalchemy.exc.ArgumentError as e:
+        raise ValueError from e
 
 
 class DataBaseSettings(BaseOverhavePrefix):
     """Overhave database settings."""
 
-    db_url: SAUrl = Field(
-        SAUrl.validate("postgresql://postgres:postgres@localhost/overhave")  # type: ignore[assignment]
-    )
+    db_url: str = "postgresql://postgres:postgres@localhost/overhave"
     db_pool_recycle: int = 500
     db_pool_size: int = 6
     db_echo: bool = False
     db_application_name: str = socket.gethostname()
     db_connect_timeout: int = 30
     db_poolclass: type[Pool] = SingletonThreadPool
 
     def _create_engine(self) -> sqlalchemy.engine.Engine:  # SQLAlchemy2.0 - sa.Engine
         return sa.engine_from_config(
             {
-                "url": self.db_url,
+                "url": _as_alchemy_url(self.db_url),
                 "pool_recycle": self.db_pool_recycle,
                 "pool_pre_ping": True,
                 "pool_size": self.db_pool_size,
                 "poolclass": self.db_poolclass,
                 "connect_args": {
                     "connect_timeout": self.db_connect_timeout,
                     "application_name": self.db_application_name,
@@ -73,15 +64,15 @@
 
 class LoggingSettings(BaseOverhavePrefix):
     """Overhave logging settings."""
 
     log_level: str = logging.getLevelName(logging.INFO)
     log_config: dict[str, Any] = {}
 
-    @validator("log_config", each_item=True)
+    @field_validator("log_config", check_fields=True)
     def dict_config_validator(cls, v: dict[str, Any]) -> DictConfigurator | None:
         if not v:
             return None
         return DictConfigurator(v)
 
     def setup_logging(self) -> None:
         if isinstance(self.log_config, DictConfigurator):
```

### Comparing `overhave-4.1.1/overhave/cli/admin.py` & `overhave-5.0.0/overhave/cli/admin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/cli/api.py` & `overhave-5.0.0/overhave/cli/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     workers: int = typer.Option(1, "-w", "--workers", help="Uvicorn workers"),
 ) -> None:
     """Run Overhave API."""
     from overhave.api.asgi import app
     from overhave.api.settings import OverhaveUvicornApiSettings
 
     settings = OverhaveUvicornApiSettings(port=port, workers=workers)
-    uvicorn.run(app, **settings.dict())
+    uvicorn.run(app, **settings.model_dump())
```

### Comparing `overhave-4.1.1/overhave/cli/consumers.py` & `overhave-5.0.0/overhave/cli/consumers.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/cli/db_cmds/group.py` & `overhave-5.0.0/overhave/cli/db_cmds/group.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/cli/db_cmds/regular.py` & `overhave-5.0.0/overhave/cli/db_cmds/regular.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/cli/s3.py` & `overhave-5.0.0/overhave/cli/s3.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/cli/synchronizer.py` & `overhave-5.0.0/overhave/cli/synchronizer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/db/base.py` & `overhave-5.0.0/overhave/db/base.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/db/statuses.py` & `overhave-5.0.0/overhave/db/statuses.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/db/tables.py` & `overhave-5.0.0/overhave/db/tables.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/db/users.py` & `overhave-5.0.0/overhave/db/users.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/db/utils.py` & `overhave-5.0.0/overhave/db/utils.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/emulation/emulator.py` & `overhave-5.0.0/overhave/emulation/emulator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/entities/__init__.py` & `overhave-5.0.0/overhave/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/entities/archiver.py` & `overhave-5.0.0/overhave/entities/archiver.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/entities/auth_managers/default.py` & `overhave-5.0.0/overhave/entities/auth_managers/default.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     """
 
     def authorize_user(self, username: str, password: SecretStr) -> SystemUserModel | None:
         with db.create_session() as session:
             user = self._system_user_storage.get_user_by_credits(session=session, login=username, password=password)
             if user is None:
                 return None
-            return SystemUserModel.from_orm(user)
+            return SystemUserModel.model_validate(user)
```

### Comparing `overhave-4.1.1/overhave/entities/auth_managers/ldap/manager.py` & `overhave-5.0.0/overhave/entities/auth_managers/ldap/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,18 +61,18 @@
             intended_user_role = self._user_role_by_admin_group_entry(user_has_admin_group)
 
             user = self._system_user_storage.get_user_by_credits(session=session, login=username)
             if user is not None:
                 if user.role is db.Role.user and user.role is not intended_user_role:
                     user.role = intended_user_role
                     session.flush()
-                return SystemUserModel.from_orm(user)
+                return SystemUserModel.model_validate(user)
 
             logger.debug("Have not found user with username '%s'!", username)
             if self._can_user_be_created(
                 session=session, user_has_admin_group=user_has_admin_group, user_groups=user_groups
             ):
                 user = self._system_user_storage.create_user(session=session, login=username, role=intended_user_role)
-                return SystemUserModel.from_orm(user)
+                return SystemUserModel.model_validate(user)
 
         logger.debug("Received user groups (%s) are not supplied with exist groups!", user_groups)
         return None
```

### Comparing `overhave-4.1.1/overhave/entities/auth_managers/secret_mixin.py` & `overhave-5.0.0/overhave/entities/auth_managers/secret_mixin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/entities/auth_managers/simple.py` & `overhave-5.0.0/overhave/entities/auth_managers/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,9 +28,9 @@
         with db.create_session() as session:
             user = self._system_user_storage.get_user_by_credits(session=session, login=username)
             if user is None:
                 user = self._system_user_storage.create_user(session=session, login=username, password=password)
             if user.password is None:
                 raise NullablePasswordError(f"User with id={user.id} has not got password!")
             if user.password == password.get_secret_value():
-                return SystemUserModel.from_orm(user)
+                return SystemUserModel.model_validate(user)
         return None
```

### Comparing `overhave-4.1.1/overhave/entities/feature/extractor.py` & `overhave-5.0.0/overhave/entities/feature/extractor.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/entities/file_extractor.py` & `overhave-5.0.0/overhave/entities/file_extractor.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/entities/git_initializer.py` & `overhave-5.0.0/overhave/entities/git_initializer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/entities/language/prefixes.py` & `overhave-5.0.0/overhave/entities/language/prefixes.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/entities/report_manager/report_manager.py` & `overhave-5.0.0/overhave/entities/report_manager/report_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,9 +118,10 @@
             return resolution
 
         unpacked_report = self._archive_manager.unpack_path(
             path=zip_report_path, extension=self._settings.archive_extension
         )
         zip_report_path.unlink()
         logger.info("Unpacked Allure report: %s", unpacked_report)
-        resolution.exists = True
-        return resolution
+        return ReportPresenceResolution(
+            exists=True, s3_enabled=self._s3_manager.enabled, report_status=test_run.report_status
+        )
```

### Comparing `overhave-4.1.1/overhave/entities/settings.py` & `overhave-5.0.0/overhave/entities/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,46 @@
+from datetime import timedelta
 from pathlib import Path
 from typing import Any, Sequence
 
 import httpx
 from flask_admin.contrib.sqla import ModelView
-from pydantic import root_validator, validator
-from pydantic.datetime_parse import timedelta
+from pydantic import Field, field_validator, model_validator
 
 from overhave.base_settings import BaseOverhavePrefix
 from overhave.entities.language import StepPrefixesModel
 
 
 class OverhaveAdminSettings(BaseOverhavePrefix):
     """Settings for Overhave Flask Admin customization."""
 
     # Path to custom index template. By default, contains Overhave project info.
-    index_template_path: Path | None
+    index_template_path: Path | None = Field(default=None)
 
     # Custom SQLAlchemy ModelViews for Overhave admin panel
-    custom_views: Sequence[ModelView] | None
+    custom_views: Sequence[ModelView] | None = Field(default=None)
 
     # Enable testing with test execution consumer, based on Redis tasks. Enabled by default.
     # When disabled - all test runs will be executed with :class:`Threadpool`.
     consumer_based: bool = True
 
     # Threadpool size for admin service
     threadpool_process_num: int = 5
 
     # Force filling the tasks field in feature creation
     strict_feature_tasks: bool = False
 
     # Link to support chat
-    support_chat_url: httpx.URL | None
+    support_chat_url: httpx.URL | None = Field(default=None)
 
 
 class OverhaveLanguageSettings(BaseOverhavePrefix):
     """Settings for language definitions."""
 
-    step_prefixes: StepPrefixesModel | None
+    step_prefixes: StepPrefixesModel | None = Field(default=None)
 
 
 class OverhaveFileSettings(BaseOverhavePrefix):
     """Settings for scenario file savings."""
 
     feature_suffix: str = ".feature"
     fixture_suffix: str = ".py"
@@ -64,31 +64,29 @@
 
     # Base directory for pytest-bdd steps, , by default - root_dir / 'steps'
     steps_dir: Path
 
     # Temporary directory for scenarios test runs
     tmp_dir: Path = Path("/tmp/overhave")  # noqa: S108
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     def validate_dirs(cls, values: dict[str, Any]) -> dict[str, Any]:
         root_dir = values.get("root_dir")
         if root_dir:
             for directory in ("features_dir", "fixtures_dir", "steps_dir"):
                 if values.get(directory):
                     continue
                 values[directory] = Path(root_dir) / directory.replace("_dir", "")
         return values
 
-    @validator("steps_dir")
-    def validate_nesting(cls, v: Path, values: dict[str, Any]) -> Path:
-        validate_steps_dir = values["validate_steps_dir"]
-        if validate_steps_dir:
-            work_dir: Path = values["work_dir"]
-            v.relative_to(work_dir)
-        return v
+    @model_validator(mode="after")  # type: ignore[misc]
+    def validate_nesting(self) -> "OverhaveFileSettings":
+        if self.validate_steps_dir and not self.steps_dir.relative_to(self.work_dir):
+            raise ValueError("'steps_dir' is not relative to 'work_dir', but should be!")
+        return self  # type: ignore[return-value]
 
     @property
     def tmp_features_dir(self) -> Path:
         return self.tmp_dir / "features"
 
     @property
     def tmp_fixtures_dir(self) -> Path:
@@ -120,43 +118,43 @@
     # Path for emulation core application, such as GoTTY
     emulation_core_path: str = "/gotty"
 
     # All emulation core application prefixes for execution
     emulation_prefix: str = "--permit-write --once --address {address} --port {port} --timeout {timeout}"
 
     # Specific terminal tool startup command with relative `feature_type`, for example: `myapp {feature_type}`
-    emulation_base_cmd: str | None
+    emulation_base_cmd: str | None = Field(default=None)
     # Terminal tool command postfix with specified user `name` and `model`, for example: `--name={name} --model={model}`
     # If it is no need in use - may be optional.
-    emulation_postfix: str | None
+    emulation_postfix: str | None = Field(default=None)
 
     # Optional additional terminal tool usage description
-    emulation_desc_link: str | None
+    emulation_desc_link: str | None = Field(default=None)
 
     emulation_bind_ip: str = "0.0.0.0"  # noqa: S104
     # Ports for emulation binding. Expects as string with format `["port1", "port2", ...]`
     emulation_ports: list[int] = [8080]
 
     # As a real service, should be used follow path: `http://my-service.domain/mount`
     # where `emulation_service_url` = `http://my-service.domain` - URL for service,
     # and `emulation_service_mount` = `mount` - mount point for service redirection.
     # If `emulation_service_mount` is `None` - this is localhost debug.
     emulation_service_url: httpx.URL = httpx.URL("http://localhost")
-    emulation_service_mount: str | None
+    emulation_service_mount: str | None = Field(default=None)
 
     # Wait until emulation become served
     emulation_wait_timeout: timedelta = timedelta(seconds=300)
 
-    @validator("emulation_service_url", pre=True)
+    @field_validator("emulation_service_url", mode="before")
     def validate_url(cls, v: str | httpx.URL) -> httpx.URL:
         if isinstance(v, str):
             return httpx.URL(v)
         return v
 
-    @validator("emulation_ports", pre=True)
+    @field_validator("emulation_ports", mode="before")
     def validate_ports(cls, v: list[int] | str) -> list[int]:
         if isinstance(v, str):
             return [int(x.strip()) for x in v.split(",")]
         return v
 
     def get_emulation_url(self, port: str) -> httpx.URL:
         if isinstance(self.emulation_service_mount, str):
```

### Comparing `overhave-4.1.1/overhave/factory/__init__.py` & `overhave-5.0.0/overhave/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/factory/base_factory.py` & `overhave-5.0.0/overhave/factory/base_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/factory/components/admin_factory.py` & `overhave-5.0.0/overhave/factory/components/admin_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/factory/components/emulation_factory.py` & `overhave-5.0.0/overhave/factory/components/emulation_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/factory/components/publication_factory.py` & `overhave-5.0.0/overhave/factory/components/publication_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/factory/components/synchronizer_factory.py` & `overhave-5.0.0/overhave/factory/components/synchronizer_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/factory/components/test_execution_factory.py` & `overhave-5.0.0/overhave/factory/components/test_execution_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/factory/consumer_factory.py` & `overhave-5.0.0/overhave/factory/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/factory/context/__init__.py` & `overhave-5.0.0/overhave/factory/context/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/factory/context/admin_context.py` & `overhave-5.0.0/overhave/factory/context/admin_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/factory/context/base_context.py` & `overhave-5.0.0/overhave/factory/context/base_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import cast
 
-from pydantic import BaseSettings
+from pydantic_settings import BaseSettings
 
 from overhave.entities import (
     OverhaveEmulationSettings,
     OverhaveFileSettings,
     OverhaveLanguageSettings,
     OverhaveReportManagerSettings,
 )
```

### Comparing `overhave-4.1.1/overhave/factory/context/publication_context.py` & `overhave-5.0.0/overhave/factory/context/publication_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/factory/context/synchronizer_context.py` & `overhave-5.0.0/overhave/factory/context/synchronizer_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/factory/context/test_execution_context.py` & `overhave-5.0.0/overhave/factory/context/test_execution_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/factory/getters.py` & `overhave-5.0.0/overhave/factory/getters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/metrics/client/container.py` & `overhave-5.0.0/overhave/metrics/client/container.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/metrics/getters.py` & `overhave-5.0.0/overhave/metrics/getters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/publication/base_publisher.py` & `overhave-5.0.0/overhave/publication/base_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/publication/errors.py` & `overhave-5.0.0/overhave/publication/errors.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/publication/git_publisher.py` & `overhave-5.0.0/overhave/publication/git_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/publication/gitlab/gitlab_publisher.py` & `overhave-5.0.0/overhave/publication/gitlab/gitlab_publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             project_id=self._git_publisher_settings.repository_id,
             title=context.feature.name,
             source_branch=context.target_branch,
             target_branch=self._git_publisher_settings.target_branch,
             description=self._compile_publication_description(context),
             reviewer_ids=self._git_publisher_settings.get_reviewers(feature_type=context.feature.feature_type.name),
         )
-        logger.info("Prepared merge-request: %s", merge_request.json(by_alias=True))
+        logger.info("Prepared merge-request: %s", merge_request.model_dump_json(by_alias=True))
         try:
             token = (
                 self._gitlab_client._settings.auth_token or self._tokenizer_client.get_token(draft_id=draft_id).token
             )
             response = self._gitlab_client.send_merge_request(
                 merge_request=merge_request, token=token, repository_id=self._git_publisher_settings.repository_id
             )
```

### Comparing `overhave-4.1.1/overhave/publication/gitlab/settings.py` & `overhave-5.0.0/overhave/publication/gitlab/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/publication/gitlab/tokenizer/client.py` & `overhave-5.0.0/overhave/publication/gitlab/tokenizer/client.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/publication/gitlab/tokenizer/settings.py` & `overhave-5.0.0/overhave/publication/gitlab/tokenizer/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Any
-
 import httpx
-from pydantic import validator
+from pydantic import field_validator
+from pydantic_core.core_schema import FieldValidationInfo
 
 from overhave.transport.http import BaseHttpClientSettings
 from overhave.utils import make_url
 
 
 class TokenizerClientSettings(BaseHttpClientSettings):
     """Important environments and settings for :class:`TokenizerClient`."""
@@ -15,16 +14,16 @@
     initiator: str = "Overhave"
     remote_key: str | None = None
     remote_key_name: str | None = None
 
     class Config:
         env_prefix = "OVERHAVE_GITLAB_TOKENIZER_"
 
-    @validator("url", pre=True)
+    @field_validator("url", mode="before")
     def make_url(cls, v: str | None) -> httpx.URL | None:
         return make_url(v)
 
-    @validator("url", "remote_key", "remote_key_name")
-    def validate_remote_key_and_initiator(cls, v: str | None, values: dict[str, Any]) -> str | None:
-        if values.get("enabled") and not isinstance(v, str):
+    @field_validator("url", "remote_key", "remote_key_name", mode="after")
+    def validate_remote_key_and_initiator(cls, v: str | None, values: FieldValidationInfo) -> str | None:
+        if values.data.get("enabled") and not isinstance(v, str):
             raise ValueError("Please verify that url, remote_key and remote_key_name variables are not nullable!")
         return v
```

### Comparing `overhave-4.1.1/overhave/publication/settings.py` & `overhave-5.0.0/overhave/publication/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/publication/stash/settings.py` & `overhave-5.0.0/overhave/publication/stash/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/publication/stash/stash_publisher.py` & `overhave-5.0.0/overhave/publication/stash/stash_publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             title=context.feature.name,
             description=self._compile_publication_description(context),
             open=True,
             fromRef=StashBranch(id=context.target_branch, repository=self._git_publisher_settings.repository),
             toRef=self._git_publisher_settings.target_branch,
             reviewers=self._git_publisher_settings.get_reviewers(feature_type=context.feature.feature_type.name),
         )
-        logger.info("Prepared pull-request: %s", pull_request.json(by_alias=True))
+        logger.info("Prepared pull-request: %s", pull_request.model_dump_json(by_alias=True))
         try:
             response = self._client.send_pull_request(pull_request)
             if isinstance(response, StashPrCreationResponse):
                 self._draft_storage.save_response_as_created(
                     draft_id=draft_id,
                     pr_url=response.get_pr_url(),
                     published_at=response.created_date,
```

### Comparing `overhave-4.1.1/overhave/pytest_plugin/config_injector.py` & `overhave-5.0.0/overhave/pytest_plugin/config_injector.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/pytest_plugin/deps.py` & `overhave-5.0.0/overhave/pytest_plugin/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/pytest_plugin/helpers/__init__.py` & `overhave-5.0.0/overhave/pytest_plugin/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/description_manager.py` & `overhave-5.0.0/overhave/pytest_plugin/helpers/allure_utils/description_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/links.py` & `overhave-5.0.0/overhave/pytest_plugin/helpers/allure_utils/links.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/severity.py` & `overhave-5.0.0/overhave/pytest_plugin/helpers/allure_utils/severity.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py` & `overhave-5.0.0/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/pytest_plugin/helpers/bdd_item.py` & `overhave-5.0.0/overhave/pytest_plugin/helpers/bdd_item.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/pytest_plugin/helpers/parsed_info.py` & `overhave-5.0.0/overhave/pytest_plugin/helpers/parsed_info.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/pytest_plugin/helpers/tag_controller.py` & `overhave-5.0.0/overhave/pytest_plugin/helpers/tag_controller.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/pytest_plugin/plugin.py` & `overhave-5.0.0/overhave/pytest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/pytest_plugin/plugin_resolver.py` & `overhave-5.0.0/overhave/pytest_plugin/plugin_resolver.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/pytest_plugin/proxy_manager.py` & `overhave-5.0.0/overhave/pytest_plugin/proxy_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/scenario/__init__.py` & `overhave-5.0.0/overhave/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/scenario/compiler/compiler.py` & `overhave-5.0.0/overhave/scenario/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/scenario/compiler/settings.py` & `overhave-5.0.0/overhave/scenario/compiler/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/scenario/file_manager/file_manager.py` & `overhave-5.0.0/overhave/scenario/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/scenario/file_manager/settings.py` & `overhave-5.0.0/overhave/scenario/file_manager/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
-from typing import Any, Mapping
+from typing import Mapping
 
 import httpx
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator, model_validator
 
 from overhave.base_settings import BaseOverhavePrefix
 from overhave.utils import make_url
 
 
 class EmptyTaskTrackerURLError(ValueError):
     """Exception for situation with empty ```task_tracker_url``` while trying to ```get_task_link```."""
@@ -41,25 +41,25 @@
     # Git project URL
     git_project_url: httpx.URL | None
 
     # Templates are used for creation of test user and system specifications.
     # Keys for specification mapping are still the same - feature types.
     user_spec_template_mapping: Mapping[str, type[BaseModel]] = {}
 
-    @validator("task_tracker_url", pre=True)
+    @model_validator(mode="after")
+    def validate_links_keyword(self: "OverhaveProjectSettings") -> "OverhaveProjectSettings":  # type: ignore[misc]
+        if isinstance(self.tasks_keyword, str) and self.task_tracker_url is None:
+            raise ValueError("'task_tracker_url' should be specified in case of 'tasks_keyword' usage!")
+        return self
+
+    @field_validator("task_tracker_url", mode="before")
     def make_tasktracker_url(cls, v: str | None) -> httpx.URL | None:
         return make_url(v)
 
-    @validator("tasks_keyword")
-    def validate_links_keyword(cls, v: str | None, values: dict[str, Any]) -> str | None:
-        if isinstance(v, str) and values.get("task_tracker_url") is None:
-            raise ValueError("Task tracker URL should be specified in case of links keyword usage!")
-        return v
-
-    @validator("git_project_url", pre=True)
+    @field_validator("git_project_url", mode="before")
     def make_git_project_url(cls, v: str | None) -> httpx.URL | None:
         return make_url(v)
 
     def get_task_link(self, link: str) -> httpx.URL:
         if isinstance(self.task_tracker_url, httpx.URL):
             return httpx.URL(f"{self.task_tracker_url}/{link}")
         raise EmptyTaskTrackerURLError("Task tracker URL is None, so could not create link URL!")
```

### Comparing `overhave-4.1.1/overhave/scenario/parser/models.py` & `overhave-5.0.0/overhave/scenario/parser/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,39 @@
+from dataclasses import dataclass, field
 from datetime import datetime
 
 import allure
-from pydantic import BaseModel
 
 from overhave.storage import FeatureTypeName
 
 
-class FeatureInfo(BaseModel):
+@dataclass
+class FeatureInfo:
     """Model for feature info keeping."""
 
-    id: int | None
-    name: str | None
-    type: FeatureTypeName | None
-    tags: list[str] | None
-    severity: allure.severity_level | None
-    author: str | None
-    last_edited_by: str | None
-    last_edited_at: datetime | None
-    tasks: list[str] | None
-    scenarios: str | None
+    id: int | None = None
+    name: str | None = None
+    type: FeatureTypeName | None = None
+    tags: list[str] | None = None
+    severity: allure.severity_level | None = None
+    author: str | None = None
+    last_edited_by: str | None = None
+    last_edited_at: datetime | None = None
+    tasks: list[str] | None = None
+    scenarios: str | None = None
 
 
-class StrictFeatureInfo(BaseModel):
+@dataclass
+class StrictFeatureInfo:
     """Model for feature info keeping with strict presence of fields."""
 
     id: int
     name: str
     type: FeatureTypeName
-    tags: list[str] = []
-    severity: allure.severity_level = allure.severity_level.NORMAL
     author: str
     last_edited_by: str
     last_edited_at: datetime
-    tasks: list[str] = []
     scenarios: str
+
+    tags: list[str] = field(default_factory=list)
+    severity: allure.severity_level = allure.severity_level.NORMAL
+    tasks: list[str] = field(default_factory=list)
```

### Comparing `overhave-4.1.1/overhave/scenario/parser/parser.py` & `overhave-5.0.0/overhave/scenario/parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import re
+from dataclasses import asdict
 from datetime import datetime
 from functools import cached_property
 from typing import Sequence
 
 import allure
 from pytest_bdd import types as default_types
 
@@ -189,10 +190,10 @@
         feature_info = self._parse_feature_info(header)
         feature_info.scenarios = blocks_delimiter.join(blocks).replace(indent_substitute, indent)
         if not self._parser_settings.parser_strict_mode:
             return feature_info
         if feature_info.id is None:
             raise NullableFeatureIdError("Feature has not got specified ID!")
         try:
-            return StrictFeatureInfo(**feature_info.dict())
+            return StrictFeatureInfo(**asdict(feature_info))
         except ValueError as err:
             raise StrictFeatureParsingError("Could not parse feature to StrictFeatureInfo!") from err
```

### Comparing `overhave-4.1.1/overhave/scenario/validator/duplicate_id_mixin.py` & `overhave-5.0.0/overhave/scenario/validator/duplicate_id_mixin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/scenario/validator/validator.py` & `overhave-5.0.0/overhave/scenario/validator/validator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/storage/__init__.py` & `overhave-5.0.0/overhave/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/storage/api_auth_storage.py` & `overhave-5.0.0/overhave/storage/api_auth_storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import abc
 from datetime import datetime
+from typing import Literal
 
-from pydantic.fields import Field
-from pydantic.main import BaseModel
+from pydantic import BaseModel
 
 from overhave.utils import get_current_time
 
 
 class AuthToken(BaseModel):
     """Model for OAuth2 auth_managers token."""
 
     access_token: str
     expires_at: datetime
-    token_type: str = Field("Bearer", const=True)
+    token_type: Literal["Bearer"] = "Bearer"
 
 
 class IAuthStorage(abc.ABC):
     """Abstract storage for auth_managers tokens."""
 
     @abc.abstractmethod
     def get_auth_token(self, username: str) -> AuthToken | None:
```

### Comparing `overhave-4.1.1/overhave/storage/converters.py` & `overhave-5.0.0/overhave/storage/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 TestUserSpecification = NewType("TestUserSpecification", dict[str, str | None])
 
 
 class _SqlAlchemyOrmModel(BaseModel):
     """:class:`BaseModel` with enabled `orm_mode`."""
 
     class Config:
-        orm_mode = True
+        from_attributes = True
 
 
 class SystemUserModel(_SqlAlchemyOrmModel):
     """Model for :class:`UserRole`."""
 
     id: int
     login: str
```

### Comparing `overhave-4.1.1/overhave/storage/draft_storage.py` & `overhave-5.0.0/overhave/storage/draft_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 class DraftStorage(IDraftStorage):
     """Class for scenario versions storage."""
 
     @staticmethod
     def draft_model_by_id(session: so.Session, draft_id: int) -> DraftModel:
         draft = session.query(db.Draft).filter(db.Draft.id == draft_id).one()
-        return DraftModel.from_orm(draft)
+        return DraftModel.model_validate(draft)
 
     @staticmethod
     def get_last_published_at_for_feature(feature_id: int) -> datetime | None:
         with db.create_session() as session:
             last_draft_with_published_at = (
                 session.query(db.Draft)
                 .filter(db.Draft.feature_id == feature_id, db.Draft.published_at.isnot(None))
```

### Comparing `overhave-4.1.1/overhave/storage/emulation_storage.py` & `overhave-5.0.0/overhave/storage/emulation_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import abc
 import logging
 import socket
 from typing import cast
 
 import sqlalchemy as sa
 import sqlalchemy.orm as so
-from pydantic.tools import parse_obj_as
 
 from overhave import db
 from overhave.entities.settings import OverhaveEmulationSettings
 from overhave.storage import EmulationRunModel
 from overhave.utils import get_current_time
 
 logger = logging.getLogger(__name__)
@@ -101,15 +100,15 @@
 
     def get_requested_emulation_run(self, emulation_run_id: int) -> EmulationRunModel:
         with db.create_session() as session:
             emulation_run = session.query(db.EmulationRun).filter(db.EmulationRun.id == emulation_run_id).one()
             emulation_run.status = db.EmulationStatus.REQUESTED
             emulation_run.port = self._get_next_port(session)
             emulation_run.changed_at = get_current_time()
-            return EmulationRunModel.from_orm(emulation_run)
+            return EmulationRunModel.model_validate(emulation_run)
 
     def set_emulation_run_status(self, emulation_run_id: int, status: db.EmulationStatus) -> None:
         with db.create_session() as session:
             session.execute(
                 sa.update(db.EmulationRun)
                 .where(db.EmulationRun.id == emulation_run_id)
                 .values(status=status, changed_at=get_current_time())
@@ -131,8 +130,8 @@
                 .with_entities(db.Emulation.id)
                 .filter(db.Emulation.test_user_id == test_user_id)
                 .scalar_subquery()
             )
             emulation_runs = (
                 session.query(db.EmulationRun).where(db.EmulationRun.emulation_id.in_(emulation_ids_query)).all()
             )
-            return parse_obj_as(list[EmulationRunModel], emulation_runs)
+            return [EmulationRunModel.model_validate(x) for x in emulation_runs]
```

### Comparing `overhave-4.1.1/overhave/storage/feature_storage.py` & `overhave-5.0.0/overhave/storage/feature_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import abc
 import logging
 from typing import Iterable, cast
 
 import sqlalchemy as sa
 import sqlalchemy.orm as so
-from pydantic.tools import parse_obj_as
 
 from overhave import db
 from overhave.storage.converters import FeatureModel
 from overhave.utils import get_current_time
 
 logger = logging.getLogger(__name__)
 
@@ -26,14 +25,15 @@
 
     @staticmethod
     @abc.abstractmethod
     def feature_model_by_id(session: so.Session, feature_id: int) -> FeatureModel:
         pass
 
     @staticmethod
+    @abc.abstractmethod
     def get_feature_model(feature_id: int) -> FeatureModel | None:
         pass
 
     @staticmethod
     @abc.abstractmethod
     def create_feature(model: FeatureModel) -> int:
         pass
@@ -48,29 +48,29 @@
     def get_features_by_tag(tag_id: int) -> list[FeatureModel]:
         pass
 
 
 def _append_tags_to_feature(session: so.Session, feature: db.Feature, tag_ids: Iterable[int]) -> None:
     db_tags: list[db.Tags] = []
     for tag_id in tag_ids:
-        db_tag = session.get(db.Tags, tag_id)
+        db_tag: db.Tags | None = session.get(db.Tags, tag_id)
         if db_tag is None:
             raise FeatureTagNotExistsError(f"Feature tag with id={tag_id} does not exist!")
         logger.info("Append tag with id=%s and value=%s", tag_id, db_tag.value)
         db_tags.append(db_tag)
     feature.feature_tags.extend(db_tags)
 
 
 class FeatureStorage(IFeatureStorage):
     """Class for feature storage."""
 
     @staticmethod
     def feature_model_by_id(session: so.Session, feature_id: int) -> FeatureModel:
         feature = session.query(db.Feature).filter(db.Feature.id == feature_id).one()
-        return FeatureModel.from_orm(feature)
+        return FeatureModel.model_validate(feature)
 
     @staticmethod
     def create_feature(model: FeatureModel) -> int:
         with db.create_session() as session:
             feature = db.Feature(
                 name=model.name,
                 author=model.author,
@@ -120,16 +120,16 @@
             feature_ids_query = (
                 session.query(db.FeatureTagsAssociationTable)
                 .with_entities(db.FeatureTagsAssociationTable.feature_id)
                 .filter(db.FeatureTagsAssociationTable.tags_id == tag_id)
                 .scalar_subquery()
             )
             features = session.query(db.Feature).filter(db.Feature.id.in_(feature_ids_query)).all()
-            return parse_obj_as(list[FeatureModel], features)
+            return [FeatureModel.model_validate(x) for x in features]
 
     @staticmethod
     def get_feature_model(feature_id: int) -> FeatureModel | None:
         with db.create_session() as session:
             feature = session.get(db.Feature, feature_id)
             if feature is not None:
-                return FeatureModel.from_orm(feature)
+                return FeatureModel.model_validate(feature)
             return None
```

### Comparing `overhave-4.1.1/overhave/storage/feature_tag_storage.py` & `overhave-5.0.0/overhave/storage/feature_tag_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,22 +29,22 @@
     """Class for feature tags storage."""
 
     @staticmethod
     def get_tag_by_value(value: str) -> TagModel | None:
         with db.create_session() as session:
             tag = session.query(db.Tags).filter(db.Tags.value == value).one_or_none()
             if tag is not None:
-                return TagModel.from_orm(tag)
+                return TagModel.model_validate(tag)
             return None
 
     @staticmethod
     def get_tags_like_value(value: str) -> list[TagModel]:
         with db.create_session() as session:
             db_tags = session.query(db.Tags).filter(db.Tags.value.like(value)).all()
-            return [TagModel.from_orm(tag) for tag in db_tags]
+            return [TagModel.model_validate(tag) for tag in db_tags]
 
     @staticmethod
     def get_or_create_tag(session: so.Session, value: str, created_by: str) -> db.Tags:
         tag = session.query(db.Tags).filter(db.Tags.value == value).one_or_none()
         if tag is None:
             tag = db.Tags(value=value, created_by=created_by)
             session.add(tag)
```

### Comparing `overhave-4.1.1/overhave/storage/feature_type_storage.py` & `overhave-5.0.0/overhave/storage/feature_type_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,8 +57,8 @@
             raise FeatureTypeNotExistsError(f"Could not find feature type with name='{name}'!")
         return feature_type
 
     @cached_property
     def all_feature_types(self) -> list[FeatureTypeModel]:
         with db.create_session() as session:
             db_feature_types = session.query(db.FeatureType).all()
-            return [FeatureTypeModel.from_orm(x) for x in db_feature_types]
+            return [FeatureTypeModel.model_validate(x) for x in db_feature_types]
```

### Comparing `overhave-4.1.1/overhave/storage/scenario_storage.py` & `overhave-5.0.0/overhave/storage/scenario_storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 
 class ScenarioStorage(IScenarioStorage):
     """Class for feature type storage."""
 
     @staticmethod
     def scenario_model_by_id(session: so.Session, scenario_id: int) -> ScenarioModel:
         scenario = session.query(db.Scenario).filter(db.Scenario.id == scenario_id).one()
-        return ScenarioModel.from_orm(scenario)
+        return ScenarioModel.model_validate(scenario)
 
     @staticmethod
     def get_scenario_by_feature_id(feature_id: int) -> ScenarioModel:
         with db.create_session() as session:
             scenario: db.Scenario = session.query(db.Scenario).filter(db.Scenario.feature_id == feature_id).one()
-            return ScenarioModel.from_orm(scenario)
+            return ScenarioModel.model_validate(scenario)
 
     @staticmethod
     def update_scenario(model: ScenarioModel) -> None:
         with db.create_session() as session:
             session.execute(sa.update(db.Scenario).where(db.Scenario.id == model.id).values(text=model.text))
 
     @staticmethod
```

### Comparing `overhave-4.1.1/overhave/storage/system_user_group_storage.py` & `overhave-5.0.0/overhave/storage/system_user_group_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/storage/system_user_storage.py` & `overhave-5.0.0/overhave/storage/system_user_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """Class for system user storage."""
 
     @staticmethod
     def get_user_model(user_id: int) -> SystemUserModel | None:
         with db.create_session() as session:
             db_user = session.get(db.UserRole, user_id)
             if db_user is not None:
-                return SystemUserModel.from_orm(db_user)
+                return SystemUserModel.model_validate(db_user)
             return None
 
     @staticmethod
     def create_user(
         session: so.Session, login: str, password: SecretStr | None = None, role: db.Role = db.Role.user
     ) -> db.UserRole:
         db_password = None
```

### Comparing `overhave-4.1.1/overhave/storage/test_run_storage.py` & `overhave-5.0.0/overhave/storage/test_run_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             if isinstance(report, str):
                 values["report"] = report
 
             session.execute(sa.update(db.TestRun).where(db.TestRun.id == run_id).values(**values))
 
     def testrun_model_by_id(self, session: so.Session, run_id: int) -> TestRunModel:
         run = session.query(db.TestRun).filter(db.TestRun.id == run_id).one()
-        return TestRunModel.from_orm(run)
+        return TestRunModel.model_validate(run)
 
     def get_testrun_model(self, run_id: int) -> TestRunModel | None:
         with db.create_session() as session:
             run = session.get(db.TestRun, run_id)
             if run is None:
                 return None
-            return TestRunModel.from_orm(run)
+            return TestRunModel.model_validate(run)
```

### Comparing `overhave-4.1.1/overhave/storage/test_user_storage.py` & `overhave-5.0.0/overhave/storage/test_user_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,35 +59,35 @@
     """Class for Test User storage."""
 
     @staticmethod
     def get_testuser_model_by_id(user_id: int) -> TestUserModel | None:
         with db.create_session() as session:
             user = session.get(db.TestUser, user_id)
             if user is not None:
-                return TestUserModel.from_orm(user)
+                return TestUserModel.model_validate(user)
             return None
 
     @staticmethod
     def get_testuser_model_by_key(key: str) -> TestUserModel | None:
         with db.create_session() as session:
             user: db.TestUser | None = session.query(db.TestUser).filter(db.TestUser.key == key).one_or_none()
             if user is not None:
-                return TestUserModel.from_orm(user)
+                return TestUserModel.model_validate(user)
             return None
 
     @staticmethod
     def get_test_users_by_feature_type_name(
         session: so.Session, feature_type_id: int, allow_update: bool
     ) -> list[TestUserModel]:
         db_users = (
             session.query(db.TestUser)
             .filter(db.TestUser.feature_type_id == feature_type_id, db.TestUser.allow_update.is_(allow_update))
             .all()
         )
-        return [TestUserModel.from_orm(user) for user in db_users]
+        return [TestUserModel.model_validate(user) for user in db_users]
 
     @staticmethod
     def update_test_user_specification(user_id: int, specification: TestUserSpecification) -> None:
         with db.create_session() as session:
             test_user = session.get(db.TestUser, user_id)
             if test_user is None:
                 raise TestUserDoesNotExistError(f"Test user with id {user_id} does not exist!")
```

### Comparing `overhave-4.1.1/overhave/synchronization/storage_manager.py` & `overhave-5.0.0/overhave/synchronization/storage_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 from datetime import datetime
 
 import sqlalchemy.orm as so
-from pydantic import parse_obj_as
 
 from overhave.scenario import StrictFeatureInfo
 from overhave.storage import (
     FeatureModel,
     FeatureTypeModel,
     FeatureTypeName,
     IDraftStorage,
@@ -66,19 +65,19 @@
 
     def get_feature_tags(self, session: so.Session, info: StrictFeatureInfo) -> list[TagModel]:
         db_tags = [
             self._tag_storage.get_or_create_tag(session=session, value=tag, created_by=info.last_edited_by)
             for tag in info.tags
         ]
         session.flush()
-        return parse_obj_as(list[TagModel], db_tags)
+        return [TagModel.model_validate(x) for x in db_tags]
 
     def feature_type_by_name(self, session: so.Session, feature_type: FeatureTypeName) -> FeatureTypeModel:
         db_feature_type = self._feature_type_storage.feature_type_by_name(session=session, name=feature_type)
-        return FeatureTypeModel.from_orm(db_feature_type)
+        return FeatureTypeModel.model_validate(db_feature_type)
 
     def ensure_users_exist(self, session: so.Session, info: StrictFeatureInfo) -> None:
         for user in {info.author, info.last_edited_by}:
             if self._system_user_storage.get_user_by_credits(session=session, login=user):
                 continue
             raise FeatureInfoUserNotFoundError(f"Could not find user with login={user}!")
```

### Comparing `overhave-4.1.1/overhave/synchronization/synchronizer.py` & `overhave-5.0.0/overhave/synchronization/synchronizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from dataclasses import asdict
 from datetime import datetime
 from pathlib import Path
 from typing import cast
 
 import allure
 import pytz
 
@@ -72,15 +73,15 @@
             raise NullableInfoFeatureTypeError("Could not create feature without feature type!")
         if info.author is None:
             raise NullableInfoAuthorError("Could not create feature without author!")
         if info.last_edited_by is None:
             info.last_edited_by = info.author
 
         info.id = ANY_INT
-        strict_info = StrictFeatureInfo(**info.dict())
+        strict_info = StrictFeatureInfo(**asdict(info))
 
         with db.create_session() as session:
             self._storage_manager.ensure_users_exist(session=session, info=strict_info)
             feature_tags = self._storage_manager.get_feature_tags(session=session, info=strict_info)
             feature_type = self._storage_manager.feature_type_by_name(session=session, feature_type=strict_info.type)
 
         feature_model = FeatureModel(
```

### Comparing `overhave-4.1.1/overhave/test_execution/executor.py` & `overhave-5.0.0/overhave/test_execution/executor.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/test_execution/objects.py` & `overhave-5.0.0/overhave/test_execution/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import re
 from types import FunctionType
 from typing import NewType
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator
 from pytest_bdd.types import STEP_TYPES
 
 StepTypeName = NewType("StepTypeName", str)
 PUBLIC_STEP_ATTR_NAME = "_is_public_step"
 
 
 class BddStepModel(BaseModel):
     """Model for pytest_bdd step in Overhave."""
 
     type: StepTypeName
     name: str
     doc: str
 
-    @validator("type")
+    @field_validator("type")
     def validate_type(cls, v: str) -> StepTypeName:
         if v not in STEP_TYPES:
             raise ValueError
         return StepTypeName(v)
 
     @property
     def html_doc(self) -> str:
```

### Comparing `overhave-4.1.1/overhave/test_execution/settings.py` & `overhave-5.0.0/overhave/test_execution/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import httpx
-from pydantic import validator
+from pydantic import Field, field_validator
 
 from overhave.base_settings import BaseOverhavePrefix
 from overhave.utils import make_url
 
 
 class EmptyOverhaveAdminURLError(ValueError):
     """Exception for situation with empty ````admin_url``` while trying to ```get_feature_url```."""
@@ -13,15 +13,15 @@
     """Settings for dynamic links to Overhave Admin in Allure report."""
 
     admin_url: httpx.URL | None
 
     feature_id_filter_path: str = "feature/?flt2_0={feature_id}"
     feature_id_placeholder: str = "Overhave feature #{feature_id}"
 
-    @validator("admin_url", pre=True)
+    @field_validator("admin_url", mode="before")
     def make_admin_url(cls, v: str | None) -> httpx.URL | None:
         return make_url(v)
 
     @property
     def enabled(self) -> bool:
         return self.admin_url is not None
 
@@ -34,16 +34,16 @@
         return self.feature_id_placeholder.format(feature_id=feature_id)
 
 
 class OverhaveTestSettings(BaseOverhavePrefix):
     """Settings for PytestRunner, which runs scenario tests with specified addoptions."""
 
     default_pytest_addoptions: str = "--disable-warnings"
-    extra_pytest_addoptions: str | None
+    extra_pytest_addoptions: str | None = Field(default=None)
 
-    workers: int | None  # Number of xdist workers, `None` by default
+    workers: int | None = Field(default=None, description="Number of xdist workers")
 
 
 class OverhaveStepCollectorSettings(BaseOverhavePrefix):
     """Settings for StepCollector, which collect BDD steps for Overhave Admin UI."""
 
     hide_non_public_steps: bool = False
```

### Comparing `overhave-4.1.1/overhave/test_execution/step_collector.py` & `overhave-5.0.0/overhave/test_execution/step_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 reverse=True,
             ),
         )
 
     def _compile_full_step_name(self, fixture_name: str, step_type: str) -> str:
         prefix = step_type.title()
         if self._step_prefixes is not None:
-            prefix = self._step_prefixes.dict()[step_type.upper()].strip()
+            prefix = self._step_prefixes.model_dump()[step_type.upper()].strip()
         return f"{prefix} {fixture_name}"
 
     def _compile_step_models(self, steps: tuple[FixtureDef[Any], ...]) -> list[BddStepModel]:
         return [
             BddStepModel(
                 type=f.func._pytest_bdd_step_context.type,  # type: ignore
                 name=self._compile_full_step_name(
```

### Comparing `overhave-4.1.1/overhave/test_execution/test_runner.py` & `overhave-5.0.0/overhave/test_execution/test_runner.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/transport/__init__.py` & `overhave-5.0.0/overhave/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/transport/http/__init__.py` & `overhave-5.0.0/overhave/transport/http/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/transport/http/api_client/authenticator.py` & `overhave-5.0.0/overhave/transport/http/api_client/authenticator.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
     def _auth_by_credentials(self, username: str, password: SecretStr) -> AuthToken:
         logger.info("Get auth_managers token by username and password")
         data = TokenRequestData(username=username, password=password.get_secret_value())
         response = self._make_request(
             method=HttpMethod.POST,
             url=self._settings.get_auth_token_url,
-            data=data.dict(by_alias=True),
+            data=data.model_dump(by_alias=True),
         )
-        return AuthToken.parse_obj(response.json())
+        return AuthToken.model_validate(response.json())
 
     def _get_auth_token(self, username: str, password: SecretStr) -> AuthToken:
         token: AuthToken | None = self._auth_storage.get_auth_token(username=username)
         if token is None:
             token = self._auth_by_credentials(username=username, password=password)
             self._auth_storage.update_auth_token(username=username, new_auth_token=token)
         return token
```

### Comparing `overhave-4.1.1/overhave/transport/http/base_client/auth.py` & `overhave-5.0.0/overhave/transport/http/base_client/auth.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/transport/http/base_client/client.py` & `overhave-5.0.0/overhave/transport/http/base_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from typing import Any, Generic, Mapping, cast
 
 import httpx
 import tenacity
 from pydantic import BaseModel, ValidationError
-from pydantic.main import ModelMetaclass
+from pydantic._internal._model_construction import ModelMetaclass
 
 from overhave.transport.http.base_client.objects import HttpMethod
 from overhave.transport.http.base_client.settings import HttpSettingsType
 
 logger = logging.getLogger(__name__)
 
 
@@ -25,15 +25,15 @@
 
     def __init__(self, settings: HttpSettingsType) -> None:
         self._settings = settings
 
     @staticmethod
     def _parse_or_raise(response: httpx.Response, model: ModelMetaclass) -> BaseModel:
         try:
-            return cast(BaseModel, model).parse_obj(response.json())
+            return cast(BaseModel, model).model_validate(response.json())
         except (ValueError, ValidationError) as e:
             url = getattr(response, "raw_url", response.url)
             raise HttpClientValidationError(f'Response validation error for "{url}"') from e
 
     @tenacity.retry(
         reraise=True,
         retry=tenacity.retry_if_exception_type(httpx.ConnectError),
```

### Comparing `overhave-4.1.1/overhave/transport/http/base_client/settings.py` & `overhave-5.0.0/overhave/transport/http/base_client/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import timedelta
 from typing import TypeVar
 
 import httpx
-from pydantic import BaseSettings, validator
+from pydantic import field_validator
+from pydantic_settings import BaseSettings
 
 from overhave.utils import make_url
 
 
 class BaseHttpClientSettings(BaseSettings):
     """Base settings for :class:`BaseHttpClient`."""
 
@@ -14,15 +15,15 @@
 
     default_timeout: timedelta | None = None
     connect_timeout: timedelta = timedelta(seconds=1)
     read_timeout: timedelta = timedelta(seconds=5)
     write_timeout: timedelta | None = None
     pool_timeout: timedelta | None = None
 
-    @validator("url", pre=True)
+    @field_validator("url", mode="before")
     def make_url(cls, v: str | None) -> httpx.URL | None:
         return make_url(v)
 
     @staticmethod
     def _as_optional_timeout(timeout: timedelta | None) -> float | None:
         if timeout is not None:
             return timeout.total_seconds()
```

### Comparing `overhave-4.1.1/overhave/transport/http/gitlab_client/client.py` & `overhave-5.0.0/overhave/transport/http/gitlab_client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         gitlab_python_client = get_gitlab_python_client(
             url=self._settings.url,
             token_type=self._settings.token_type,
             token=token,
         )
         project = gitlab_python_client.projects.get(repository_id, lazy=True)
         try:
-            result = project.mergerequests.create(merge_request.dict(by_alias=True))
+            result = project.mergerequests.create(merge_request.model_dump(by_alias=True))
             logger.debug("Response from GitLab: %s", result)
             if isinstance(result, ProjectMergeRequest):
                 return GitlabMrCreationResponse(created_at=result.created_at, web_url=result.web_url)
             raise HttpClientValidationError("Unsupported response: %s", result)
         except GitlabAuthenticationError as e:
             logging.exception("Please verify your token or URL! Maybe they are invalid")
             raise GitlabInvalidTokenError("Please verify your token or URL! Maybe they are invalid") from e
```

### Comparing `overhave-4.1.1/overhave/transport/http/gitlab_client/models.py` & `overhave-5.0.0/overhave/transport/http/gitlab_client/models.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/transport/http/gitlab_client/utils.py` & `overhave-5.0.0/overhave/transport/http/gitlab_client/utils.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/transport/http/stash_client/client.py` & `overhave-5.0.0/overhave/transport/http/stash_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         url = self._settings.get_pr_url(
             project_key=pull_request.target_branch.repository.project.key,
             repository_name=pull_request.target_branch.repository.name,
         )
         response = self._make_request(
             method=HttpMethod.POST,
             url=url,
-            json=pull_request.dict(by_alias=True),
+            json=pull_request.model_dump(by_alias=True),
             auth=BearerAuth(self._settings.auth_token),
             raise_for_status=False,
         )
         if response.status_code == HTTPStatus.CONFLICT:
             raise StashHttpClientConflictError("Got conflict when trying to send pull-request!")
         response.raise_for_status()
         for model in STASH_RESPONSE_MODELS:
```

### Comparing `overhave-4.1.1/overhave/transport/http/stash_client/models.py` & `overhave-5.0.0/overhave/transport/http/stash_client/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 from typing import Final
 
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, Field, field_validator
 
 
 class StashProject(BaseModel):
     """Model for Stash pull-request project slug."""
 
     key: str
 
@@ -19,15 +19,15 @@
 
 class StashBranch(BaseModel):
     """Model for Stash pull-request branch."""
 
     branch: str = Field(..., alias="id")
     repository: StashRepository
 
-    @validator("branch")
+    @field_validator("branch")
     def insert_refs(cls, v: str) -> str:
         return "refs/heads/" + v
 
 
 class StashReviewerInfo(BaseModel):
     """Model for Stash pull-request reviewer information."""
 
@@ -39,15 +39,15 @@
 
     user: StashReviewerInfo
 
 
 class StashBasicPrInfo(BaseModel):
     """Model for Stash basic pull-request information."""
 
-    title: str | None
+    title: str | None = Field(default=None)
     open: bool
 
 
 class StashPrRequest(StashBasicPrInfo):
     """Model for Stash pull-request request."""
 
     description: str
@@ -64,17 +64,17 @@
 
 
 class StashPrCreationResponse(StashBasicPrInfo):
     """Model for Stash pull-request creation response."""
 
     created_date: datetime = Field(..., alias="createdDate")
     updated_date: datetime = Field(..., alias="updatedDate")
-    pull_request_url: str | None
-    traceback: Exception | None
-    links: StashLinksType | None
+    pull_request_url: str | None = Field(default=None)
+    traceback: Exception | None = Field(default=None)
+    links: StashLinksType | None = Field(default=None)
 
     class Config:
         arbitrary_types_allowed = True
 
     def get_pr_url(self) -> str:
         if isinstance(self.pull_request_url, str):
             return self.pull_request_url
```

### Comparing `overhave-4.1.1/overhave/transport/http/stash_client/settings.py` & `overhave-5.0.0/overhave/transport/http/stash_client/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/transport/ldap/authenticator.py` & `overhave-5.0.0/overhave/transport/ldap/authenticator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/transport/redis/consumer.py` & `overhave-5.0.0/overhave/transport/redis/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     @property
     def _stream(self) -> walrus.containers.ConsumerGroupStream:
         return getattr(self._consumer_group, self._stream_name.with_dunder)
 
     def _clean_pending(self) -> None:
         pending_messages = self._stream.pending()
-        models: list[RedisPendingData] = [RedisPendingData.parse_obj(msg) for msg in pending_messages]
+        models: list[RedisPendingData] = [RedisPendingData.model_validate(msg) for msg in pending_messages]
         if models:
             message_ids = [x.message_id for x in models]
             self._stream.claim(*message_ids)
             self._stream.ack(*message_ids)
             logger.info("Clean all pending messages for stream %s: %s", self._stream_name, models)
 
     def _consume(self) -> Sequence[RedisUnreadData]:
@@ -70,8 +70,8 @@
                     yield messages
                 continue
             except Exception:
                 logger.exception("Error while trying to consume message from redis!")
             raise StopIteration()
 
     def __exit__(self, exc_type: type[Exception], exc_val: Exception, exc_tb: TracebackType) -> None:
-        pass
+        pass  # no actions on exit required
```

### Comparing `overhave-4.1.1/overhave/transport/redis/deps.py` & `overhave-5.0.0/overhave/transport/redis/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/transport/redis/objects.py` & `overhave-5.0.0/overhave/transport/redis/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     def message(self) -> dict[bytes, bytes]:
         pass
 
 
 class BaseRedisTask(_IRedisTask):
     """Base task for Redis streams."""
 
-    data: Any
+    data: BaseModel
 
     @property
     def message(self) -> dict[bytes, bytes]:
-        return {b"data": self.data.json().encode("utf-8")}
+        return {b"data": self.data.model_dump_json().encode("utf-8")}
 
 
 class TestRunData(BaseModel):
     """Specific data for test run."""
 
     __test__ = False
```

### Comparing `overhave-4.1.1/overhave/transport/redis/producer.py` & `overhave-5.0.0/overhave/transport/redis/producer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/transport/redis/runner.py` & `overhave-5.0.0/overhave/transport/redis/runner.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.1/overhave/transport/redis/settings.py` & `overhave-5.0.0/overhave/transport/redis/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from datetime import timedelta
+
 import yarl
-from pydantic.class_validators import validator
-from pydantic.datetime_parse import timedelta
-from pydantic.env_settings import BaseSettings
+from pydantic import field_validator
+from pydantic_settings import BaseSettings
 
 
 class BaseRedisSettings(BaseSettings):
     """Base settings for Redis entities, which use for work with different framework tasks."""
 
     db: int = 0
     block_timeout: timedelta = timedelta(seconds=1)
@@ -21,30 +22,30 @@
 
 
 class OverhaveRedisSettings(BaseRedisSettings):
     """Settings for Redis entities, which use for work with different framework tasks."""
 
     url: yarl.URL = yarl.URL("redis://localhost:6379")
 
-    @validator("url", pre=True)
+    @field_validator("url", mode="before")
     def validate_url(cls, v: str | yarl.URL) -> yarl.URL:
         if isinstance(v, str):
             return yarl.URL(v)
         return v
 
 
 class OverhaveRedisSentinelSettings(BaseRedisSettings):
     """Settings for Redis sentinel entities, which use for work with different framework tasks."""
 
     enabled: bool = False
     urls: list[yarl.URL] = [yarl.URL("redis://localhost:6379")]
     master_set: str = "foo"
     password: str = "bar"
 
-    @validator("urls", pre=True)
+    @field_validator("urls", mode="before")
     def validate_urls(cls, v: list[str] | list[yarl.URL]) -> list[yarl.URL]:
         urls = []
         for url in v:
             if isinstance(url, str):
                 urls.append(yarl.URL(url))
             if isinstance(url, yarl.URL):
                 urls.append(url)
```

### Comparing `overhave-4.1.1/overhave/transport/s3/manager.py` & `overhave-5.0.0/overhave/transport/s3/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,22 @@
 from typing import Any, Callable
 
 import boto3
 import botocore.exceptions
 import httpx
 import urllib3
 from boto3_type_annotations.s3 import Client
-from pydantic.tools import parse_obj_as
 
-from overhave.transport.s3.models import BucketModel, DeletionResultModel, ObjectModel
+from overhave.transport.s3.models import (
+    LIST_BUCKET_MODEL_ADAPTER,
+    LIST_OBJECT_MODEL_ADAPTER,
+    BucketModel,
+    DeletionResultModel,
+    ObjectModel,
+)
 from overhave.transport.s3.objects import OverhaveS3Bucket
 from overhave.transport.s3.settings import OverhaveS3ManagerSettings
 from overhave.utils import make_url
 
 logger = logging.getLogger(__name__)
 
 
@@ -114,15 +119,15 @@
         for bucket in list(filter(lambda x: x.value not in bucket_names, list(OverhaveS3Bucket))):
             self.create_bucket(bucket.value)
         logger.info("Successfully ensured existence of Overhave service buckets.")
 
     @_s3_error(msg="Error while getting buckets list!")
     def _get_buckets(self) -> list[BucketModel]:
         response = self._ensured_client.list_buckets()
-        return parse_obj_as(list[BucketModel], response.get("Buckets"))
+        return LIST_BUCKET_MODEL_ADAPTER.validate_python(response.get("Buckets"))
 
     @_s3_error(msg="Error while creating bucket!")
     def create_bucket(self, bucket: str) -> None:
         logger.info("Creating bucket %s...", bucket)
         kwargs: dict[str, Any] = {"Bucket": bucket}
         if isinstance(self._settings.region_name, str):
             kwargs["CreateBucketConfiguration"] = {"LocationConstraint": self._settings.region_name}
@@ -139,27 +144,27 @@
             logger.exception("Could not upload file to s3 cloud!")
             return False
 
     @_s3_error(msg="Error while getting bucket objects list!")
     def get_bucket_objects(self, bucket: str) -> list[ObjectModel]:
         response = self._ensured_client.list_objects(Bucket=bucket)
         logger.debug("List objects response:\n%s", response)
-        return parse_obj_as(list[ObjectModel], response.get("Contents"))
+        return LIST_OBJECT_MODEL_ADAPTER.validate_python(response.get("Contents"))
 
     @_s3_error(msg="Error while deleting bucket objects!")
     def delete_bucket_objects(self, bucket: str, objects: list[ObjectModel]) -> DeletionResultModel:
         if not objects:
             raise EmptyObjectsListError("No one object specified for deletion!")
         logger.info("Deleting items %s...", [obj.name for obj in objects])
         response = self._ensured_client.delete_objects(
             Bucket=bucket,
             Delete={"Objects": [{"Key": obj.name} for obj in objects]},
         )
         logger.debug("Delete objects response:\n%s", response)
-        return DeletionResultModel.parse_obj(response)
+        return DeletionResultModel.model_validate(response)
 
     def _ensure_bucket_clean(self, bucket: str) -> None:
         objects = self.get_bucket_objects(bucket)
         if not objects:
             logger.info("Has not got any objects in bucket '%s'.", bucket)
             return
         deletion_result = self.delete_bucket_objects(bucket=bucket, objects=objects)
```

### Comparing `overhave-4.1.1/overhave/transport/s3/models.py` & `overhave-5.0.0/overhave/transport/s3/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from datetime import datetime
 from typing import Any
 
-from pydantic import Extra, Field, root_validator
-from pydantic.main import BaseModel
+from pydantic import BaseModel, Field, TypeAdapter, model_validator
 
 
 class BucketModel(BaseModel):
     """Model for boto3 client Bucket."""
 
     name: str = Field(alias="Name")
     created_at: datetime = Field(alias="CreationDate")
 
 
+LIST_BUCKET_MODEL_ADAPTER: TypeAdapter[list[BucketModel]] = TypeAdapter(list[BucketModel])
+
+
 class OwnerModel(BaseModel):
     """Model for boto3 client object owner."""
 
     name: str = Field(alias="DisplayName")
     owner_id: str = Field(alias="ID")
 
 
@@ -26,45 +28,48 @@
     modified_at: datetime = Field(alias="LastModified")
     etag: str = Field(alias="ETag")
     size: int = Field(alias="Size")
     storage_class: str = Field(alias="StorageClass")
     owner: OwnerModel = Field(alias="Owner")
 
     class Config:
-        extra = Extra.allow
+        extra = "allow"
+
+
+LIST_OBJECT_MODEL_ADAPTER: TypeAdapter[list[ObjectModel]] = TypeAdapter(list[ObjectModel])
 
 
 class BaseObjectToDeletionModel(BaseModel):
     """Base model for boto3 client object deletion result."""
 
     name: str = Field(alias="Key")
-    etag: str | None = Field(alias="VersionId")
+    etag: str | None = Field(default=None, alias="VersionId")
 
 
 class DeletedObjectModel(BaseObjectToDeletionModel):
     """Model for boto3 client deleted object."""
 
-    marker: bool | None = Field(alias="DeleteMarker")
-    marker_id: bool | None = Field(alias="DeleteMarkerVersionId")
+    marker: bool | None = Field(default=None, alias="DeleteMarker")
+    marker_id: bool | None = Field(default=None, alias="DeleteMarkerVersionId")
 
 
 class NotDeletedObjectModel(BaseObjectToDeletionModel):
     """Model for boto3 client not deleted object."""
 
     code: str = Field(alias="Code")
     message: str = Field(alias="Message")
 
 
 class DeletionResultModel(BaseModel):
     """Model for boto3 client objects deletion result."""
 
-    deleted: list[DeletedObjectModel] | None = Field(alias="Deleted")
-    errors: list[NotDeletedObjectModel] | None = Field(alias="Errors")
-    requester: str | None = Field(alias="RequestCharged")
+    deleted: list[DeletedObjectModel] | None = Field(default=None, alias="Deleted")
+    errors: list[NotDeletedObjectModel] | None = Field(default=None, alias="Errors")
+    requester: str | None = Field(default=None, alias="RequestCharged")
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     def validate_results(cls, values: dict[str, Any]) -> dict[str, Any]:
         deleted = values.get("Deleted")
         errors = values.get("Errors")
         if deleted is None and errors is None:
             raise ValueError("At least one result field should be presented!")
         return values
```

### Comparing `overhave-4.1.1/overhave/transport/s3/settings.py` & `overhave-5.0.0/overhave/transport/s3/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from typing import Any
 
-from pydantic import BaseSettings, root_validator
+from pydantic import Field, model_validator
+from pydantic_settings import BaseSettings
 
 
 class OverhaveS3ManagerSettings(BaseSettings):
     """Settings for S3Client."""
 
     enabled: bool = False
 
-    url: str | None
-    region_name: str | None
-    access_key: str | None
-    secret_key: str | None
+    url: str | None = Field(default=None)
+    region_name: str | None = Field(default=None)
+    access_key: str | None = Field(default=None)
+    secret_key: str | None = Field(default=None)
     verify: bool = True
 
     autocreate_buckets: bool = False
 
     class Config:
         env_prefix = "OVERHAVE_S3_"
 
-    @root_validator
+    @model_validator(mode="before")
     def validate_enabling(cls, values: dict[str, Any]) -> dict[str, Any]:
         enabled = values.get("enabled")
         if enabled and not all(
             (
                 isinstance(values.get("url"), str),
                 isinstance(values.get("access_key"), str),
                 isinstance(values.get("secret_key"), str),
```

### Comparing `overhave-4.1.1/pyproject.toml` & `overhave-5.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "overhave"
-version = "4.1.1"
+version = "5.0.0"
 description = "Overhave - web-framework for BDD"
 readme = "README.rst"
 authors = [
     "Vladislav Mukhamatnurov <livestreamepidemz@yandex.ru>",
     "Tinkoff Backend Dialog System Team <bds-dev@tinkoff.ru>"
 ]
 classifiers = [
@@ -59,14 +59,15 @@
 flask-login = "^0.6.2"
 flask-wtf = "^1.1.1"
 flask = "^2.3.2"
 sqlalchemy = ">=1.4"
 sqlalchemy-utils = "^0.41.1"
 sqlalchemy-utc = "^0.14.0"
 prometheus-client = "^0.16.0"
+pydantic-settings = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 flake8-awesome = "<1.3"
 requests_mock = "*"
 flake8-docstrings = "^1.5"
 pytest-faker = "^2.0"
 filelock = "*"
```

### Comparing `overhave-4.1.1/PKG-INFO` & `overhave-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overhave
-Version: 4.1.1
+Version: 5.0.0
 Summary: Overhave - web-framework for BDD
 Author: Vladislav Mukhamatnurov
 Author-email: livestreamepidemz@yandex.ru
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
@@ -33,14 +33,15 @@
 Requires-Dist: flask-wtf (>=1.1.1,<2.0.0)
 Requires-Dist: httptools (>=0.5.0,<0.6.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: ldap3 (>=2.6,<3.0)
 Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
 Requires-Dist: psycopg2-binary (>=2.8,<3.0)
 Requires-Dist: pydantic (>=1.7)
+Requires-Dist: pydantic-settings (>=2.0.1,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
 Requires-Dist: python-gitlab (>=2.9.0,<3.0.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: python-ldap (>=3.2,<4.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: pytz
 Requires-Dist: redis (>=4.2.0,<5.0.0)
```

