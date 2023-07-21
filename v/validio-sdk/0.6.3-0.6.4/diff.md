# Comparing `tmp/validio_sdk-0.6.3.tar.gz` & `tmp/validio_sdk-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_sdk-0.6.3.tar", max compression
+gzip compressed data, was "validio_sdk-0.6.4.tar", max compression
```

## Comparing `validio_sdk-0.6.3.tar` & `validio_sdk-0.6.4.tar`

### file list

```diff
@@ -1,227 +1,229 @@
--rw-r--r--   0        0        0    11340 2023-07-10 07:22:33.392637 validio_sdk-0.6.3/LICENSE
--rw-r--r--   0        0        0      308 2023-07-10 07:22:33.393637 validio_sdk-0.6.3/README_PUBLIC.md
--rw-r--r--   0        0        0     5010 2023-07-10 07:22:49.313606 validio_sdk-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      588 2023-07-10 07:22:33.398637 validio_sdk-0.6.3/validio_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 07:22:33.398637 validio_sdk-0.6.3/validio_sdk/code/__init__.py
--rw-r--r--   0        0        0      551 2023-07-10 07:22:33.398637 validio_sdk-0.6.3/validio_sdk/code/apply.py
--rw-r--r--   0        0        0     4751 2023-07-10 07:22:33.398637 validio_sdk-0.6.3/validio_sdk/code/plan.py
--rw-r--r--   0        0        0     1565 2023-07-10 07:22:33.398637 validio_sdk-0.6.3/validio_sdk/code/scaffold.py
--rw-r--r--   0        0        0      305 2023-07-10 07:22:33.398637 validio_sdk-0.6.3/validio_sdk/code/settings.py
--rw-r--r--   0        0        0     5891 2023-07-10 07:22:33.398637 validio_sdk-0.6.3/validio_sdk/config.py
--rw-r--r--   0        0        0   261520 2023-07-10 07:22:33.399637 validio_sdk-0.6.3/validio_sdk/graphql_client/__init__.py
--rw-r--r--   0        0        0      573 2023-07-10 07:22:33.399637 validio_sdk-0.6.3/validio_sdk/graphql_client/apply_validator_recommendation.py
--rw-r--r--   0        0        0     7319 2023-07-10 07:22:33.399637 validio_sdk-0.6.3/validio_sdk/graphql_client/async_base_client.py
--rw-r--r--   0        0        0      526 2023-07-10 07:22:33.399637 validio_sdk-0.6.3/validio_sdk/graphql_client/aws_credential_secret_changed.py
--rw-r--r--   0        0        0      613 2023-07-10 07:22:33.399637 validio_sdk-0.6.3/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py
--rw-r--r--   0        0        0      614 2023-07-10 07:22:33.399637 validio_sdk-0.6.3/validio_sdk/graphql_client/backfill_source.py
--rw-r--r--   0        0        0     1899 2023-07-10 07:22:33.399637 validio_sdk-0.6.3/validio_sdk/graphql_client/base_model.py
--rw-r--r--   0        0        0   652845 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/client.py
--rw-r--r--   0        0        0      506 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_aws_athena_credential.py
--rw-r--r--   0        0        0      458 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_aws_athena_source.py
--rw-r--r--   0        0        0      445 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_aws_credential.py
--rw-r--r--   0        0        0      528 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_aws_kinesis_destination.py
--rw-r--r--   0        0        0      468 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_aws_kinesis_source.py
--rw-r--r--   0        0        0      526 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_aws_redshift_credential.py
--rw-r--r--   0        0        0      480 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_aws_redshift_source.py
--rw-r--r--   0        0        0      418 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_aws_s3_source.py
--rw-r--r--   0        0        0      843 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      823 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      455 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_demo_credential.py
--rw-r--r--   0        0        0      407 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_demo_source.py
--rw-r--r--   0        0        0      407 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_file_window.py
--rw-r--r--   0        0        0      468 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_fixed_batch_window.py
--rw-r--r--   0        0        0      702 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      682 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      539 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_gcp_big_query_destination.py
--rw-r--r--   0        0        0      481 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_gcp_big_query_source.py
--rw-r--r--   0        0        0      445 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_gcp_credential.py
--rw-r--r--   0        0        0      500 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_gcp_pub_sub_lite_source.py
--rw-r--r--   0        0        0      459 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_gcp_pub_sub_source.py
--rw-r--r--   0        0        0      468 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_gcp_storage_source.py
--rw-r--r--   0        0        0      557 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_kafka_sasl_plain_credential.py
--rw-r--r--   0        0        0      417 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_kafka_source.py
--rw-r--r--   0        0        0      498 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_kafka_ssl_credential.py
--rw-r--r--   0        0        0      487 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_notification_rule.py
--rw-r--r--   0        0        0      753 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      733 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      803 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      783 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      823 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      682 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      662 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      702 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      516 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_postgre_sql_credential.py
--rw-r--r--   0        0        0      468 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_postgre_sql_source.py
--rw-r--r--   0        0        0      733 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      713 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      753 2023-07-10 07:22:33.401637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      753 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      733 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      528 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_saml_identity_provider.py
--rw-r--r--   0        0        0      438 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_segmentation.py
--rw-r--r--   0        0        0      477 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_sessionized_window.py
--rw-r--r--   0        0        0      429 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_slack_channel.py
--rw-r--r--   0        0        0      505 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_snowflake_credential.py
--rw-r--r--   0        0        0      517 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_snowflake_destination.py
--rw-r--r--   0        0        0      457 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_snowflake_source.py
--rw-r--r--   0        0        0      447 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_tumbling_window.py
--rw-r--r--   0        0        0      328 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_user.py
--rw-r--r--   0        0        0      672 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      652 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      449 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/create_webhook_channel.py
--rw-r--r--   0        0        0      364 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_channel.py
--rw-r--r--   0        0        0      614 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_credential.py
--rw-r--r--   0        0        0      622 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_credentials.py
--rw-r--r--   0        0        0      630 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_destination.py
--rw-r--r--   0        0        0      638 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_destinations.py
--rw-r--r--   0        0        0      376 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_identity.py
--rw-r--r--   0        0        0      487 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_identity_provider.py
--rw-r--r--   0        0        0      487 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_notification_rule.py
--rw-r--r--   0        0        0      646 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_segmentation.py
--rw-r--r--   0        0        0      536 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_source.py
--rw-r--r--   0        0        0      544 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_sources.py
--rw-r--r--   0        0        0      328 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_user.py
--rw-r--r--   0        0        0      606 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_validators.py
--rw-r--r--   0        0        0      536 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_window.py
--rw-r--r--   0        0        0      544 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/delete_windows.py
--rw-r--r--   0        0        0      589 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/dismiss_validator_recommendation.py
--rw-r--r--   0        0        0     3198 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/enums.py
--rw-r--r--   0        0        0     2314 2023-07-10 07:22:33.402637 validio_sdk-0.6.3/validio_sdk/graphql_client/exceptions.py
--rw-r--r--   0        0        0   188520 2023-07-10 07:22:33.403637 validio_sdk-0.6.3/validio_sdk/graphql_client/fragments.py
--rw-r--r--   0        0        0      526 2023-07-10 07:22:33.403637 validio_sdk-0.6.3/validio_sdk/graphql_client/gcp_credential_secret_changed.py
--rw-r--r--   0        0        0     2896 2023-07-10 07:22:33.403637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_channel_by_resource_name.py
--rw-r--r--   0        0        0     2427 2023-07-10 07:22:33.403637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_channels.py
--rw-r--r--   0        0        0     8034 2023-07-10 07:22:33.403637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_credential_by_resource_name.py
--rw-r--r--   0        0        0     5997 2023-07-10 07:22:33.403637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_destination_by_resource_name.py
--rw-r--r--   0        0        0     2218 2023-07-10 07:22:33.403637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py
--rw-r--r--   0        0        0     2033 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_identity_providers.py
--rw-r--r--   0        0        0     5368 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_incidents.py
--rw-r--r--   0        0        0      627 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py
--rw-r--r--   0        0        0      480 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_notification_rules.py
--rw-r--r--   0        0        0     2245 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_recommendation.py
--rw-r--r--   0        0        0      460 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_segment_incidents.py
--rw-r--r--   0        0        0      357 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_segmentation.py
--rw-r--r--   0        0        0      572 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_segmentation_by_resource_name.py
--rw-r--r--   0        0        0    24018 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_source.py
--rw-r--r--   0        0        0    29481 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_source_by_resource_name.py
--rw-r--r--   0        0        0     1727 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_source_incidents.py
--rw-r--r--   0        0        0    25201 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_source_recommended_validators.py
--rw-r--r--   0        0        0      476 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_user_by_resource_name.py
--rw-r--r--   0        0        0      300 2023-07-10 07:22:33.404637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_users.py
--rw-r--r--   0        0        0    40168 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_validator.py
--rw-r--r--   0        0        0    48254 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_validator_by_resource_name.py
--rw-r--r--   0        0        0      480 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_validator_incidents.py
--rw-r--r--   0        0        0      551 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_validator_segment_incidents.py
--rw-r--r--   0        0        0     3986 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_validator_segment_metrics.py
--rw-r--r--   0        0        0     5711 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/get_window_by_resource_name.py
--rw-r--r--   0        0        0      286 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/infer_aws_athena_schema.py
--rw-r--r--   0        0        0      290 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/infer_aws_kinesis_schema.py
--rw-r--r--   0        0        0      308 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/infer_aws_redshift_schema.py
--rw-r--r--   0        0        0      270 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/infer_aws_s3_schema.py
--rw-r--r--   0        0        0      265 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/infer_demo_schema.py
--rw-r--r--   0        0        0      309 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/infer_gcp_big_query_schema.py
--rw-r--r--   0        0        0      318 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/infer_gcp_pub_sub_lite_schema.py
--rw-r--r--   0        0        0      287 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/infer_gcp_pub_sub_schema.py
--rw-r--r--   0        0        0      290 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/infer_gcp_storage_schema.py
--rw-r--r--   0        0        0      269 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/infer_kafka_schema.py
--rw-r--r--   0        0        0      290 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/infer_postgre_sql_schema.py
--rw-r--r--   0        0        0      285 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/infer_snowflake_schema.py
--rw-r--r--   0        0        0    39680 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/input_types.py
--rw-r--r--   0        0        0      644 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/kafka_sasl_plain_credential_secret_changed.py
--rw-r--r--   0        0        0      583 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/kafka_ssl_credential_secret_changed.py
--rw-r--r--   0        0        0     6977 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/list_credentials.py
--rw-r--r--   0        0        0     5202 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/list_destinations.py
--rw-r--r--   0        0        0      457 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/list_segmentations.py
--rw-r--r--   0        0        0    25334 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/list_sources.py
--rw-r--r--   0        0        0    42237 2023-07-10 07:22:33.405637 validio_sdk-0.6.3/validio_sdk/graphql_client/list_validators.py
--rw-r--r--   0        0        0     4976 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/list_windows.py
--rw-r--r--   0        0        0      603 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py
--rw-r--r--   0        0        0      594 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/scalars.py
--rw-r--r--   0        0        0      288 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/segments.py
--rw-r--r--   0        0        0      499 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/segments_by_resource_name.py
--rw-r--r--   0        0        0      592 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/snowflake_credential_secret_changed.py
--rw-r--r--   0        0        0      566 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/start_source.py
--rw-r--r--   0        0        0      550 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/stop_source.py
--rw-r--r--   0        0        0      502 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_aws_athena_credential.py
--rw-r--r--   0        0        0      454 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_aws_athena_source.py
--rw-r--r--   0        0        0      441 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_aws_credential.py
--rw-r--r--   0        0        0      524 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_aws_kinesis_destination.py
--rw-r--r--   0        0        0      464 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_aws_kinesis_source.py
--rw-r--r--   0        0        0      522 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_aws_redshift_credential.py
--rw-r--r--   0        0        0      476 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_aws_redshift_source.py
--rw-r--r--   0        0        0      414 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_aws_s3_source.py
--rw-r--r--   0        0        0      636 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_categorical_distribution_validator.py
--rw-r--r--   0        0        0      469 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_channel_namespace.py
--rw-r--r--   0        0        0      499 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_credential_namespace.py
--rw-r--r--   0        0        0      509 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_destination_namespace.py
--rw-r--r--   0        0        0      464 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_fixed_batch_window.py
--rw-r--r--   0        0        0      491 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_freshness_validator.py
--rw-r--r--   0        0        0      535 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_gcp_big_query_destination.py
--rw-r--r--   0        0        0      477 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_gcp_big_query_source.py
--rw-r--r--   0        0        0      441 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_gcp_credential.py
--rw-r--r--   0        0        0      496 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_gcp_pub_sub_lite_source.py
--rw-r--r--   0        0        0      455 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_gcp_pub_sub_source.py
--rw-r--r--   0        0        0      464 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_gcp_storage_source.py
--rw-r--r--   0        0        0      560 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_identity_provider_namespace.py
--rw-r--r--   0        0        0      553 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_kafka_sasl_plain_credential.py
--rw-r--r--   0        0        0      413 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_kafka_source.py
--rw-r--r--   0        0        0      494 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_kafka_ssl_credential.py
--rw-r--r--   0        0        0      534 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_local_identity_provider.py
--rw-r--r--   0        0        0      483 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_notification_rule.py
--rw-r--r--   0        0        0      560 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_notification_rule_namespace.py
--rw-r--r--   0        0        0      540 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_numeric_anomaly_validator.py
--rw-r--r--   0        0        0      596 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_numeric_distribution_validator.py
--rw-r--r--   0        0        0      469 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_numeric_validator.py
--rw-r--r--   0        0        0      512 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_postgre_sql_credential.py
--rw-r--r--   0        0        0      464 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_postgre_sql_source.py
--rw-r--r--   0        0        0      520 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_relative_time_validator.py
--rw-r--r--   0        0        0      540 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_relative_volume_validator.py
--rw-r--r--   0        0        0      524 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_saml_identity_provider.py
--rw-r--r--   0        0        0      519 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_segmentation_namespace.py
--rw-r--r--   0        0        0      473 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_sessionized_window.py
--rw-r--r--   0        0        0      425 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_slack_channel.py
--rw-r--r--   0        0        0      501 2023-07-10 07:22:33.406637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_snowflake_credential.py
--rw-r--r--   0        0        0      513 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_snowflake_destination.py
--rw-r--r--   0        0        0      453 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_snowflake_source.py
--rw-r--r--   0        0        0      459 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_source_namespace.py
--rw-r--r--   0        0        0      443 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_tumbling_window.py
--rw-r--r--   0        0        0      324 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_user.py
--rw-r--r--   0        0        0      439 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_user_namespace.py
--rw-r--r--   0        0        0      491 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_validator_namespace.py
--rw-r--r--   0        0        0    57176 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0    56052 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0    58306 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      459 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_volume_validator.py
--rw-r--r--   0        0        0      445 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_webhook_channel.py
--rw-r--r--   0        0        0      459 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/graphql_client/update_window_namespace.py
--rw-r--r--   0        0        0      265 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/metadata.py
--rw-r--r--   0        0        0        0 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/py.typed
--rw-r--r--   0        0        0      135 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/resource/__init__.py
--rw-r--r--   0        0        0    21078 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/resource/_diff.py
--rw-r--r--   0        0        0     1505 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/resource/_diff_util.py
--rw-r--r--   0        0        0     1657 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/resource/_diffable.py
--rw-r--r--   0        0        0     1579 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/resource/_errors.py
--rw-r--r--   0        0        0     4002 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/resource/_field_selector.py
--rw-r--r--   0        0        0    17790 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/resource/_resource.py
--rw-r--r--   0        0        0     1355 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/resource/_resource_graph.py
--rw-r--r--   0        0        0     5366 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/resource/_serde.py
--rw-r--r--   0        0        0    21679 2023-07-10 07:22:33.407637 validio_sdk-0.6.3/validio_sdk/resource/_server_resources.py
--rw-r--r--   0        0        0      847 2023-07-10 07:22:33.408637 validio_sdk-0.6.3/validio_sdk/resource/_util.py
--rw-r--r--   0        0        0     5027 2023-07-10 07:22:33.408637 validio_sdk-0.6.3/validio_sdk/resource/channels.py
--rw-r--r--   0        0        0     7692 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/resource/credentials.py
--rw-r--r--   0        0        0     5601 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/resource/destinations.py
--rw-r--r--   0        0        0     6262 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/resource/filters.py
--rw-r--r--   0        0        0     4846 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/resource/notification_rules.py
--rw-r--r--   0        0        0     2040 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/resource/segmentations.py
--rw-r--r--   0        0        0    25888 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/resource/sources.py
--rw-r--r--   0        0        0        0 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/resource/tests/__init__.py
--rw-r--r--   0        0        0    15408 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/resource/tests/test__diff.py
--rw-r--r--   0        0        0     1905 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/resource/tests/test__field_selector.py
--rw-r--r--   0        0        0    16357 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/resource/tests/test__resource.py
--rw-r--r--   0        0        0     5638 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/resource/thresholds.py
--rw-r--r--   0        0        0    32563 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/resource/validators.py
--rw-r--r--   0        0        0     5995 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/resource/windows.py
--rw-r--r--   0        0        0     1377 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/scalars.py
--rw-r--r--   0        0        0     1813 2023-07-10 07:22:33.409637 validio_sdk-0.6.3/validio_sdk/util.py
--rw-r--r--   0        0        0     2382 2023-07-10 07:22:33.410637 validio_sdk-0.6.3/validio_sdk/validio_client.py
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 validio_sdk-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-07-21 13:06:25.395451 validio_sdk-0.6.4/LICENSE
+-rw-r--r--   0        0        0      308 2023-07-21 13:06:25.395451 validio_sdk-0.6.4/README_PUBLIC.md
+-rw-r--r--   0        0        0     5010 2023-07-21 13:06:37.623433 validio_sdk-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      588 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/code/__init__.py
+-rw-r--r--   0        0        0     7069 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/code/_import.py
+-rw-r--r--   0        0        0      551 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/code/apply.py
+-rw-r--r--   0        0        0     4751 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/code/plan.py
+-rw-r--r--   0        0        0     1565 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/code/scaffold.py
+-rw-r--r--   0        0        0      305 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/code/settings.py
+-rw-r--r--   0        0        0     5891 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/config.py
+-rw-r--r--   0        0        0   261652 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/__init__.py
+-rw-r--r--   0        0        0      573 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/apply_validator_recommendation.py
+-rw-r--r--   0        0        0     7319 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0      526 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/aws_credential_secret_changed.py
+-rw-r--r--   0        0        0      613 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py
+-rw-r--r--   0        0        0      614 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/backfill_source.py
+-rw-r--r--   0        0        0     1899 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/base_model.py
+-rw-r--r--   0        0        0   653049 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/client.py
+-rw-r--r--   0        0        0      506 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_athena_credential.py
+-rw-r--r--   0        0        0      458 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_athena_source.py
+-rw-r--r--   0        0        0      445 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_credential.py
+-rw-r--r--   0        0        0      528 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      468 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_kinesis_source.py
+-rw-r--r--   0        0        0      526 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_redshift_credential.py
+-rw-r--r--   0        0        0      480 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_redshift_source.py
+-rw-r--r--   0        0        0      418 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_s3_source.py
+-rw-r--r--   0        0        0      843 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      823 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      455 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_demo_credential.py
+-rw-r--r--   0        0        0      407 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_demo_source.py
+-rw-r--r--   0        0        0      407 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_file_window.py
+-rw-r--r--   0        0        0      468 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_fixed_batch_window.py
+-rw-r--r--   0        0        0      702 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      682 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      539 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      481 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_big_query_source.py
+-rw-r--r--   0        0        0      445 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_credential.py
+-rw-r--r--   0        0        0      500 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      459 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      468 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_storage_source.py
+-rw-r--r--   0        0        0      594 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_kafka_sasl_ssl_plain_credential.py
+-rw-r--r--   0        0        0      417 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_kafka_source.py
+-rw-r--r--   0        0        0      498 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_kafka_ssl_credential.py
+-rw-r--r--   0        0        0      487 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_notification_rule.py
+-rw-r--r--   0        0        0      753 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      803 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      783 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      823 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      682 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      662 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      702 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      516 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_postgre_sql_credential.py
+-rw-r--r--   0        0        0      468 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_postgre_sql_source.py
+-rw-r--r--   0        0        0      733 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      713 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      753 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      753 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      528 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_saml_identity_provider.py
+-rw-r--r--   0        0        0      438 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_segmentation.py
+-rw-r--r--   0        0        0      477 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_sessionized_window.py
+-rw-r--r--   0        0        0      429 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_slack_channel.py
+-rw-r--r--   0        0        0      505 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_snowflake_credential.py
+-rw-r--r--   0        0        0      517 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_snowflake_destination.py
+-rw-r--r--   0        0        0      457 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_snowflake_source.py
+-rw-r--r--   0        0        0      447 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_tumbling_window.py
+-rw-r--r--   0        0        0      328 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_user.py
+-rw-r--r--   0        0        0      672 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      652 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      449 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_webhook_channel.py
+-rw-r--r--   0        0        0      364 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_channel.py
+-rw-r--r--   0        0        0      614 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_credential.py
+-rw-r--r--   0        0        0      622 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_credentials.py
+-rw-r--r--   0        0        0      630 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_destination.py
+-rw-r--r--   0        0        0      638 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_destinations.py
+-rw-r--r--   0        0        0      376 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_identity.py
+-rw-r--r--   0        0        0      487 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_identity_provider.py
+-rw-r--r--   0        0        0      487 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_notification_rule.py
+-rw-r--r--   0        0        0      646 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_segmentation.py
+-rw-r--r--   0        0        0      536 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_source.py
+-rw-r--r--   0        0        0      544 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_sources.py
+-rw-r--r--   0        0        0      328 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_user.py
+-rw-r--r--   0        0        0      606 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_validators.py
+-rw-r--r--   0        0        0      536 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_window.py
+-rw-r--r--   0        0        0      544 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_windows.py
+-rw-r--r--   0        0        0      589 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/dismiss_validator_recommendation.py
+-rw-r--r--   0        0        0     3198 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/enums.py
+-rw-r--r--   0        0        0     2314 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/exceptions.py
+-rw-r--r--   0        0        0   188562 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/fragments.py
+-rw-r--r--   0        0        0      526 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/gcp_credential_secret_changed.py
+-rw-r--r--   0        0        0     2896 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_channel_by_resource_name.py
+-rw-r--r--   0        0        0     2427 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_channels.py
+-rw-r--r--   0        0        0     8055 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_credential_by_resource_name.py
+-rw-r--r--   0        0        0     5997 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_destination_by_resource_name.py
+-rw-r--r--   0        0        0     2218 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py
+-rw-r--r--   0        0        0     2033 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_identity_providers.py
+-rw-r--r--   0        0        0     5368 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_incidents.py
+-rw-r--r--   0        0        0      627 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py
+-rw-r--r--   0        0        0      480 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_notification_rules.py
+-rw-r--r--   0        0        0     2245 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_recommendation.py
+-rw-r--r--   0        0        0      460 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_segment_incidents.py
+-rw-r--r--   0        0        0      357 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_segmentation.py
+-rw-r--r--   0        0        0      572 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_segmentation_by_resource_name.py
+-rw-r--r--   0        0        0    24018 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_source.py
+-rw-r--r--   0        0        0    29481 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_source_by_resource_name.py
+-rw-r--r--   0        0        0     1727 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_source_incidents.py
+-rw-r--r--   0        0        0    25201 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_source_recommended_validators.py
+-rw-r--r--   0        0        0      476 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_user_by_resource_name.py
+-rw-r--r--   0        0        0      300 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_users.py
+-rw-r--r--   0        0        0    40168 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator.py
+-rw-r--r--   0        0        0    48254 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator_by_resource_name.py
+-rw-r--r--   0        0        0      480 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator_incidents.py
+-rw-r--r--   0        0        0      551 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator_segment_incidents.py
+-rw-r--r--   0        0        0     3986 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator_segment_metrics.py
+-rw-r--r--   0        0        0     5711 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_window_by_resource_name.py
+-rw-r--r--   0        0        0      286 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_aws_athena_schema.py
+-rw-r--r--   0        0        0      290 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_aws_kinesis_schema.py
+-rw-r--r--   0        0        0      308 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_aws_redshift_schema.py
+-rw-r--r--   0        0        0      270 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_aws_s3_schema.py
+-rw-r--r--   0        0        0      265 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_demo_schema.py
+-rw-r--r--   0        0        0      309 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_gcp_big_query_schema.py
+-rw-r--r--   0        0        0      318 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_gcp_pub_sub_lite_schema.py
+-rw-r--r--   0        0        0      287 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_gcp_pub_sub_schema.py
+-rw-r--r--   0        0        0      290 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_gcp_storage_schema.py
+-rw-r--r--   0        0        0      269 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_kafka_schema.py
+-rw-r--r--   0        0        0      290 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_postgre_sql_schema.py
+-rw-r--r--   0        0        0      285 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_snowflake_schema.py
+-rw-r--r--   0        0        0    39698 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/input_types.py
+-rw-r--r--   0        0        0      675 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/kafka_sasl_ssl_plain_credential_secret_changed.py
+-rw-r--r--   0        0        0      583 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/kafka_ssl_credential_secret_changed.py
+-rw-r--r--   0        0        0     6998 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/list_credentials.py
+-rw-r--r--   0        0        0     5202 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/list_destinations.py
+-rw-r--r--   0        0        0      457 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/list_segmentations.py
+-rw-r--r--   0        0        0    25334 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/list_sources.py
+-rw-r--r--   0        0        0    42237 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/list_validators.py
+-rw-r--r--   0        0        0     4976 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/list_windows.py
+-rw-r--r--   0        0        0      603 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py
+-rw-r--r--   0        0        0      594 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/scalars.py
+-rw-r--r--   0        0        0      288 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/segments.py
+-rw-r--r--   0        0        0      499 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/segments_by_resource_name.py
+-rw-r--r--   0        0        0      592 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/snowflake_credential_secret_changed.py
+-rw-r--r--   0        0        0      566 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/start_source.py
+-rw-r--r--   0        0        0      550 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/stop_source.py
+-rw-r--r--   0        0        0      502 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_athena_credential.py
+-rw-r--r--   0        0        0      454 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_athena_source.py
+-rw-r--r--   0        0        0      441 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_credential.py
+-rw-r--r--   0        0        0      524 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      464 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_kinesis_source.py
+-rw-r--r--   0        0        0      522 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_redshift_credential.py
+-rw-r--r--   0        0        0      476 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_redshift_source.py
+-rw-r--r--   0        0        0      414 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_s3_source.py
+-rw-r--r--   0        0        0      636 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_categorical_distribution_validator.py
+-rw-r--r--   0        0        0      469 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_channel_namespace.py
+-rw-r--r--   0        0        0      499 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_credential_namespace.py
+-rw-r--r--   0        0        0      509 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_destination_namespace.py
+-rw-r--r--   0        0        0      464 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_fixed_batch_window.py
+-rw-r--r--   0        0        0      491 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_freshness_validator.py
+-rw-r--r--   0        0        0      535 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      477 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_big_query_source.py
+-rw-r--r--   0        0        0      441 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_credential.py
+-rw-r--r--   0        0        0      496 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      455 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      464 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_storage_source.py
+-rw-r--r--   0        0        0      560 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_identity_provider_namespace.py
+-rw-r--r--   0        0        0      590 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_kafka_sasl_ssl_plain_credential.py
+-rw-r--r--   0        0        0      413 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_kafka_source.py
+-rw-r--r--   0        0        0      494 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_kafka_ssl_credential.py
+-rw-r--r--   0        0        0      534 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_local_identity_provider.py
+-rw-r--r--   0        0        0      483 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_notification_rule.py
+-rw-r--r--   0        0        0      560 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_notification_rule_namespace.py
+-rw-r--r--   0        0        0      540 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_numeric_anomaly_validator.py
+-rw-r--r--   0        0        0      596 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_numeric_distribution_validator.py
+-rw-r--r--   0        0        0      469 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_numeric_validator.py
+-rw-r--r--   0        0        0      512 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_postgre_sql_credential.py
+-rw-r--r--   0        0        0      464 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_postgre_sql_source.py
+-rw-r--r--   0        0        0      520 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_relative_time_validator.py
+-rw-r--r--   0        0        0      540 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_relative_volume_validator.py
+-rw-r--r--   0        0        0      524 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_saml_identity_provider.py
+-rw-r--r--   0        0        0      519 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_segmentation_namespace.py
+-rw-r--r--   0        0        0      473 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_sessionized_window.py
+-rw-r--r--   0        0        0      425 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_slack_channel.py
+-rw-r--r--   0        0        0      501 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_snowflake_credential.py
+-rw-r--r--   0        0        0      513 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_snowflake_destination.py
+-rw-r--r--   0        0        0      453 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_snowflake_source.py
+-rw-r--r--   0        0        0      459 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_source_namespace.py
+-rw-r--r--   0        0        0      443 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_tumbling_window.py
+-rw-r--r--   0        0        0      324 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_user.py
+-rw-r--r--   0        0        0      439 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_user_namespace.py
+-rw-r--r--   0        0        0      491 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_validator_namespace.py
+-rw-r--r--   0        0        0    57176 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0    56052 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0    58306 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      459 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_volume_validator.py
+-rw-r--r--   0        0        0      445 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_webhook_channel.py
+-rw-r--r--   0        0        0      459 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_window_namespace.py
+-rw-r--r--   0        0        0      265 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/metadata.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/py.typed
+-rw-r--r--   0        0        0      135 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/resource/__init__.py
+-rw-r--r--   0        0        0    21078 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/resource/_diff.py
+-rw-r--r--   0        0        0     1505 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_diff_util.py
+-rw-r--r--   0        0        0     4326 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_diffable.py
+-rw-r--r--   0        0        0     1579 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_errors.py
+-rw-r--r--   0        0        0     4002 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_field_selector.py
+-rw-r--r--   0        0        0    19682 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_resource.py
+-rw-r--r--   0        0        0     1355 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_resource_graph.py
+-rw-r--r--   0        0        0     6860 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_serde.py
+-rw-r--r--   0        0        0    21679 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_server_resources.py
+-rw-r--r--   0        0        0     5273 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_update_namespace.py
+-rw-r--r--   0        0        0      847 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_util.py
+-rw-r--r--   0        0        0     5027 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/channels.py
+-rw-r--r--   0        0        0     8164 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/credentials.py
+-rw-r--r--   0        0        0     5601 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/destinations.py
+-rw-r--r--   0        0        0     6262 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/filters.py
+-rw-r--r--   0        0        0     4846 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/notification_rules.py
+-rw-r--r--   0        0        0     2040 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/segmentations.py
+-rw-r--r--   0        0        0    26091 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/sources.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/tests/__init__.py
+-rw-r--r--   0        0        0    15408 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/tests/test__diff.py
+-rw-r--r--   0        0        0     1905 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/tests/test__field_selector.py
+-rw-r--r--   0        0        0    16357 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/tests/test__resource.py
+-rw-r--r--   0        0        0     5638 2023-07-21 13:06:25.410451 validio_sdk-0.6.4/validio_sdk/resource/thresholds.py
+-rw-r--r--   0        0        0    33277 2023-07-21 13:06:25.410451 validio_sdk-0.6.4/validio_sdk/resource/validators.py
+-rw-r--r--   0        0        0     5995 2023-07-21 13:06:25.410451 validio_sdk-0.6.4/validio_sdk/resource/windows.py
+-rw-r--r--   0        0        0     1377 2023-07-21 13:06:25.410451 validio_sdk-0.6.4/validio_sdk/scalars.py
+-rw-r--r--   0        0        0     1813 2023-07-21 13:06:25.410451 validio_sdk-0.6.4/validio_sdk/util.py
+-rw-r--r--   0        0        0     2382 2023-07-21 13:06:25.410451 validio_sdk-0.6.4/validio_sdk/validio_client.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 validio_sdk-0.6.4/PKG-INFO
```

### Comparing `validio_sdk-0.6.3/LICENSE` & `validio_sdk-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/pyproject.toml` & `validio_sdk-0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "validio-sdk"
 # This version does not represent the released version or any tag. For each
 # release we automatically bump this before building and publishing so this
 # should be kept at 0.0.1dev1
-version = "0.6.3"
+version = "0.6.4"
 description = "SDK to interact with the Validio platform"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 homepage = "https://validio.io/"
 documentation = "https://dev.validio.io/sdk-docs"
 packages = [{ include = "validio_sdk" }]
 exclude = ["./validio_sdk/bin/pull_graphql.py", "./schema/**", "./plugins/**", "./examples/**"]
```

### Comparing `validio_sdk-0.6.3/validio_sdk/__init__.py` & `validio_sdk-0.6.4/validio_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/code/apply.py` & `validio_sdk-0.6.4/validio_sdk/code/apply.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/code/plan.py` & `validio_sdk-0.6.4/validio_sdk/code/plan.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/code/scaffold.py` & `validio_sdk-0.6.4/validio_sdk/code/scaffold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/config.py` & `validio_sdk-0.6.4/validio_sdk/config.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/__init__.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,17 +93,17 @@
     CreateGcpPubSubSource,
     CreateGcpPubSubSourceGcpPubSubSourceCreate,
 )
 from .create_gcp_storage_source import (
     CreateGcpStorageSource,
     CreateGcpStorageSourceGcpStorageSourceCreate,
 )
-from .create_kafka_sasl_plain_credential import (
-    CreateKafkaSaslPlainCredential,
-    CreateKafkaSaslPlainCredentialKafkaSaslPlainCredentialCreate,
+from .create_kafka_sasl_ssl_plain_credential import (
+    CreateKafkaSaslSslPlainCredential,
+    CreateKafkaSaslSslPlainCredentialKafkaSaslSslPlainCredentialCreate,
 )
 from .create_kafka_source import CreateKafkaSource, CreateKafkaSourceKafkaSourceCreate
 from .create_kafka_ssl_credential import (
     CreateKafkaSslCredential,
     CreateKafkaSslCredentialKafkaSslCredentialCreate,
 )
 from .create_notification_rule import (
@@ -335,16 +335,16 @@
     CredentialCreationCredentialAwsAthenaCredential,
     CredentialCreationCredentialAwsAthenaCredentialConfig,
     CredentialCreationCredentialAwsCredential,
     CredentialCreationCredentialAwsCredentialConfig,
     CredentialCreationCredentialAwsRedshiftCredential,
     CredentialCreationCredentialAwsRedshiftCredentialConfig,
     CredentialCreationCredentialCredential,
-    CredentialCreationCredentialKafkaSASLPlainCredential,
-    CredentialCreationCredentialKafkaSASLPlainCredentialConfig,
+    CredentialCreationCredentialKafkaSaslSSLPlainCredential,
+    CredentialCreationCredentialKafkaSaslSSLPlainCredentialConfig,
     CredentialCreationCredentialKafkaSSLCredential,
     CredentialCreationCredentialKafkaSSLCredentialConfig,
     CredentialCreationCredentialPostgreSqlCredential,
     CredentialCreationCredentialPostgreSqlCredentialConfig,
     CredentialCreationCredentialSnowflakeCredential,
     CredentialCreationCredentialSnowflakeCredentialConfig,
     CredentialCreationErrors,
@@ -354,16 +354,16 @@
     CredentialUpdateCredentialAwsAthenaCredential,
     CredentialUpdateCredentialAwsAthenaCredentialConfig,
     CredentialUpdateCredentialAwsCredential,
     CredentialUpdateCredentialAwsCredentialConfig,
     CredentialUpdateCredentialAwsRedshiftCredential,
     CredentialUpdateCredentialAwsRedshiftCredentialConfig,
     CredentialUpdateCredentialCredential,
-    CredentialUpdateCredentialKafkaSASLPlainCredential,
-    CredentialUpdateCredentialKafkaSASLPlainCredentialConfig,
+    CredentialUpdateCredentialKafkaSaslSSLPlainCredential,
+    CredentialUpdateCredentialKafkaSaslSSLPlainCredentialConfig,
     CredentialUpdateCredentialKafkaSSLCredential,
     CredentialUpdateCredentialKafkaSSLCredentialConfig,
     CredentialUpdateCredentialPostgreSqlCredential,
     CredentialUpdateCredentialPostgreSqlCredentialConfig,
     CredentialUpdateCredentialSnowflakeCredential,
     CredentialUpdateCredentialSnowflakeCredentialConfig,
     CredentialUpdateErrors,
@@ -823,16 +823,16 @@
     GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredential,
     GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredentialConfig,
     GetCredentialByResourceNameCredentialByResourceNameAwsCredential,
     GetCredentialByResourceNameCredentialByResourceNameAwsCredentialConfig,
     GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredential,
     GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredentialConfig,
     GetCredentialByResourceNameCredentialByResourceNameCredential,
-    GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential,
-    GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredentialConfig,
+    GetCredentialByResourceNameCredentialByResourceNameKafkaSaslSSLPlainCredential,
+    GetCredentialByResourceNameCredentialByResourceNameKafkaSaslSSLPlainCredentialConfig,
     GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredential,
     GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredentialConfig,
     GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredential,
     GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredentialConfig,
     GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredential,
     GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredentialConfig,
 )
@@ -1381,17 +1381,17 @@
     GcpStorageInferSchemaInput,
     GcpStorageSourceCreateInput,
     GcpStorageSourceUpdateInput,
     IdentityDeleteInput,
     IdentityProviderDeleteInput,
     IncidentsInput,
     KafkaInferSchemaInput,
-    KafkaSASLPlainCredentialCreateInput,
-    KafkaSASLPlainCredentialSecretChangedInput,
-    KafkaSASLPlainCredentialUpdateInput,
+    KafkaSaslSSLPlainCredentialCreateInput,
+    KafkaSaslSSLPlainCredentialSecretChangedInput,
+    KafkaSaslSSLPlainCredentialUpdateInput,
     KafkaSourceCreateInput,
     KafkaSourceUpdateInput,
     KafkaSSLCredentialCreateInput,
     KafkaSSLCredentialSecretChangedInput,
     KafkaSSLCredentialUpdateInput,
     LocalIdentityProviderUpdateInput,
     MonotonicThresholdCreateInput,
@@ -1452,33 +1452,33 @@
     ValidatorWithFixedThresholdUpdateInput,
     ValidatorWithMonotonicThresholdUpdateInput,
     VolumeValidatorCreateInput,
     VolumeValidatorUpdateInput,
     WebhookChannelCreateInput,
     WebhookChannelUpdateInput,
 )
-from .kafka_sasl_plain_credential_secret_changed import (
-    KafkaSaslPlainCredentialSecretChanged,
-    KafkaSaslPlainCredentialSecretChangedKafkaSaslPlainCredentialSecretChanged,
+from .kafka_sasl_ssl_plain_credential_secret_changed import (
+    KafkaSaslSslPlainCredentialSecretChanged,
+    KafkaSaslSslPlainCredentialSecretChangedKafkaSaslSslPlainCredentialSecretChanged,
 )
 from .kafka_ssl_credential_secret_changed import (
     KafkaSslCredentialSecretChanged,
     KafkaSslCredentialSecretChangedKafkaSslCredentialSecretChanged,
 )
 from .list_credentials import (
     ListCredentials,
     ListCredentialsCredentialsListAwsAthenaCredential,
     ListCredentialsCredentialsListAwsAthenaCredentialConfig,
     ListCredentialsCredentialsListAwsCredential,
     ListCredentialsCredentialsListAwsCredentialConfig,
     ListCredentialsCredentialsListAwsRedshiftCredential,
     ListCredentialsCredentialsListAwsRedshiftCredentialConfig,
     ListCredentialsCredentialsListCredential,
-    ListCredentialsCredentialsListKafkaSASLPlainCredential,
-    ListCredentialsCredentialsListKafkaSASLPlainCredentialConfig,
+    ListCredentialsCredentialsListKafkaSaslSSLPlainCredential,
+    ListCredentialsCredentialsListKafkaSaslSSLPlainCredentialConfig,
     ListCredentialsCredentialsListKafkaSSLCredential,
     ListCredentialsCredentialsListKafkaSSLCredentialConfig,
     ListCredentialsCredentialsListPostgreSqlCredential,
     ListCredentialsCredentialsListPostgreSqlCredentialConfig,
     ListCredentialsCredentialsListSnowflakeCredential,
     ListCredentialsCredentialsListSnowflakeCredentialConfig,
 )
@@ -1765,17 +1765,17 @@
     UpdateGcpStorageSource,
     UpdateGcpStorageSourceGcpStorageSourceUpdate,
 )
 from .update_identity_provider_namespace import (
     UpdateIdentityProviderNamespace,
     UpdateIdentityProviderNamespaceIdentityProviderNamespaceUpdate,
 )
-from .update_kafka_sasl_plain_credential import (
-    UpdateKafkaSaslPlainCredential,
-    UpdateKafkaSaslPlainCredentialKafkaSaslPlainCredentialUpdate,
+from .update_kafka_sasl_ssl_plain_credential import (
+    UpdateKafkaSaslSslPlainCredential,
+    UpdateKafkaSaslSslPlainCredentialKafkaSaslSslPlainCredentialUpdate,
 )
 from .update_kafka_source import UpdateKafkaSource, UpdateKafkaSourceKafkaSourceUpdate
 from .update_kafka_ssl_credential import (
     UpdateKafkaSslCredential,
     UpdateKafkaSslCredentialKafkaSslCredentialUpdate,
 )
 from .update_local_identity_provider import (
@@ -2262,16 +2262,16 @@
     "CreateGcpCredentialGcpCredentialCreate",
     "CreateGcpPubSubLiteSource",
     "CreateGcpPubSubLiteSourceGcpPubSubLiteSourceCreate",
     "CreateGcpPubSubSource",
     "CreateGcpPubSubSourceGcpPubSubSourceCreate",
     "CreateGcpStorageSource",
     "CreateGcpStorageSourceGcpStorageSourceCreate",
-    "CreateKafkaSaslPlainCredential",
-    "CreateKafkaSaslPlainCredentialKafkaSaslPlainCredentialCreate",
+    "CreateKafkaSaslSslPlainCredential",
+    "CreateKafkaSaslSslPlainCredentialKafkaSaslSslPlainCredentialCreate",
     "CreateKafkaSource",
     "CreateKafkaSourceKafkaSourceCreate",
     "CreateKafkaSslCredential",
     "CreateKafkaSslCredentialKafkaSslCredentialCreate",
     "CreateNotificationRule",
     "CreateNotificationRuleNotificationRuleCreate",
     "CreateNumericAnomalyValidatorWithDynamicThreshold",
@@ -2332,18 +2332,18 @@
     "CredentialCreationCredentialAwsAthenaCredential",
     "CredentialCreationCredentialAwsAthenaCredentialConfig",
     "CredentialCreationCredentialAwsCredential",
     "CredentialCreationCredentialAwsCredentialConfig",
     "CredentialCreationCredentialAwsRedshiftCredential",
     "CredentialCreationCredentialAwsRedshiftCredentialConfig",
     "CredentialCreationCredentialCredential",
-    "CredentialCreationCredentialKafkaSASLPlainCredential",
-    "CredentialCreationCredentialKafkaSASLPlainCredentialConfig",
     "CredentialCreationCredentialKafkaSSLCredential",
     "CredentialCreationCredentialKafkaSSLCredentialConfig",
+    "CredentialCreationCredentialKafkaSaslSSLPlainCredential",
+    "CredentialCreationCredentialKafkaSaslSSLPlainCredentialConfig",
     "CredentialCreationCredentialPostgreSqlCredential",
     "CredentialCreationCredentialPostgreSqlCredentialConfig",
     "CredentialCreationCredentialSnowflakeCredential",
     "CredentialCreationCredentialSnowflakeCredentialConfig",
     "CredentialCreationErrors",
     "CredentialSecretChanged",
     "CredentialSecretChangedErrors",
@@ -2351,18 +2351,18 @@
     "CredentialUpdateCredentialAwsAthenaCredential",
     "CredentialUpdateCredentialAwsAthenaCredentialConfig",
     "CredentialUpdateCredentialAwsCredential",
     "CredentialUpdateCredentialAwsCredentialConfig",
     "CredentialUpdateCredentialAwsRedshiftCredential",
     "CredentialUpdateCredentialAwsRedshiftCredentialConfig",
     "CredentialUpdateCredentialCredential",
-    "CredentialUpdateCredentialKafkaSASLPlainCredential",
-    "CredentialUpdateCredentialKafkaSASLPlainCredentialConfig",
     "CredentialUpdateCredentialKafkaSSLCredential",
     "CredentialUpdateCredentialKafkaSSLCredentialConfig",
+    "CredentialUpdateCredentialKafkaSaslSSLPlainCredential",
+    "CredentialUpdateCredentialKafkaSaslSSLPlainCredentialConfig",
     "CredentialUpdateCredentialPostgreSqlCredential",
     "CredentialUpdateCredentialPostgreSqlCredentialConfig",
     "CredentialUpdateCredentialSnowflakeCredential",
     "CredentialUpdateCredentialSnowflakeCredentialConfig",
     "CredentialUpdateErrors",
     "CsvParserInput",
     "DecisionBoundsType",
@@ -2481,18 +2481,18 @@
     "GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredential",
     "GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredentialConfig",
     "GetCredentialByResourceNameCredentialByResourceNameAwsCredential",
     "GetCredentialByResourceNameCredentialByResourceNameAwsCredentialConfig",
     "GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredential",
     "GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredentialConfig",
     "GetCredentialByResourceNameCredentialByResourceNameCredential",
-    "GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential",
-    "GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredentialConfig",
     "GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredential",
     "GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredentialConfig",
+    "GetCredentialByResourceNameCredentialByResourceNameKafkaSaslSSLPlainCredential",
+    "GetCredentialByResourceNameCredentialByResourceNameKafkaSaslSSLPlainCredentialConfig",
     "GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredential",
     "GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredentialConfig",
     "GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredential",
     "GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredentialConfig",
     "GetDestinationByResourceName",
     "GetDestinationByResourceNameDestinationByResourceNameAwsKinesisDestination",
     "GetDestinationByResourceNameDestinationByResourceNameAwsKinesisDestinationConfig",
@@ -2970,38 +2970,38 @@
     "InferGcpPubSubLiteSchema",
     "InferGcpPubSubSchema",
     "InferGcpStorageSchema",
     "InferKafkaSchema",
     "InferPostgreSqlSchema",
     "InferSnowflakeSchema",
     "KafkaInferSchemaInput",
-    "KafkaSASLPlainCredentialCreateInput",
-    "KafkaSASLPlainCredentialSecretChangedInput",
-    "KafkaSASLPlainCredentialUpdateInput",
     "KafkaSSLCredentialCreateInput",
     "KafkaSSLCredentialSecretChangedInput",
     "KafkaSSLCredentialUpdateInput",
-    "KafkaSaslPlainCredentialSecretChanged",
-    "KafkaSaslPlainCredentialSecretChangedKafkaSaslPlainCredentialSecretChanged",
+    "KafkaSaslSSLPlainCredentialCreateInput",
+    "KafkaSaslSSLPlainCredentialSecretChangedInput",
+    "KafkaSaslSSLPlainCredentialUpdateInput",
+    "KafkaSaslSslPlainCredentialSecretChanged",
+    "KafkaSaslSslPlainCredentialSecretChangedKafkaSaslSslPlainCredentialSecretChanged",
     "KafkaSourceCreateInput",
     "KafkaSourceUpdateInput",
     "KafkaSslCredentialSecretChanged",
     "KafkaSslCredentialSecretChangedKafkaSslCredentialSecretChanged",
     "ListCredentials",
     "ListCredentialsCredentialsListAwsAthenaCredential",
     "ListCredentialsCredentialsListAwsAthenaCredentialConfig",
     "ListCredentialsCredentialsListAwsCredential",
     "ListCredentialsCredentialsListAwsCredentialConfig",
     "ListCredentialsCredentialsListAwsRedshiftCredential",
     "ListCredentialsCredentialsListAwsRedshiftCredentialConfig",
     "ListCredentialsCredentialsListCredential",
-    "ListCredentialsCredentialsListKafkaSASLPlainCredential",
-    "ListCredentialsCredentialsListKafkaSASLPlainCredentialConfig",
     "ListCredentialsCredentialsListKafkaSSLCredential",
     "ListCredentialsCredentialsListKafkaSSLCredentialConfig",
+    "ListCredentialsCredentialsListKafkaSaslSSLPlainCredential",
+    "ListCredentialsCredentialsListKafkaSaslSSLPlainCredentialConfig",
     "ListCredentialsCredentialsListPostgreSqlCredential",
     "ListCredentialsCredentialsListPostgreSqlCredentialConfig",
     "ListCredentialsCredentialsListSnowflakeCredential",
     "ListCredentialsCredentialsListSnowflakeCredentialConfig",
     "ListDestinations",
     "ListDestinationsDestinationsListAwsKinesisDestination",
     "ListDestinationsDestinationsListAwsKinesisDestinationConfig",
@@ -3444,16 +3444,16 @@
     "UpdateGcpPubSubLiteSourceGcpPubSubLiteSourceUpdate",
     "UpdateGcpPubSubSource",
     "UpdateGcpPubSubSourceGcpPubSubSourceUpdate",
     "UpdateGcpStorageSource",
     "UpdateGcpStorageSourceGcpStorageSourceUpdate",
     "UpdateIdentityProviderNamespace",
     "UpdateIdentityProviderNamespaceIdentityProviderNamespaceUpdate",
-    "UpdateKafkaSaslPlainCredential",
-    "UpdateKafkaSaslPlainCredentialKafkaSaslPlainCredentialUpdate",
+    "UpdateKafkaSaslSslPlainCredential",
+    "UpdateKafkaSaslSslPlainCredentialKafkaSaslSslPlainCredentialUpdate",
     "UpdateKafkaSource",
     "UpdateKafkaSourceKafkaSourceUpdate",
     "UpdateKafkaSslCredential",
     "UpdateKafkaSslCredentialKafkaSslCredentialUpdate",
     "UpdateLocalIdentityProvider",
     "UpdateLocalIdentityProviderLocalIdentityProviderUpdate",
     "UpdateNotificationRule",
```

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/apply_validator_recommendation.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/apply_validator_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/async_base_client.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/async_base_client.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/aws_credential_secret_changed.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/aws_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/backfill_source.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/backfill_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/base_model.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/base_model.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/client.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,17 +100,17 @@
     CreateGcpPubSubSource,
     CreateGcpPubSubSourceGcpPubSubSourceCreate,
 )
 from .create_gcp_storage_source import (
     CreateGcpStorageSource,
     CreateGcpStorageSourceGcpStorageSourceCreate,
 )
-from .create_kafka_sasl_plain_credential import (
-    CreateKafkaSaslPlainCredential,
-    CreateKafkaSaslPlainCredentialKafkaSaslPlainCredentialCreate,
+from .create_kafka_sasl_ssl_plain_credential import (
+    CreateKafkaSaslSslPlainCredential,
+    CreateKafkaSaslSslPlainCredentialKafkaSaslSslPlainCredentialCreate,
 )
 from .create_kafka_source import CreateKafkaSource, CreateKafkaSourceKafkaSourceCreate
 from .create_kafka_ssl_credential import (
     CreateKafkaSslCredential,
     CreateKafkaSslCredentialKafkaSslCredentialCreate,
 )
 from .create_notification_rule import (
@@ -271,15 +271,15 @@
 )
 from .get_credential_by_resource_name import (
     GetCredentialByResourceName,
     GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredential,
     GetCredentialByResourceNameCredentialByResourceNameAwsCredential,
     GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredential,
     GetCredentialByResourceNameCredentialByResourceNameCredential,
-    GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential,
+    GetCredentialByResourceNameCredentialByResourceNameKafkaSaslSSLPlainCredential,
     GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredential,
     GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredential,
     GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredential,
 )
 from .get_destination_by_resource_name import (
     GetDestinationByResourceName,
     GetDestinationByResourceNameDestinationByResourceNameAwsKinesisDestination,
@@ -481,17 +481,17 @@
     GcpStorageInferSchemaInput,
     GcpStorageSourceCreateInput,
     GcpStorageSourceUpdateInput,
     IdentityDeleteInput,
     IdentityProviderDeleteInput,
     IncidentsInput,
     KafkaInferSchemaInput,
-    KafkaSASLPlainCredentialCreateInput,
-    KafkaSASLPlainCredentialSecretChangedInput,
-    KafkaSASLPlainCredentialUpdateInput,
+    KafkaSaslSSLPlainCredentialCreateInput,
+    KafkaSaslSSLPlainCredentialSecretChangedInput,
+    KafkaSaslSSLPlainCredentialUpdateInput,
     KafkaSourceCreateInput,
     KafkaSourceUpdateInput,
     KafkaSSLCredentialCreateInput,
     KafkaSSLCredentialSecretChangedInput,
     KafkaSSLCredentialUpdateInput,
     LocalIdentityProviderUpdateInput,
     MonotonicThresholdCreateInput,
@@ -547,29 +547,29 @@
     ValidatorWithFixedThresholdUpdateInput,
     ValidatorWithMonotonicThresholdUpdateInput,
     VolumeValidatorCreateInput,
     VolumeValidatorUpdateInput,
     WebhookChannelCreateInput,
     WebhookChannelUpdateInput,
 )
-from .kafka_sasl_plain_credential_secret_changed import (
-    KafkaSaslPlainCredentialSecretChanged,
-    KafkaSaslPlainCredentialSecretChangedKafkaSaslPlainCredentialSecretChanged,
+from .kafka_sasl_ssl_plain_credential_secret_changed import (
+    KafkaSaslSslPlainCredentialSecretChanged,
+    KafkaSaslSslPlainCredentialSecretChangedKafkaSaslSslPlainCredentialSecretChanged,
 )
 from .kafka_ssl_credential_secret_changed import (
     KafkaSslCredentialSecretChanged,
     KafkaSslCredentialSecretChangedKafkaSslCredentialSecretChanged,
 )
 from .list_credentials import (
     ListCredentials,
     ListCredentialsCredentialsListAwsAthenaCredential,
     ListCredentialsCredentialsListAwsCredential,
     ListCredentialsCredentialsListAwsRedshiftCredential,
     ListCredentialsCredentialsListCredential,
-    ListCredentialsCredentialsListKafkaSASLPlainCredential,
+    ListCredentialsCredentialsListKafkaSaslSSLPlainCredential,
     ListCredentialsCredentialsListKafkaSSLCredential,
     ListCredentialsCredentialsListPostgreSqlCredential,
     ListCredentialsCredentialsListSnowflakeCredential,
 )
 from .list_destinations import (
     ListDestinations,
     ListDestinationsDestinationsListAwsKinesisDestination,
@@ -704,17 +704,17 @@
     UpdateGcpStorageSource,
     UpdateGcpStorageSourceGcpStorageSourceUpdate,
 )
 from .update_identity_provider_namespace import (
     UpdateIdentityProviderNamespace,
     UpdateIdentityProviderNamespaceIdentityProviderNamespaceUpdate,
 )
-from .update_kafka_sasl_plain_credential import (
-    UpdateKafkaSaslPlainCredential,
-    UpdateKafkaSaslPlainCredentialKafkaSaslPlainCredentialUpdate,
+from .update_kafka_sasl_ssl_plain_credential import (
+    UpdateKafkaSaslSslPlainCredential,
+    UpdateKafkaSaslSslPlainCredentialKafkaSaslSslPlainCredentialUpdate,
 )
 from .update_kafka_source import UpdateKafkaSource, UpdateKafkaSourceKafkaSourceUpdate
 from .update_kafka_ssl_credential import (
     UpdateKafkaSslCredential,
     UpdateKafkaSslCredentialKafkaSslCredentialUpdate,
 )
 from .update_local_identity_provider import (
@@ -1009,15 +1009,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -1262,15 +1262,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -1588,15 +1588,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -2661,15 +2661,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -3936,15 +3936,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -4448,21 +4448,21 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateGcpStorageSource.parse_obj(data).gcp_storage_source_create
 
-    async def create_kafka_sasl_plain_credential(
-        self, input: KafkaSASLPlainCredentialCreateInput
-    ) -> CreateKafkaSaslPlainCredentialKafkaSaslPlainCredentialCreate:
+    async def create_kafka_sasl_ssl_plain_credential(
+        self, input: KafkaSaslSSLPlainCredentialCreateInput
+    ) -> CreateKafkaSaslSslPlainCredentialKafkaSaslSslPlainCredentialCreate:
         query = gql(
             """
-            mutation CreateKafkaSaslPlainCredential($input: KafkaSASLPlainCredentialCreateInput!) {
-              kafkaSaslPlainCredentialCreate(input: $input) {
+            mutation CreateKafkaSaslSslPlainCredential($input: KafkaSaslSSLPlainCredentialCreateInput!) {
+              kafkaSaslSslPlainCredentialCreate(input: $input) {
                 ...CredentialCreation
               }
             }
 
             fragment CredentialCreation on CredentialCreateResult {
               __typename
               errors {
@@ -4517,15 +4517,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -4535,17 +4535,17 @@
               message
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
-        return CreateKafkaSaslPlainCredential.parse_obj(
+        return CreateKafkaSaslSslPlainCredential.parse_obj(
             data
-        ).kafka_sasl_plain_credential_create
+        ).kafka_sasl_ssl_plain_credential_create
 
     async def create_kafka_source(
         self, input: KafkaSourceCreateInput
     ) -> CreateKafkaSourceKafkaSourceCreate:
         query = gql(
             """
             mutation CreateKafkaSource($input: KafkaSourceCreateInput!) {
@@ -4772,15 +4772,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -7533,15 +7533,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -9639,15 +9639,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -11311,15 +11311,15 @@
             GetCredentialByResourceNameCredentialByResourceNameCredential,
             GetCredentialByResourceNameCredentialByResourceNameAwsCredential,
             GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredential,
             GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredential,
             GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredential,
             GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredential,
             GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredential,
-            GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential,
+            GetCredentialByResourceNameCredentialByResourceNameKafkaSaslSSLPlainCredential,
         ]
     ]:
         query = gql(
             """
             query GetCredentialByResourceName($resourceName: String!, $resourceNamespace: String! = "default") {
               credentialByResourceName(
                 resourceName: $resourceName
@@ -11373,15 +11373,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
             """
@@ -13565,21 +13565,21 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return InferSnowflakeSchema.parse_obj(data).snowflake_infer_schema
 
-    async def kafka_sasl_plain_credential_secret_changed(
-        self, input: KafkaSASLPlainCredentialSecretChangedInput
-    ) -> KafkaSaslPlainCredentialSecretChangedKafkaSaslPlainCredentialSecretChanged:
+    async def kafka_sasl_ssl_plain_credential_secret_changed(
+        self, input: KafkaSaslSSLPlainCredentialSecretChangedInput
+    ) -> KafkaSaslSslPlainCredentialSecretChangedKafkaSaslSslPlainCredentialSecretChanged:
         query = gql(
             """
-            query KafkaSaslPlainCredentialSecretChanged($input: KafkaSASLPlainCredentialSecretChangedInput!) {
-              kafkaSaslPlainCredentialSecretChanged(input: $input) {
+            query KafkaSaslSslPlainCredentialSecretChanged($input: KafkaSaslSSLPlainCredentialSecretChangedInput!) {
+              kafkaSaslSslPlainCredentialSecretChanged(input: $input) {
                 ...CredentialSecretChanged
               }
             }
 
             fragment CredentialSecretChanged on CredentialSecretChangedResult {
               errors {
                 ...ErrorDetails
@@ -13593,17 +13593,17 @@
               message
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
-        return KafkaSaslPlainCredentialSecretChanged.parse_obj(
+        return KafkaSaslSslPlainCredentialSecretChanged.parse_obj(
             data
-        ).kafka_sasl_plain_credential_secret_changed
+        ).kafka_sasl_ssl_plain_credential_secret_changed
 
     async def kafka_ssl_credential_secret_changed(
         self, input: KafkaSSLCredentialSecretChangedInput
     ) -> KafkaSslCredentialSecretChangedKafkaSslCredentialSecretChanged:
         query = gql(
             """
             query KafkaSslCredentialSecretChanged($input: KafkaSSLCredentialSecretChangedInput!) {
@@ -13640,15 +13640,15 @@
             ListCredentialsCredentialsListCredential,
             ListCredentialsCredentialsListAwsCredential,
             ListCredentialsCredentialsListAwsAthenaCredential,
             ListCredentialsCredentialsListAwsRedshiftCredential,
             ListCredentialsCredentialsListPostgreSqlCredential,
             ListCredentialsCredentialsListSnowflakeCredential,
             ListCredentialsCredentialsListKafkaSSLCredential,
-            ListCredentialsCredentialsListKafkaSASLPlainCredential,
+            ListCredentialsCredentialsListKafkaSaslSSLPlainCredential,
         ]
     ]:
         query = gql(
             """
             query ListCredentials($filter: ResourceFilter) {
               credentialsList(filter: $filter) {
                 ...CredentialDetails
@@ -13699,15 +13699,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
             """
@@ -14580,15 +14580,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -14832,15 +14832,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -15157,15 +15157,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -16615,15 +16615,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -17169,21 +17169,21 @@
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return UpdateIdentityProviderNamespace.parse_obj(
             data
         ).identity_provider_namespace_update
 
-    async def update_kafka_sasl_plain_credential(
-        self, input: KafkaSASLPlainCredentialUpdateInput
-    ) -> UpdateKafkaSaslPlainCredentialKafkaSaslPlainCredentialUpdate:
+    async def update_kafka_sasl_ssl_plain_credential(
+        self, input: KafkaSaslSSLPlainCredentialUpdateInput
+    ) -> UpdateKafkaSaslSslPlainCredentialKafkaSaslSslPlainCredentialUpdate:
         query = gql(
             """
-            mutation UpdateKafkaSaslPlainCredential($input: KafkaSASLPlainCredentialUpdateInput!) {
-              kafkaSaslPlainCredentialUpdate(input: $input) {
+            mutation UpdateKafkaSaslSslPlainCredential($input: KafkaSaslSSLPlainCredentialUpdateInput!) {
+              kafkaSaslSslPlainCredentialUpdate(input: $input) {
                 ...CredentialUpdate
               }
             }
 
             fragment CredentialDetails on Credential {
               __typename
               id
@@ -17228,15 +17228,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -17255,17 +17255,17 @@
               message
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
-        return UpdateKafkaSaslPlainCredential.parse_obj(
+        return UpdateKafkaSaslSslPlainCredential.parse_obj(
             data
-        ).kafka_sasl_plain_credential_update
+        ).kafka_sasl_ssl_plain_credential_update
 
     async def update_kafka_source(
         self, input: KafkaSourceUpdateInput
     ) -> UpdateKafkaSourceKafkaSourceUpdate:
         query = gql(
             """
             mutation UpdateKafkaSource($input: KafkaSourceUpdateInput!) {
@@ -17482,15 +17482,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -18680,15 +18680,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
 
@@ -19771,15 +19771,15 @@
               }
               ... on KafkaSSLCredential {
                 config {
                   bootstrapServers
                   caCertificate
                 }
               }
-              ... on KafkaSASLPlainCredential {
+              ... on KafkaSaslSSLPlainCredential {
                 config {
                   bootstrapServers
                   username
                 }
               }
             }
```

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_aws_kinesis_destination.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_kinesis_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_aws_redshift_credential.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_redshift_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_gcp_big_query_destination.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_big_query_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_kafka_sasl_plain_credential.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/kafka_sasl_ssl_plain_credential_secret_changed.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from pydantic import Field
 
 from .base_model import BaseModel
-from .fragments import CredentialCreation
+from .fragments import CredentialSecretChanged
 
 
-class CreateKafkaSaslPlainCredential(BaseModel):
-    kafka_sasl_plain_credential_create: "CreateKafkaSaslPlainCredentialKafkaSaslPlainCredentialCreate" = Field(
-        alias="kafkaSaslPlainCredentialCreate"
+class KafkaSaslSslPlainCredentialSecretChanged(BaseModel):
+    kafka_sasl_ssl_plain_credential_secret_changed: "KafkaSaslSslPlainCredentialSecretChangedKafkaSaslSslPlainCredentialSecretChanged" = Field(
+        alias="kafkaSaslSslPlainCredentialSecretChanged"
     )
 
 
-class CreateKafkaSaslPlainCredentialKafkaSaslPlainCredentialCreate(CredentialCreation):
+class KafkaSaslSslPlainCredentialSecretChangedKafkaSaslSslPlainCredentialSecretChanged(
+    CredentialSecretChanged
+):
     pass
 
 
-CreateKafkaSaslPlainCredential.update_forward_refs()
-CreateKafkaSaslPlainCredentialKafkaSaslPlainCredentialCreate.update_forward_refs()
+KafkaSaslSslPlainCredentialSecretChanged.update_forward_refs()
+KafkaSaslSslPlainCredentialSecretChangedKafkaSaslSslPlainCredentialSecretChanged.update_forward_refs()
```

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_postgre_sql_credential.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_postgre_sql_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_saml_identity_provider.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_saml_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_snowflake_destination.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_snowflake_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/delete_credential.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/delete_credentials.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/delete_destination.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/delete_destinations.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/delete_segmentation.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_segmentation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/delete_source.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/delete_sources.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_sources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/delete_validators.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/delete_window.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_window.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/delete_windows.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/dismiss_validator_recommendation.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/dismiss_validator_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/enums.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/enums.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/exceptions.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/fragments.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
                 "CredentialCreationCredentialCredential",
                 "CredentialCreationCredentialAwsCredential",
                 "CredentialCreationCredentialAwsAthenaCredential",
                 "CredentialCreationCredentialAwsRedshiftCredential",
                 "CredentialCreationCredentialPostgreSqlCredential",
                 "CredentialCreationCredentialSnowflakeCredential",
                 "CredentialCreationCredentialKafkaSSLCredential",
-                "CredentialCreationCredentialKafkaSASLPlainCredential",
+                "CredentialCreationCredentialKafkaSaslSSLPlainCredential",
             ],
             Field(discriminator="typename__"),
         ]
     ]
 
 
 class CredentialCreationErrors(ErrorDetails):
@@ -325,26 +325,26 @@
 
 
 class CredentialCreationCredentialKafkaSSLCredentialConfig(BaseModel):
     bootstrap_servers: List[str] = Field(alias="bootstrapServers")
     ca_certificate: str = Field(alias="caCertificate")
 
 
-class CredentialCreationCredentialKafkaSASLPlainCredential(BaseModel):
-    typename__: Literal["KafkaSASLPlainCredential"] = Field(alias="__typename")
+class CredentialCreationCredentialKafkaSaslSSLPlainCredential(BaseModel):
+    typename__: Literal["KafkaSaslSSLPlainCredential"] = Field(alias="__typename")
     id: CredentialId
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
-    config: "CredentialCreationCredentialKafkaSASLPlainCredentialConfig"
+    config: "CredentialCreationCredentialKafkaSaslSSLPlainCredentialConfig"
 
 
-class CredentialCreationCredentialKafkaSASLPlainCredentialConfig(BaseModel):
+class CredentialCreationCredentialKafkaSaslSSLPlainCredentialConfig(BaseModel):
     bootstrap_servers: List[str] = Field(alias="bootstrapServers")
     username: str
 
 
 class CredentialSecretChanged(BaseModel):
     errors: List["CredentialSecretChangedErrors"]
     has_changed: Optional[bool] = Field(alias="hasChanged")
@@ -362,15 +362,15 @@
                 "CredentialUpdateCredentialCredential",
                 "CredentialUpdateCredentialAwsCredential",
                 "CredentialUpdateCredentialAwsAthenaCredential",
                 "CredentialUpdateCredentialAwsRedshiftCredential",
                 "CredentialUpdateCredentialPostgreSqlCredential",
                 "CredentialUpdateCredentialSnowflakeCredential",
                 "CredentialUpdateCredentialKafkaSSLCredential",
-                "CredentialUpdateCredentialKafkaSASLPlainCredential",
+                "CredentialUpdateCredentialKafkaSaslSSLPlainCredential",
             ],
             Field(discriminator="typename__"),
         ]
     ]
 
 
 class CredentialUpdateErrors(ErrorDetails):
@@ -485,26 +485,26 @@
 
 
 class CredentialUpdateCredentialKafkaSSLCredentialConfig(BaseModel):
     bootstrap_servers: List[str] = Field(alias="bootstrapServers")
     ca_certificate: str = Field(alias="caCertificate")
 
 
-class CredentialUpdateCredentialKafkaSASLPlainCredential(BaseModel):
-    typename__: Literal["KafkaSASLPlainCredential"] = Field(alias="__typename")
+class CredentialUpdateCredentialKafkaSaslSSLPlainCredential(BaseModel):
+    typename__: Literal["KafkaSaslSSLPlainCredential"] = Field(alias="__typename")
     id: CredentialId
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
-    config: "CredentialUpdateCredentialKafkaSASLPlainCredentialConfig"
+    config: "CredentialUpdateCredentialKafkaSaslSSLPlainCredentialConfig"
 
 
-class CredentialUpdateCredentialKafkaSASLPlainCredentialConfig(BaseModel):
+class CredentialUpdateCredentialKafkaSaslSSLPlainCredentialConfig(BaseModel):
     bootstrap_servers: List[str] = Field(alias="bootstrapServers")
     username: str
 
 
 class DestinationCreation(BaseModel):
     errors: List["DestinationCreationErrors"]
     destination: Optional[
@@ -4331,16 +4331,16 @@
 CredentialCreationCredentialAwsRedshiftCredentialConfig.update_forward_refs()
 CredentialCreationCredentialPostgreSqlCredential.update_forward_refs()
 CredentialCreationCredentialPostgreSqlCredentialConfig.update_forward_refs()
 CredentialCreationCredentialSnowflakeCredential.update_forward_refs()
 CredentialCreationCredentialSnowflakeCredentialConfig.update_forward_refs()
 CredentialCreationCredentialKafkaSSLCredential.update_forward_refs()
 CredentialCreationCredentialKafkaSSLCredentialConfig.update_forward_refs()
-CredentialCreationCredentialKafkaSASLPlainCredential.update_forward_refs()
-CredentialCreationCredentialKafkaSASLPlainCredentialConfig.update_forward_refs()
+CredentialCreationCredentialKafkaSaslSSLPlainCredential.update_forward_refs()
+CredentialCreationCredentialKafkaSaslSSLPlainCredentialConfig.update_forward_refs()
 CredentialSecretChanged.update_forward_refs()
 CredentialSecretChangedErrors.update_forward_refs()
 CredentialUpdate.update_forward_refs()
 CredentialUpdateErrors.update_forward_refs()
 CredentialUpdateCredentialCredential.update_forward_refs()
 CredentialUpdateCredentialAwsCredential.update_forward_refs()
 CredentialUpdateCredentialAwsCredentialConfig.update_forward_refs()
@@ -4350,16 +4350,16 @@
 CredentialUpdateCredentialAwsRedshiftCredentialConfig.update_forward_refs()
 CredentialUpdateCredentialPostgreSqlCredential.update_forward_refs()
 CredentialUpdateCredentialPostgreSqlCredentialConfig.update_forward_refs()
 CredentialUpdateCredentialSnowflakeCredential.update_forward_refs()
 CredentialUpdateCredentialSnowflakeCredentialConfig.update_forward_refs()
 CredentialUpdateCredentialKafkaSSLCredential.update_forward_refs()
 CredentialUpdateCredentialKafkaSSLCredentialConfig.update_forward_refs()
-CredentialUpdateCredentialKafkaSASLPlainCredential.update_forward_refs()
-CredentialUpdateCredentialKafkaSASLPlainCredentialConfig.update_forward_refs()
+CredentialUpdateCredentialKafkaSaslSSLPlainCredential.update_forward_refs()
+CredentialUpdateCredentialKafkaSaslSSLPlainCredentialConfig.update_forward_refs()
 DestinationCreation.update_forward_refs()
 DestinationCreationErrors.update_forward_refs()
 DestinationCreationDestinationDestination.update_forward_refs()
 DestinationCreationDestinationDestinationCredential.update_forward_refs()
 DestinationCreationDestinationGcpBigQueryDestination.update_forward_refs()
 DestinationCreationDestinationGcpBigQueryDestinationCredential.update_forward_refs()
 DestinationCreationDestinationGcpBigQueryDestinationConfig.update_forward_refs()
```

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/gcp_credential_secret_changed.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/gcp_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_channel_by_resource_name.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_channel_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_channels.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_channels.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_credential_by_resource_name.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_credential_by_resource_name.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                 "GetCredentialByResourceNameCredentialByResourceNameCredential",
                 "GetCredentialByResourceNameCredentialByResourceNameAwsCredential",
                 "GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredential",
                 "GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredential",
                 "GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredential",
                 "GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredential",
                 "GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredential",
-                "GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential",
+                "GetCredentialByResourceNameCredentialByResourceNameKafkaSaslSSLPlainCredential",
             ],
             Field(discriminator="typename__"),
         ]
     ] = Field(alias="credentialByResourceName")
 
 
 class GetCredentialByResourceNameCredentialByResourceNameCredential(BaseModel):
@@ -148,28 +148,28 @@
 class GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredentialConfig(
     BaseModel
 ):
     bootstrap_servers: List[str] = Field(alias="bootstrapServers")
     ca_certificate: str = Field(alias="caCertificate")
 
 
-class GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential(
+class GetCredentialByResourceNameCredentialByResourceNameKafkaSaslSSLPlainCredential(
     BaseModel
 ):
-    typename__: Literal["KafkaSASLPlainCredential"] = Field(alias="__typename")
+    typename__: Literal["KafkaSaslSSLPlainCredential"] = Field(alias="__typename")
     id: CredentialId
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
-    config: "GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredentialConfig"
+    config: "GetCredentialByResourceNameCredentialByResourceNameKafkaSaslSSLPlainCredentialConfig"
 
 
-class GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredentialConfig(
+class GetCredentialByResourceNameCredentialByResourceNameKafkaSaslSSLPlainCredentialConfig(
     BaseModel
 ):
     bootstrap_servers: List[str] = Field(alias="bootstrapServers")
     username: str
 
 
 GetCredentialByResourceName.update_forward_refs()
@@ -182,9 +182,9 @@
 GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredentialConfig.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredential.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredentialConfig.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredential.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredentialConfig.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredential.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredentialConfig.update_forward_refs()
-GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential.update_forward_refs()
-GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredentialConfig.update_forward_refs()
+GetCredentialByResourceNameCredentialByResourceNameKafkaSaslSSLPlainCredential.update_forward_refs()
+GetCredentialByResourceNameCredentialByResourceNameKafkaSaslSSLPlainCredentialConfig.update_forward_refs()
```

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_destination_by_resource_name.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_destination_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_identity_providers.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_identity_providers.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_incidents.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_recommendation.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_segmentation_by_resource_name.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_segmentation_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_source.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_source_by_resource_name.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_source_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_source_incidents.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_source_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_source_recommended_validators.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_source_recommended_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_validator.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_validator_by_resource_name.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_validator_segment_incidents.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator_segment_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_validator_segment_metrics.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator_segment_metrics.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/get_window_by_resource_name.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/get_window_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/input_types.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,35 +468,14 @@
 
 
 class KafkaInferSchemaInput(BaseModel):
     credential_id: CredentialId = Field(alias="credentialId")
     topic: str
 
 
-class KafkaSASLPlainCredentialCreateInput(BaseModel):
-    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
-    name: str
-    password: str
-    resource_name: Optional[str] = Field(alias="resourceName")
-    resource_namespace: Optional[str] = Field(alias="resourceNamespace")
-    username: str
-
-
-class KafkaSASLPlainCredentialSecretChangedInput(BaseModel):
-    id: CredentialId
-    password: str
-
-
-class KafkaSASLPlainCredentialUpdateInput(BaseModel):
-    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
-    id: CredentialId
-    password: str
-    username: str
-
-
 class KafkaSSLCredentialCreateInput(BaseModel):
     bootstrap_servers: List[str] = Field(alias="bootstrapServers")
     ca_certificate: str = Field(alias="caCertificate")
     client_certificate: str = Field(alias="clientCertificate")
     client_private_key: str = Field(alias="clientPrivateKey")
     client_private_key_password: str = Field(alias="clientPrivateKeyPassword")
     name: str
@@ -517,14 +496,35 @@
     ca_certificate: str = Field(alias="caCertificate")
     client_certificate: str = Field(alias="clientCertificate")
     client_private_key: str = Field(alias="clientPrivateKey")
     client_private_key_password: str = Field(alias="clientPrivateKeyPassword")
     id: CredentialId
 
 
+class KafkaSaslSSLPlainCredentialCreateInput(BaseModel):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    name: str
+    password: str
+    resource_name: Optional[str] = Field(alias="resourceName")
+    resource_namespace: Optional[str] = Field(alias="resourceNamespace")
+    username: str
+
+
+class KafkaSaslSSLPlainCredentialSecretChangedInput(BaseModel):
+    id: CredentialId
+    password: str
+
+
+class KafkaSaslSSLPlainCredentialUpdateInput(BaseModel):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    id: CredentialId
+    password: str
+    username: str
+
+
 class KafkaSourceCreateInput(BaseModel):
     credential_id: CredentialId = Field(alias="credentialId")
     jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
     name: str
     resource_name: Optional[str] = Field(alias="resourceName")
     resource_namespace: Optional[str] = Field(alias="resourceNamespace")
     topic: str
@@ -1084,20 +1084,20 @@
 GcpStorageInferSchemaInput.update_forward_refs()
 GcpStorageSourceCreateInput.update_forward_refs()
 GcpStorageSourceUpdateInput.update_forward_refs()
 IdentityDeleteInput.update_forward_refs()
 IdentityProviderDeleteInput.update_forward_refs()
 IncidentsInput.update_forward_refs()
 KafkaInferSchemaInput.update_forward_refs()
-KafkaSASLPlainCredentialCreateInput.update_forward_refs()
-KafkaSASLPlainCredentialSecretChangedInput.update_forward_refs()
-KafkaSASLPlainCredentialUpdateInput.update_forward_refs()
 KafkaSSLCredentialCreateInput.update_forward_refs()
 KafkaSSLCredentialSecretChangedInput.update_forward_refs()
 KafkaSSLCredentialUpdateInput.update_forward_refs()
+KafkaSaslSSLPlainCredentialCreateInput.update_forward_refs()
+KafkaSaslSSLPlainCredentialSecretChangedInput.update_forward_refs()
+KafkaSaslSSLPlainCredentialUpdateInput.update_forward_refs()
 KafkaSourceCreateInput.update_forward_refs()
 KafkaSourceUpdateInput.update_forward_refs()
 LocalIdentityProviderUpdateInput.update_forward_refs()
 MonotonicThresholdCreateInput.update_forward_refs()
 NotificationRuleCreateInput.update_forward_refs()
 NotificationRuleDeleteInput.update_forward_refs()
 NotificationRuleUpdateInput.update_forward_refs()
```

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/kafka_sasl_plain_credential_secret_changed.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/kafka_ssl_credential_secret_changed.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CredentialSecretChanged
 
 
-class KafkaSaslPlainCredentialSecretChanged(BaseModel):
-    kafka_sasl_plain_credential_secret_changed: "KafkaSaslPlainCredentialSecretChangedKafkaSaslPlainCredentialSecretChanged" = Field(
-        alias="kafkaSaslPlainCredentialSecretChanged"
+class KafkaSslCredentialSecretChanged(BaseModel):
+    kafka_ssl_credential_secret_changed: "KafkaSslCredentialSecretChangedKafkaSslCredentialSecretChanged" = Field(
+        alias="kafkaSslCredentialSecretChanged"
     )
 
 
-class KafkaSaslPlainCredentialSecretChangedKafkaSaslPlainCredentialSecretChanged(
+class KafkaSslCredentialSecretChangedKafkaSslCredentialSecretChanged(
     CredentialSecretChanged
 ):
     pass
 
 
-KafkaSaslPlainCredentialSecretChanged.update_forward_refs()
-KafkaSaslPlainCredentialSecretChangedKafkaSaslPlainCredentialSecretChanged.update_forward_refs()
+KafkaSslCredentialSecretChanged.update_forward_refs()
+KafkaSslCredentialSecretChangedKafkaSslCredentialSecretChanged.update_forward_refs()
```

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/list_credentials.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/list_credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                 "ListCredentialsCredentialsListCredential",
                 "ListCredentialsCredentialsListAwsCredential",
                 "ListCredentialsCredentialsListAwsAthenaCredential",
                 "ListCredentialsCredentialsListAwsRedshiftCredential",
                 "ListCredentialsCredentialsListPostgreSqlCredential",
                 "ListCredentialsCredentialsListSnowflakeCredential",
                 "ListCredentialsCredentialsListKafkaSSLCredential",
-                "ListCredentialsCredentialsListKafkaSASLPlainCredential",
+                "ListCredentialsCredentialsListKafkaSaslSSLPlainCredential",
             ],
             Field(discriminator="typename__"),
         ]
     ] = Field(alias="credentialsList")
 
 
 class ListCredentialsCredentialsListCredential(BaseModel):
@@ -134,26 +134,26 @@
 
 
 class ListCredentialsCredentialsListKafkaSSLCredentialConfig(BaseModel):
     bootstrap_servers: List[str] = Field(alias="bootstrapServers")
     ca_certificate: str = Field(alias="caCertificate")
 
 
-class ListCredentialsCredentialsListKafkaSASLPlainCredential(BaseModel):
-    typename__: Literal["KafkaSASLPlainCredential"] = Field(alias="__typename")
+class ListCredentialsCredentialsListKafkaSaslSSLPlainCredential(BaseModel):
+    typename__: Literal["KafkaSaslSSLPlainCredential"] = Field(alias="__typename")
     id: CredentialId
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
-    config: "ListCredentialsCredentialsListKafkaSASLPlainCredentialConfig"
+    config: "ListCredentialsCredentialsListKafkaSaslSSLPlainCredentialConfig"
 
 
-class ListCredentialsCredentialsListKafkaSASLPlainCredentialConfig(BaseModel):
+class ListCredentialsCredentialsListKafkaSaslSSLPlainCredentialConfig(BaseModel):
     bootstrap_servers: List[str] = Field(alias="bootstrapServers")
     username: str
 
 
 ListCredentials.update_forward_refs()
 ListCredentialsCredentialsListCredential.update_forward_refs()
 ListCredentialsCredentialsListAwsCredential.update_forward_refs()
@@ -164,9 +164,9 @@
 ListCredentialsCredentialsListAwsRedshiftCredentialConfig.update_forward_refs()
 ListCredentialsCredentialsListPostgreSqlCredential.update_forward_refs()
 ListCredentialsCredentialsListPostgreSqlCredentialConfig.update_forward_refs()
 ListCredentialsCredentialsListSnowflakeCredential.update_forward_refs()
 ListCredentialsCredentialsListSnowflakeCredentialConfig.update_forward_refs()
 ListCredentialsCredentialsListKafkaSSLCredential.update_forward_refs()
 ListCredentialsCredentialsListKafkaSSLCredentialConfig.update_forward_refs()
-ListCredentialsCredentialsListKafkaSASLPlainCredential.update_forward_refs()
-ListCredentialsCredentialsListKafkaSASLPlainCredentialConfig.update_forward_refs()
+ListCredentialsCredentialsListKafkaSaslSSLPlainCredential.update_forward_refs()
+ListCredentialsCredentialsListKafkaSaslSSLPlainCredentialConfig.update_forward_refs()
```

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/list_destinations.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/list_destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/list_sources.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/list_sources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/list_validators.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/list_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/list_windows.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/list_windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/scalars.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/scalars.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/snowflake_credential_secret_changed.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/snowflake_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/start_source.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/start_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/stop_source.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/stop_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_aws_kinesis_destination.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_kinesis_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_aws_redshift_credential.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_redshift_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_categorical_distribution_validator.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_categorical_distribution_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_gcp_big_query_destination.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_big_query_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_identity_provider_namespace.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_identity_provider_namespace.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_local_identity_provider.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_local_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_notification_rule_namespace.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_notification_rule_namespace.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_numeric_anomaly_validator.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_numeric_anomaly_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_numeric_distribution_validator.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_numeric_distribution_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_postgre_sql_credential.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_postgre_sql_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_relative_time_validator.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_relative_time_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_relative_volume_validator.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_relative_volume_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_saml_identity_provider.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_saml_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_segmentation_namespace.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_segmentation_namespace.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_snowflake_destination.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_snowflake_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.4/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/_diff.py` & `validio_sdk-0.6.4/validio_sdk/resource/_diff.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/_diff_util.py` & `validio_sdk-0.6.4/validio_sdk/resource/_diff_util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/_errors.py` & `validio_sdk-0.6.4/validio_sdk/resource/_errors.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/_field_selector.py` & `validio_sdk-0.6.4/validio_sdk/resource/_field_selector.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/_resource.py` & `validio_sdk-0.6.4/validio_sdk/resource/_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,25 @@
 
 # We need validio_sdk in scope due to eval.
 # ruff: noqa: F401
 import validio_sdk
 from validio_sdk.resource._diffable import Diffable
 from validio_sdk.resource._serde import (
     NODE_TYPE_FIELD_NAME,
+    ImportValue,
     _api_create_input_params,
     _api_update_input_params,
+    _import_resource_params,
+    _import_value_repr,
     without_skipped_internal_fields,
 )
 from validio_sdk.validio_client import ValidioAPIClient
 
 if TYPE_CHECKING:
+    from validio_sdk.code._import import ImportContext
     from validio_sdk.resource.channels import Channel
     from validio_sdk.resource.credentials import Credential
     from validio_sdk.resource.destinations import Destination
     from validio_sdk.resource.notification_rules import NotificationRule
     from validio_sdk.resource.segmentations import Segmentation
     from validio_sdk.resource.sources import Source
     from validio_sdk.resource.validators import Validator
@@ -58,14 +62,36 @@
     def fields() -> list[str]:
         return [
             f
             for f in list(inspect.signature(DiffContext).parameters)
             if f != "pending_validators_raw"
         ]
 
+    @staticmethod
+    def fields_topological_order() -> list[tuple[str, list[str]]]:
+        """Returns the fields but with their parent-child dependency encoded."""
+        fields: list[tuple[str, list[str]]] = [
+            # Channels need to come before sources because notification rules
+            # have references to sources.
+            ("channels", ["notification_rules"]),
+            ("credentials", ["sources", "destinations"]),
+            ("sources", ["windows", "segmentations", "validators"]),
+            ("destinations", []),
+            ("windows", []),
+            ("segmentations", []),
+            ("validators", []),
+            ("notification_rules", []),
+        ]
+        # Sanity check that this doesn't go out of sync
+        parents = {parent for (parent, _) in fields}
+        expected = set(DiffContext.fields())
+        if parents != expected:
+            raise Exception(f"DiffContext fields mismatch {parents} != {expected}")
+        return fields
+
 
 class ResourceID:
     """
     ResourceID represents the id of a resource.
 
     This value is potentially unknown until after the configuration has been fully
     provisioned. So it acts like a future/promise where it starts out as unknown
@@ -278,15 +304,15 @@
         method_name: str,
         response_field: str | None,
     ) -> Any | None:
         if len(response.errors) > 0:
             raise RuntimeError(
                 f"operation '{method_name}' failed for "
                 f"resource {self.__class__.__name__}(name={self.name}): "
-                f"{response.result.errors}"
+                f"{response.errors}"
             )
 
         if response_field is None:
             return None
 
         payload = response.__getattribute__(response_field)
         if payload is None:
@@ -314,14 +340,38 @@
     def _api_update_input(self, _namespace: str, _: "DiffContext") -> Any:
         """
         Similar to _api_create_input. Returns the graphql input(s) to
         update this resource.
         """
         return _api_update_input_params(self)
 
+    def _import_str(
+        self,
+        indent_level: int,
+        import_ctx: "ImportContext",
+        inits: list[tuple[str, Any, str | None]] | None = None,
+    ) -> str:
+        params = [("name", repr(self.name), None), *list(inits or [])]
+
+        for field, import_value in self._import_params().items():
+            params.append(
+                (
+                    field,
+                    _import_value_repr(
+                        import_value.value, indent_level + 1, import_ctx
+                    ),
+                    import_value.comment,
+                ),
+            )
+
+        return self._write_import_str(indent_level=indent_level, inits=params)
+
+    def _import_params(self) -> dict[str, ImportValue]:
+        return _import_resource_params(resource=self)
+
     @abstractmethod
     def resource_class_name(self) -> str:
         """What type of resource this is. (e.g. Window, Segmentation etc)."""
 
     @abstractmethod
     def _encode(self) -> dict[str, object]:
         """Encode the resource as json."""
```

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/_resource_graph.py` & `validio_sdk-0.6.4/validio_sdk/resource/_resource_graph.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/_serde.py` & `validio_sdk-0.6.4/validio_sdk/resource/_serde.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import inspect
-from typing import TYPE_CHECKING, Any
+from dataclasses import dataclass
+from enum import Enum
+from typing import TYPE_CHECKING, Any, Optional
 
 from camel_converter import to_snake
 
 # We need validio_sdk in scope due to eval.
 # ruff: noqa: F401
 import validio_sdk
 
 if TYPE_CHECKING:
+    from validio_sdk.code._import import ImportContext
+    from validio_sdk.resource._diffable import Diffable
     from validio_sdk.resource._resource import Resource
 
 """
 These are fields in a node of the graph that contains links to the resource graph
 itself or other internal fields that we don't need to serialise. We ignore these
 during encoding.
 """
@@ -171,7 +175,52 @@
                 for f in fields
                 if to_snake(f) not in skip_fields
             },
             **overrides,
             "id": resource._must_id(),
         }
     )
+
+
+@dataclass
+class ImportValue:
+    value: Any
+    comment: str | None = None
+
+
+def _import_resource_params(
+    resource: "Diffable",
+    skip_fields: set[str] | None = None,
+) -> dict[str, ImportValue]:
+    from validio_sdk.resource._resource import DiffContext
+
+    skip_fields = skip_fields or set({})
+    parent_resource_name_fields = {f"{f[:len(f)-1]}_name" for f in DiffContext.fields()}
+    parent_resource_name_fields.add("source_names")  # Notification rules have this
+    skip_fields = {*(skip_fields or set({})), *parent_resource_name_fields}
+    return {
+        field: ImportValue(getattr(resource, field))
+        for field in resource._all_fields()
+        if field not in skip_fields
+    }
+
+
+def _import_value_repr(
+    value: Any,
+    indent_level: int,
+    import_ctx: "ImportContext",
+) -> str:
+    from validio_sdk.resource._diffable import Diffable
+
+    if isinstance(value, Diffable):
+        value_repr = value._import_str(indent_level=indent_level, import_ctx=import_ctx)
+    elif isinstance(value, Enum):
+        value_repr = value.__str__()
+    elif isinstance(value, list):
+        values = ",".join(
+            [_import_value_repr(v, indent_level, import_ctx) for v in value]
+        )
+        value_repr = f"[{values}]"
+    else:
+        value_repr = repr(value)
+
+    return value_repr
```

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/_server_resources.py` & `validio_sdk-0.6.4/validio_sdk/resource/_server_resources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/_util.py` & `validio_sdk-0.6.4/validio_sdk/resource/_util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/channels.py` & `validio_sdk-0.6.4/validio_sdk/resource/channels.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/credentials.py` & `validio_sdk-0.6.4/validio_sdk/resource/credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from typing import TYPE_CHECKING, Any, Optional, cast
 
 from validio_sdk.resource._resource import Resource, ResourceGraph
 from validio_sdk.resource._resource_graph import RESOURCE_GRAPH
 from validio_sdk.resource._serde import (
     CONFIG_FIELD_NAME,
     NODE_TYPE_FIELD_NAME,
+    ImportValue,
     _encode_resource,
+    _import_resource_params,
     get_children_node,
     with_resource_graph_info,
 )
 
 if TYPE_CHECKING:
     from validio_sdk.resource._diff import DiffContext
 
@@ -103,14 +105,27 @@
             r = cast(Any, resource_cls)._decode(ctx, cls, value, credential)
             resources[resource_name] = r
             ctx.__getattribute__(resource_module)[resource_name] = r
 
         if len(resources) > 0:
             credential._children[resource_cls.__name__] = resources
 
+    def _import_params(self) -> dict[str, ImportValue]:
+        secret_fields = {
+            field: ImportValue(value="UNSET", comment="FIXME: Add secret value")
+            for field in (self._secret_fields() or set({}))
+        }
+        return {
+            **_import_resource_params(
+                resource=self,
+                skip_fields=self._secret_fields(),
+            ),
+            **secret_fields,
+        }
+
 
 class DemoCredential(Credential):
     """A demo credential resource."""
 
     def _immutable_fields(self) -> set[str]:
         return set({})
```

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/destinations.py` & `validio_sdk-0.6.4/validio_sdk/resource/destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/filters.py` & `validio_sdk-0.6.4/validio_sdk/resource/filters.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/notification_rules.py` & `validio_sdk-0.6.4/validio_sdk/resource/notification_rules.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/segmentations.py` & `validio_sdk-0.6.4/validio_sdk/resource/segmentations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/sources.py` & `validio_sdk-0.6.4/validio_sdk/resource/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Sources."""
 import inspect
 import json
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, cast
 
 from camel_converter import to_snake
 
 # We need validio_sdk in scope due to eval.
 # ruff: noqa: F401
 import validio_sdk
 from validio_sdk.graphql_client import CsvParserInput
 from validio_sdk.resource._diffable import Diffable
 from validio_sdk.resource._resource import Resource
 from validio_sdk.resource._serde import (
     CONFIG_FIELD_NAME,
     NODE_TYPE_FIELD_NAME,
+    ImportValue,
     _api_create_input_params,
     _api_update_input_params,
     _encode_resource,
+    _import_resource_params,
     get_children_node,
 )
 from validio_sdk.resource.credentials import (
     AwsCredential,
     AwsRedshiftCredential,
     Credential,
     DemoCredential,
@@ -189,14 +191,20 @@
         )
         for name, value in validators_obj.items():
             ctx.pending_validators_raw[name] = (
                 eval(f"validio_sdk.resource.validators.{value[NODE_TYPE_FIELD_NAME]}"),
                 value,
             )
 
+    def _import_params(self) -> dict[str, ImportValue]:
+        return _import_resource_params(
+            resource=self,
+            skip_fields={"jtd_schema"},
+        )
+
     async def _api_infer_schema(self, credential: Credential, client: ValidioAPIClient):
         # e.g GcpBigQuerySource
         class_name = self.__class__.__name__
         # => GcpBigQuery
         source_type_name = class_name[: -len("Source")]
         # => gcp_big_query
         resource_snake_case = to_snake(source_type_name)
```

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/tests/test__diff.py` & `validio_sdk-0.6.4/validio_sdk/resource/tests/test__diff.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/tests/test__field_selector.py` & `validio_sdk-0.6.4/validio_sdk/resource/tests/test__field_selector.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/tests/test__resource.py` & `validio_sdk-0.6.4/validio_sdk/resource/tests/test__resource.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/thresholds.py` & `validio_sdk-0.6.4/validio_sdk/resource/thresholds.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/validators.py` & `validio_sdk-0.6.4/validio_sdk/resource/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from validio_sdk.resource.sources import Source
 from validio_sdk.resource.thresholds import DynamicThreshold, Threshold
 from validio_sdk.resource.windows import TumblingWindow, Window
 from validio_sdk.scalars import JsonFilterExpression, JsonPointer
 from validio_sdk.validio_client import ValidioAPIClient
 
 if TYPE_CHECKING:
+    from validio_sdk.code._import import ImportContext
     from validio_sdk.resource._diff import DiffContext
 
 
 class Reference(Diffable):
     """
     Represents configuration for reference validators.
 
@@ -83,14 +84,30 @@
 
     def _mutable_fields(self) -> set[str]:
         return {"history", "offset"}
 
     def _nested_objects(self) -> dict[str, Diffable | None]:
         return {"filter": self.filter}
 
+    def _import_str(
+        self,
+        indent_level: int,
+        import_ctx: "ImportContext",
+        inits: list[tuple[str, Any, str | None]] | None = None,
+    ) -> str:
+        inits = list(inits or [])
+        source = import_ctx.get_variable(Source, self.source_name)
+        window = import_ctx.get_variable(Window, self.window_name)
+        inits = [*inits, ("source", source, None), ("window", window, None)]
+        return super()._import_str(
+            indent_level=indent_level,
+            import_ctx=import_ctx,
+            inits=inits,
+        )
+
     def _reference_source_config_create_input(
         self, ctx: "DiffContext"
     ) -> ReferenceSourceConfigCreateInput:
         source_id = ctx.sources[self.source_name]._must_id()
         window_id = ctx.windows[self.window_name]._must_id()
         return ReferenceSourceConfigCreateInput(
             # type: ignore[call-arg]
@@ -291,19 +308,22 @@
                 f"invalid {self.__class__.__name__} '{self.name}': "
                 f"field selector not allowed in {position}"
             )
 
         self._validate_reference_filter_no_field_selector()
 
     def _nested_objects(self) -> dict[str, Diffable | None]:
-        return {
+        objects: dict[str, Diffable | None] = {
             "filter": self.filter,
-            "reference": self.reference,
             "threshold": self.threshold,
         }
+        if self.reference:
+            objects["reference"] = self.reference
+
+        return objects
 
     def _immutable_fields(self) -> set[str]:
         fields = {
             "window_name",
             "segmentation_name",
         }
```

### Comparing `validio_sdk-0.6.3/validio_sdk/resource/windows.py` & `validio_sdk-0.6.4/validio_sdk/resource/windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/scalars.py` & `validio_sdk-0.6.4/validio_sdk/scalars.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/util.py` & `validio_sdk-0.6.4/validio_sdk/util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/validio_sdk/validio_client.py` & `validio_sdk-0.6.4/validio_sdk/validio_client.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.3/PKG-INFO` & `validio_sdk-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validio-sdk
-Version: 0.6.3
+Version: 0.6.4
 Summary: SDK to interact with the Validio platform
 Home-page: https://validio.io/
 License: Apache-2.0
 Author: Validio
 Author-email: support@validio.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

