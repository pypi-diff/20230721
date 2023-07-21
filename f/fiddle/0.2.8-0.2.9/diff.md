# Comparing `tmp/fiddle-0.2.8.tar.gz` & `tmp/fiddle-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddle-0.2.8.tar", last modified: Mon Jul 17 18:56:16 2023, max compression
+gzip compressed data, was "fiddle-0.2.9.tar", last modified: Fri Jul 21 19:08:24 2023, max compression
```

## Comparing `fiddle-0.2.8.tar` & `fiddle-0.2.9.tar`

### file list

```diff
@@ -1,212 +1,217 @@
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11357 2022-02-19 00:33:27.000000 fiddle-0.2.8/LICENSE
--rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-07-17 18:56:16.484165 fiddle-0.2.8/PKG-INFO
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      603 2023-07-17 18:55:59.000000 fiddle-0.2.8/README.md
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.464165 fiddle-0.2.8/fiddle/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1610 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.472165 fiddle-0.2.8/fiddle/_src/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.472165 fiddle-0.2.8/fiddle/_src/absl_flags/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      907 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/absl_flags/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    21439 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/absl_flags/flags.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1021 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/absl_flags/sample_module_for_flags_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16567 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/arg_factory.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15484 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/arg_factory_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5939 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/building.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2483 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/building_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.472165 fiddle-0.2.8/fiddle/_src/codegen/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.476165 fiddle-0.2.8/fiddle/_src/codegen/auto_config/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7956 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/code_ir.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2506 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/code_ir_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5371 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/complex_to_variables.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4327 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/complex_to_variables_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8540 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/experimental_top_level_api.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9988 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2445 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/get_history_comments.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2187 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/get_history_comments_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1605 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/init_task.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1181 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/init_task_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5242 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_printer.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3942 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_printer_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7921 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_to_cst.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6294 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_to_cst_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8328 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/make_symbolic_references.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7507 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6743 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/naming.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8402 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/naming_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4183 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/parents_first_traversal.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2322 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4027 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/shared_to_variables.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3586 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/shared_to_variables_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2047 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/split_arg_factories.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2335 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/split_arg_factories_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11043 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/sub_fixture.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3467 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/sub_fixture_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5759 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/test_fixtures.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    17419 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/codegen_diff.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1951 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/formatting_utilities.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8776 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/import_manager.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5074 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/import_manager_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11220 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/legacy_codegen.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9134 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/legacy_codegen_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4206 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/mini_ast.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3471 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/namespace.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2204 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/namespace_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5207 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/new_codegen.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3653 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/new_codegen_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4537 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/newcg_symbolic_references.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6544 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/newcg_symbolic_references_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15928 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/py_val_to_cst_converter.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6189 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/py_val_to_cst_converter_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3500 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/special_value_codegen.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.476165 fiddle-0.2.8/fiddle/_src/codegen/test_submodule/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/test_submodule/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      810 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/test_submodule/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    51137 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    53885 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    27540 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/daglish.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5349 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/daglish_extensions.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3241 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/daglish_extensions_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    20247 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/daglish_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    41201 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/diffing.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    45929 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/diffing_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/_src/experimental/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    42854 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/auto_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5668 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/auto_config_policy.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    43562 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/auto_config_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/_src/experimental/autobuilders/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/autobuilders/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11256 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/autobuilders/autobuilders.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6512 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/autobuilders/autobuilders_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      922 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3585 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/configurator.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12374 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/daglish_legacy.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16195 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/daglish_legacy_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7228 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/dataclasses.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14396 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/dataclasses_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1173 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/dict_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2706 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/dict_config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1264 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/namespace_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2678 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/namespace_config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    30108 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/serialization.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3228 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/transform.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4743 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/transform_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11539 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/visualize.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2338 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/with_tags.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2169 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/with_tags_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2804 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/yaml_serialization.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4422 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/yaml_serialization_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/_src/extensions/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1324 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/flax_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5458 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/jax.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1408 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/seqio.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1479 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/seqio_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3433 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/tf.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4583 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/tf_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1633 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/field_metadata.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    36979 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/graphviz.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2133 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/graphviz_custom_object.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9437 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/history.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5216 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/history_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2380 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/materialize.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1760 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/materialize_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3459 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/module_reflection.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2768 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/module_reflection_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1420 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/module_reflection_test_module.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1795 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/mutate_buildable.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1615 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/mutate_buildable_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12318 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/printing.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14648 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/printing_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2879 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/reraised_exception.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2235 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/reraised_exception_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    10408 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/selectors.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11289 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/selectors_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4274 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/signatures.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6539 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/signatures_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1011 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/signatures_test_helper.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4267 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/tag_type.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7368 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/tagging.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14083 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/tagging_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1275 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/tagging_test_module.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/_src/testing/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5543 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/autotest.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/_src/testing/example/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/example/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1871 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/example/demo_configs.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2533 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/example/fake_encoder_decoder.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1235 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/example/person_friend_toy.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5419 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/nested_values.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3155 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/nested_values_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9562 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9805 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/test_util_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/absl_flags/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      967 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/absl_flags/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/absl_flags/example/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/absl_flags/example/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1342 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/absl_flags/example/business_logic.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3451 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/absl_flags/example/configs.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1444 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/absl_flags/example/example.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      906 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/absl_flags/example/tags.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3528 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/arg_factory.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      792 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/building.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/codegen/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/codegen/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/codegen/auto_config/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/codegen/auto_config/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1828 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/codegen/auto_config/experimental_top_level_api.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1076 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/codegen/codegen.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/codegen/codegen_diff.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1296 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/codegen/py_val_to_cst_converter.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1011 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1002 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2119 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/daglish.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1705 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/diffing.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/examples/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/examples/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/examples/colabs/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/examples/colabs/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/experimental/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1658 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/auto_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1210 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/auto_config_policy.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/experimental/autobuilders/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/autobuilders/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1025 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/configurator.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1523 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/dataclasses.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/dict_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      781 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/namespace_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1910 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/serialization.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      860 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/transform.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1327 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/visualize.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1043 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/yaml_serialization.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/extensions/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/extensions/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      824 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/extensions/jax.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      868 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/extensions/seqio.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      840 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/extensions/tf.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      942 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/graphviz.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1184 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/history.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      812 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/printing.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1049 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/selectors.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/signatures.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      847 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/tag_type.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2682 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/tagging.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/testing/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/testing/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1300 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/testing/autotest.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      762 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/testing/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      676 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/version.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.468165 fiddle-0.2.8/fiddle.egg-info/
--rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-07-17 18:56:16.000000 fiddle-0.2.8/fiddle.egg-info/PKG-INFO
--rw-r-----   0 dhr      (201437) primarygroup (89939)     6948 2023-07-17 18:56:16.000000 fiddle-0.2.8/fiddle.egg-info/SOURCES.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)        1 2023-07-17 18:56:16.000000 fiddle-0.2.8/fiddle.egg-info/dependency_links.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)      151 2023-07-17 18:56:16.000000 fiddle-0.2.8/fiddle.egg-info/requires.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)        7 2023-07-17 18:56:16.000000 fiddle-0.2.8/fiddle.egg-info/top_level.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)       38 2023-07-17 18:56:16.484165 fiddle-0.2.8/setup.cfg
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3554 2023-07-17 18:56:00.000000 fiddle-0.2.8/setup.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11357 2022-02-19 00:33:27.000000 fiddle-0.2.9/LICENSE
+-rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-07-21 19:08:24.555863 fiddle-0.2.9/PKG-INFO
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      603 2023-07-21 19:08:10.000000 fiddle-0.2.9/README.md
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.539863 fiddle-0.2.9/fiddle/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1610 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.543863 fiddle-0.2.9/fiddle/_src/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.543863 fiddle-0.2.9/fiddle/_src/absl_flags/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      907 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/absl_flags/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1047 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/absl_flags/flags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15534 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/absl_flags/legacy_flags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1021 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/absl_flags/sample_module_for_flags_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7150 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/absl_flags/utils.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16567 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/arg_factory.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15484 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/arg_factory_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5939 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/building.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2483 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/building_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.543863 fiddle-0.2.9/fiddle/_src/codegen/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.547863 fiddle-0.2.9/fiddle/_src/codegen/auto_config/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7956 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/code_ir.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2506 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/code_ir_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5371 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/complex_to_variables.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4327 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/complex_to_variables_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8540 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/experimental_top_level_api.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11095 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2445 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/get_history_comments.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2187 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/get_history_comments_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1605 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/init_task.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1181 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/init_task_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5265 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_printer.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3942 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_printer_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7921 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_to_cst.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6294 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_to_cst_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8328 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/make_symbolic_references.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7507 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6640 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/naming.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8476 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/naming_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4183 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/parents_first_traversal.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2765 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4027 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/shared_to_variables.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3586 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/shared_to_variables_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2047 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/split_arg_factories.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2335 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/split_arg_factories_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    17405 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/sub_fixture.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11681 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/sub_fixture_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5759 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/test_fixtures.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    17419 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/codegen_diff.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1951 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/formatting_utilities.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8776 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/import_manager.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5074 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/import_manager_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11220 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/legacy_codegen.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9134 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/legacy_codegen_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4206 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/mini_ast.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3471 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/namespace.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2204 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/namespace_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5207 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/new_codegen.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3653 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/new_codegen_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4537 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/newcg_symbolic_references.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6544 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/newcg_symbolic_references_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15928 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/py_val_to_cst_converter.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6189 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/py_val_to_cst_converter_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3500 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/special_value_codegen.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.547863 fiddle-0.2.9/fiddle/_src/codegen/test_submodule/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/test_submodule/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      810 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/test_submodule/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    42592 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    53885 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    27540 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/daglish.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5349 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/daglish_extensions.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3241 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/daglish_extensions_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    20247 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/daglish_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    41201 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/diffing.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    45929 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/diffing_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.551863 fiddle-0.2.9/fiddle/_src/experimental/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    43693 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/auto_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5668 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/auto_config_policy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    44111 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/auto_config_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.551863 fiddle-0.2.9/fiddle/_src/experimental/autobuilders/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/autobuilders/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11256 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/autobuilders/autobuilders.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6512 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/autobuilders/autobuilders_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      922 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3585 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/configurator.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12374 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/experimental/daglish_legacy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16195 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/daglish_legacy_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3167 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/experimental/dataclasses.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2917 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/dataclasses_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1173 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/experimental/dict_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2706 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/dict_config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7286 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/lazy_imports.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9119 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/lazy_imports_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      909 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/lazy_imports_test_example.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1264 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/namespace_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2678 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/namespace_config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    30877 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/experimental/serialization.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3228 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/experimental/transform.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4743 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/transform_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11539 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/visualize.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2338 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/with_tags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2169 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/with_tags_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2804 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/yaml_serialization.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4422 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/yaml_serialization_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.551863 fiddle-0.2.9/fiddle/_src/extensions/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1324 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/flax_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5458 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/jax.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1408 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/seqio.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1479 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/seqio_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3433 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/tf.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4583 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/tf_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    36979 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/graphviz.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2133 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/graphviz_custom_object.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9437 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/history.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5216 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/history_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2380 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/materialize.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1760 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/materialize_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3459 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/module_reflection.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2768 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/module_reflection_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1420 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/module_reflection_test_module.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1795 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/mutate_buildable.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1615 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/mutate_buildable_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12318 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/printing.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14648 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/printing_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2879 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/reraised_exception.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2235 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/reraised_exception_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    10408 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/selectors.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11289 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/selectors_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4274 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/signatures.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6539 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/signatures_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1011 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/signatures_test_helper.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4267 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/tag_type.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7368 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/tagging.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    13570 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/tagging_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1275 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/tagging_test_module.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.551863 fiddle-0.2.9/fiddle/_src/testing/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5543 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/autotest.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.551863 fiddle-0.2.9/fiddle/_src/testing/example/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/example/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2463 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/example/demo_configs.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2533 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/example/fake_encoder_decoder.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1235 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/example/person_friend_toy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5419 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/nested_values.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3155 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/nested_values_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9562 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/testing/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9805 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/test_util_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.551863 fiddle-0.2.9/fiddle/absl_flags/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      967 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/absl_flags/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/absl_flags/example/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/absl_flags/example/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1342 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/absl_flags/example/business_logic.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3451 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/absl_flags/example/configs.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1444 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/absl_flags/example/example.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      906 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/absl_flags/example/tags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3528 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/arg_factory.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      792 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/building.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/codegen/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/codegen/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/codegen/auto_config/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/codegen/auto_config/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1828 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/codegen/auto_config/experimental_top_level_api.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1076 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/codegen/codegen.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/codegen/codegen_diff.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1296 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/codegen/py_val_to_cst_converter.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1011 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1002 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2119 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/daglish.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1705 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/diffing.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/examples/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/examples/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/examples/colabs/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/examples/colabs/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/experimental/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1719 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/auto_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1210 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/experimental/auto_config_policy.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/experimental/autobuilders/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/autobuilders/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1025 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/configurator.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      854 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/dataclasses.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/dict_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      781 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/lazy_imports.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      781 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/namespace_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1910 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/serialization.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      860 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/transform.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1327 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/visualize.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1043 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/yaml_serialization.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/extensions/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/extensions/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      824 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/extensions/jax.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      868 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/extensions/seqio.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      840 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/extensions/tf.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      942 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/graphviz.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1184 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/history.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      812 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/printing.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1049 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/selectors.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/signatures.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      847 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/tag_type.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2682 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/tagging.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/testing/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/testing/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1300 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/testing/autotest.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      762 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/testing/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      676 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/version.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.539863 fiddle-0.2.9/fiddle.egg-info/
+-rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-07-21 19:08:24.000000 fiddle-0.2.9/fiddle.egg-info/PKG-INFO
+-rw-r-----   0 dhr      (201437) primarygroup (89939)     7166 2023-07-21 19:08:24.000000 fiddle-0.2.9/fiddle.egg-info/SOURCES.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)        1 2023-07-21 19:08:24.000000 fiddle-0.2.9/fiddle.egg-info/dependency_links.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)      151 2023-07-21 19:08:24.000000 fiddle-0.2.9/fiddle.egg-info/requires.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)        7 2023-07-21 19:08:24.000000 fiddle-0.2.9/fiddle.egg-info/top_level.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)       38 2023-07-21 19:08:24.555863 fiddle-0.2.9/setup.cfg
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3554 2023-07-21 19:08:11.000000 fiddle-0.2.9/setup.py
```

### Comparing `fiddle-0.2.8/LICENSE` & `fiddle-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/PKG-INFO` & `fiddle-0.2.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddle
-Version: 0.2.8
+Version: 0.2.9
 Summary: Fiddle: A Python-first configuration library
 Home-page: https://github.com/google/fiddle
 Author: The Fiddle Team
 Author-email: noreply@google.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/google/fiddle/docs
 Project-URL: Bug Reports, https://github.com/google/fiddle/issues
```

### Comparing `fiddle-0.2.8/README.md` & `fiddle-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/__init__.py` & `fiddle-0.2.9/fiddle/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/__init__.py` & `fiddle-0.2.9/fiddle/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/absl_flags/__init__.py` & `fiddle-0.2.9/fiddle/_src/absl_flags/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/absl_flags/flags.py` & `fiddle-0.2.9/fiddle/_src/absl_flags/legacy_flags.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,21 +9,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Utilities to use command line flags with Fiddle Buildables.
+"""Legacy API to use command line flags with Fiddle Buildables.
 
 While it's generally better to check in the full configuration into a source-
 control system, there are some instances (e.g. hyperparameter sweeps) where it's
 most effective to set initialization parameters (hyperparameters) from command
 line flags. This library exposes functions you can call within your program.
 
+NOTE: The flags aren't applied in the order they are passed in on the command
+  line. The order followed is:
+  - all fiddlers are applied first, followed by
+  - all tags, followed by
+  - all overrides.
+
 ## Quickstart
 
 > Note: although different bits of functionality are designed to be usable
 > piecemeal, this is the fastest way to get all flag-integrated features.
 
 First, some definitions:
 
@@ -104,36 +110,32 @@
 
 ## Acknowledgements
 
 This implementation has drawn inspiration from multiple sources, including
 [T5X](https://github.com/google-research/t5x), among others. Thank you!
 """
 
-import ast
-import dataclasses
-import enum
-import importlib
 import inspect
 import re
 import sys
 import textwrap
 import typing
-from typing import Any, Dict, List, Optional, Sequence, Tuple
+from typing import Any, List, Optional, Sequence
 
 from absl import app
 from absl import flags
 from absl import logging
 from etils import epath
 from fiddle import printing
 from fiddle import selectors
 from fiddle._src import config
 from fiddle._src import daglish
-from fiddle._src import daglish_extensions
 from fiddle._src import module_reflection
 from fiddle._src import tagging
+from fiddle._src.absl_flags import utils
 from fiddle._src.experimental import auto_config
 from fiddle._src.experimental import serialization
 
 
 _FDL_CONFIG = flags.DEFINE_string(
     'fdl_config',
     default=None,
@@ -167,214 +169,39 @@
     'information on any loaded configuration) and exit.')
 
 
 def _print_stderr(*args, **kwargs):
   print(*args, **kwargs, file=sys.stderr)
 
 
-def _parse_path(path: str) -> daglish.Path:
-  """Parses a path into a list of either attributes or index lookups."""
-  if not path.startswith('[') and not path.startswith('.'):
-    path = f'.{path}'  # Add a leading `.` to make parsing work properly.
-
-  return daglish_extensions.parse_path(path)
-
-
-class _ImportDottedNameDebugContext(enum.Enum):
-  """Context of importing a sumbol, for error messages."""
-
-  BASE_CONFIG = 1
-  FIDDLER = 2
-
-  def error_prefix(self, name: str) -> str:
-    if self == _ImportDottedNameDebugContext.BASE_CONFIG:
-      return f'Could not init a buildable from {name!r}'
-    assert self == _ImportDottedNameDebugContext.FIDDLER
-    return f'Could not load fiddler {name!r}'
-
-
-def _import_dotted_name(name: str, mode: _ImportDottedNameDebugContext) -> Any:
-  """Returns the Python object with the given dotted name.
-
-  Args:
-    name: The dotted name of a Python object, including the module name.
-    mode: Whether we're looking for a base config function or a fiddler.
-
-  Returns:
-    The named value.
-
-  Raises:
-    ValueError: If `name` is not a dotted name.
-    ModuleNotFoundError: If no dotted prefix of `name` can be imported.
-    AttributeError: If the imported module does not contain a value with
-      the indicated name.
-  """
-  name_pieces = name.split('.')
-  if len(name_pieces) < 2:
-    raise ValueError(
-        f'{mode.error_prefix(name)}: Expected a dotted name including the '
-        'module name.'
-    )
-
-  # We don't know where the module ends and the name begins; so we need to
-  # try different split points.  Longer module names take precedence.
-  for i in range(len(name_pieces) - 1, 0, -1):
-    try:
-      value = importlib.import_module('.'.join(name_pieces[:i]))
-      for j, name_piece in enumerate(name_pieces[i:]):
-        try:
-          value = getattr(value, name_piece)  # Can raise AttributeError.
-        except AttributeError:
-          available_names = ', '.join(
-              repr(n) for n in dir(value) if not n.startswith('_')
-          )
-          module_name = '.'.join(name_pieces[: i + j])
-          failing_name = name_pieces[i + j]
-          raise ValueError(
-              f'{mode.error_prefix(name)}: module {module_name!r} has no '
-              f'attribute {failing_name!r}; available names: {available_names}'
-          ) from None
-      return value
-    except ModuleNotFoundError:
-      if i == 1:  # Final iteration through the loop.
-        raise
-
-  # The following line should be unreachable -- the "if i == 1: raise" above
-  # should have raised an exception before we exited the loop.
-  raise ModuleNotFoundError(f'No module named {name_pieces[0]!r}')
-
-
-def parse_value(value: str, path: str) -> Any:
-  """Parses a string `value` (e.g. from the command line) to a Python type."""
-
-  # Apply a few rules that are unambiguous and would otherwise just cause
-  # spurious failures (e.g. `--fdl_set=use_cached=false`).
-  if value.lower() == 'false':
-    return False
-  elif value.lower() == 'true':
-    return True
-
-  try:
-    return ast.literal_eval(value)
-  except Exception as e:
-    raise ValueError(
-        f'Could not parse literal value "{value}" while trying to set '
-        f'"{path}". Does a string need to be quoted? For example, you might '
-        f"want to pass --fdl_set={path}='{value}' instead of "
-        f'--fdl_set={path}={value}.'
-    ) from e
-
-
-@dataclasses.dataclass(frozen=True)
-class CallExpression:
-  """Parsed components of a call expression (or bare function name).
-
-  Examples:
-
-  >>> CallExpression.parse("fn('foo', False, x=[1, 2])")
-  CallExpression(func_name='fn', args=('foo', False'), kwargs={'x': [1, 2]})
-  >>> CallExpression.parse("fn")  # Bare function name: empty args/kwargs.
-  CallExpression(func_name='fn', args=()), kwargs={})
-
-  Attributes:
-    func_name: The name fo the function that should be called.
-    args: Parsed values of positional arguments for the function.
-    kwargs: Parsed values of keyword arguments for the function.
-  """
-
-  func_name: str
-  args: Optional[Tuple[Any, ...]]
-  kwargs: Optional[Dict[str, Any]]
-
-  _PARSE_RE = re.compile(r'(?P<func_name>[\w\.]+)(?:\((?P<args>.*)\))?')
-
-  @classmethod
-  def parse(cls, value: str) -> 'CallExpression':
-    """Returns a CallExpression parsed from a string.
-
-    Args:
-      value: A string containing positional and keyword arguments for a
-        function.  Must consist of an open paren followed by comma-separated
-        argument values followed by a close paren.  Argument values must be
-        literal constants (i.e., must be parsable with `ast.literal_eval`).
-        var-positional and var-keyword arguments are not supported.
-
-    Raises:
-      SyntaxError: If `value` is not a simple call expression with literal
-        arguments.
-    """
-    m = re.fullmatch(cls._PARSE_RE, value)
-    if m is None:
-      raise SyntaxError(
-          f'Expected a function name or call expression; got: {value!r}'
-      )
-    if m.group('args') is None:  # Bare function name
-      return CallExpression(m.group('func_name'), (), {})
-
-    node = ast.parse(value)  # Can raise SyntaxError.
-    if not (
-        isinstance(node, ast.Module)
-        and len(node.body) == 1
-        and isinstance(node.body[0], ast.Expr)
-        and isinstance(node.body[0].value, ast.Call)
-    ):
-      raise SyntaxError(
-          f'Expected a function name or call expression; got: {value!r}'
-      )
-    call_node = node.body[0].value
-    args = []
-    for arg in call_node.args:
-      if isinstance(arg, ast.Starred):
-        raise SyntaxError('*args is not supported.')
-      try:
-        args.append(ast.literal_eval(arg))
-      except ValueError as exc:
-        raise SyntaxError(
-            'Expected arguments to be simple literals; got '
-            f'{ast.unparse(arg)!r} (while parsing {value!r})'
-        ) from exc
-    kwargs = {}
-    for kwarg in call_node.keywords:
-      if kwarg.arg is None:
-        raise SyntaxError('**kwargs is not supported.')
-      try:
-        kwargs[kwarg.arg] = ast.literal_eval(kwarg.value)
-      except ValueError as exc:
-        raise SyntaxError(
-            'Expected arguments to be simple literals; got '
-            f'{ast.unparse(kwarg.value)!r} (while parsing {value!r})'
-        ) from exc
-    return CallExpression(m.group('func_name'), tuple(args), kwargs)
-
-
 def apply_overrides_to(cfg: config.Buildable):
   """Applies all command line flags to `cfg`."""
   for flag in _FDL_SET.value:
     path, value = flag.split('=', maxsplit=1)
-    *parents, last = _parse_path(path)
+    *parents, last = utils.parse_path(path)
     walk = typing.cast(Any, cfg)
     try:
       for parent in parents:
         walk = parent.follow(walk)
     except Exception as e:
       raise ValueError(f'Invalid path "{path}".') from e
 
-    literal_value = parse_value(value=value, path=path)
+    literal_value = utils.parse_value(value=value, path=path)
     try:
       if isinstance(last, daglish.Attr):
         setattr(walk, last.name, literal_value)
       elif isinstance(last, daglish.Key):
         walk[last.key] = literal_value
       else:
         raise ValueError(f'Unexpected path element {last}.')
     except Exception as e:
       raise ValueError(f'Could not set "{path}" to "{value}".') from e
 
 
-def _rewrite_fdl_args(args: Sequence[str]) -> List[str]:
+def rewrite_fdl_args(args: Sequence[str]) -> List[str]:
   """Rewrites short-form Fiddle flags.
 
   There are two main rewrites:
 
     * `--fdl.NAME=VALUE` to `--fdl_set=NAME = VALUE`.
     * `--fdl_tag.NAME=VALUE` to `--fdl_tags_set=NAME = VALUE`.
 
@@ -414,15 +241,15 @@
 
   Args:
     args: All command line arguments.
 
   Returns:
     Whatever `absl.app.parse_flags_with_usage` returns. Sorry!
   """
-  return app.parse_flags_with_usage(_rewrite_fdl_args(args))
+  return app.parse_flags_with_usage(rewrite_fdl_args(args))
 
 
 def set_tags(cfg: config.Buildable):
   """Sets tags based on their name, from CLI flags."""
   all_tags = tagging.list_tags(cfg, add_superclasses=True)
   for flag in _FDL_TAGS_SET.value:
     name, value = flag.split('=', maxsplit=1)
@@ -438,32 +265,32 @@
     elif len(matching_tags) > 1:
       raise EnvironmentError(
           f'There were multiple tags with name {name!r}; perhaps some module '
           'reloading weirdness is going on? This should be very rare. Please '
           'make sure that you are not dynamically creating subclasses of '
           '`fdl.Tag` and using 2 instances with the same module and name '
           'in the configuration.')
-    selectors.select(
-        cfg, tag=matching_tags[0]).replace(
-            value=parse_value(value=value, path=str(matching_tags[0])))
+    selectors.select(cfg, tag=matching_tags[0]).replace(
+        value=utils.parse_value(value=value, path=str(matching_tags[0]))
+    )
 
 
 def apply_fiddlers_to(cfg: config.Buildable,
                       source_module: Any,
                       allow_imports=False):
   """Applies fiddlers to `cfg`."""
   for fiddler_value in _FIDDLER.value:
-    call_expr = CallExpression.parse(fiddler_value)
+    call_expr = utils.CallExpression.parse(fiddler_value)
     fiddler_name = call_expr.func_name
     if hasattr(source_module, fiddler_name):
       fiddler = getattr(source_module, fiddler_name)
     elif allow_imports:
       try:
-        fiddler = _import_dotted_name(
-            fiddler_name, mode=_ImportDottedNameDebugContext.FIDDLER
+        fiddler = utils.import_dotted_name(
+            fiddler_name, mode=utils.ImportDottedNameDebugContext.FIDDLER
         )
       except ModuleNotFoundError as e:
         raise ValueError(f'Could not load fiddler {fiddler_name!r}: {e}') from e
     else:
       available_fiddlers = ', '.join(
           module_reflection.find_fiddler_like_things(source_module))
       raise ValueError(
@@ -515,14 +342,20 @@
 def create_buildable_from_flags(
     module: Optional[Any],
     allow_imports=False,
     pyref_policy: Optional[serialization.PyrefPolicy] = None,
 ) -> config.Buildable:
   """Returns a fdl.Buildable based on standardized flags.
 
+  NOTE: the flags aren't applied in the order they are passed in on the command
+  line. The order followed is:
+  - all fiddlers are applied first, followed by
+  - all tags, followed by
+  - all overrides.
+
   Args:
     module: A common namespace to use as the basis for finding configs and
       fiddlers. May be `None`; if `None`, only fully qualified Fiddler imports
       will be used (or alternatively a base configuration can be specified using
       the `--fdl_config_file` flag.)
     allow_imports: If true, then fully qualified dotted names may be used to
       specify configs or fiddlers that should be automatically imported.
@@ -549,22 +382,23 @@
         '`{flag}` flag unless `allow_imports` is `True`.')
     if _FDL_CONFIG.value:
       raise ValueError(err_msg.format(flag='--fdl_config'))
     if _FIDDLER.value:
       raise ValueError(err_msg.format(flag='--fiddler'))
 
   if _FDL_CONFIG.value:
-    call_expr = CallExpression.parse(_FDL_CONFIG.value)
+    call_expr = utils.CallExpression.parse(_FDL_CONFIG.value)
     base_name = call_expr.func_name
     if hasattr(module, base_name):
       base_fn = getattr(module, base_name)
     elif allow_imports:
       try:
-        base_fn = _import_dotted_name(
-            base_name, mode=_ImportDottedNameDebugContext.BASE_CONFIG
+        base_fn = utils.import_dotted_name(
+            base_name,
+            mode=utils.ImportDottedNameDebugContext.BASE_CONFIG,
         )
       except ModuleNotFoundError as e:
         raise ValueError(
             f'Could not init a buildable from {base_name!r}: {e}') from e
     else:
       available_names = module_reflection.find_base_config_like_things(module)
       raise ValueError(f'Could not init a buildable from {base_name!r}; '
```

### Comparing `fiddle-0.2.8/fiddle/_src/absl_flags/sample_module_for_flags_test.py` & `fiddle-0.2.9/fiddle/_src/absl_flags/sample_module_for_flags_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/arg_factory.py` & `fiddle-0.2.9/fiddle/_src/arg_factory.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/arg_factory_test.py` & `fiddle-0.2.9/fiddle/_src/arg_factory_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/building.py` & `fiddle-0.2.9/fiddle/_src/building.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/building_test.py` & `fiddle-0.2.9/fiddle/_src/building_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/__init__.py` & `fiddle-0.2.9/fiddle/_src/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/__init__.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/code_ir.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/code_ir.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/code_ir_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/code_ir_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/complex_to_variables.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/complex_to_variables.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/complex_to_variables_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/complex_to_variables_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/experimental_top_level_api.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/experimental_top_level_api.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,54 +16,57 @@
 import dataclasses
 import importlib
 import os
 import random
 import re
 import sys
 import types
-from typing import Any
 import uuid
 
 from absl import flags
 from absl.testing import absltest
 from absl.testing import parameterized
 import fiddle as fdl
 from fiddle import daglish
 from fiddle import tagging
 from fiddle._src.codegen.auto_config import experimental_top_level_api
 from fiddle._src.codegen.auto_config import test_fixtures
 from fiddle._src.testing import nested_values
 from fiddle._src.testing import test_util
+from fiddle._src.testing.example import demo_configs
 from fiddle._src.testing.example import fake_encoder_decoder
 from fiddle.experimental.auto_config import auto_config
 
 
-@dataclasses.dataclass(frozen=True)
-class ModelWrapper:
-  model: Any
-
-
-@dataclasses.dataclass(frozen=True)
-class AnotherClass:
-  foo: Any
-  bar: Any
-
-
 def make_arg_factory_config():
   return fdl.Partial(
       test_fixtures.EncoderLayer,
       attention=fdl.ArgFactory(
           test_fixtures.Attention,
           kernel_init=fdl.ArgFactory(
               test_fixtures.initializer, name="const", dtype="float32"
           ),
       ),
   )
 
 
+def create_random_sub_fixture(config, rng, ratio=0.5):
+  fixtures = {}
+  for value, _ in daglish.iterate(config):
+    if (
+        isinstance(value, fdl.Buildable)
+        # TODO(b/284359119): Support fdl.ArgFactory as sub-fixture.
+        and (not isinstance(value, fdl.ArgFactory))
+    ):
+      if rng.random() < ratio:
+        name = f"sub_fixture_{len(fixtures) + 1}"
+        fixtures[name] = value
+  return fixtures
+
+
 class ExperimentalTopLevelApiTest(test_util.TestCase, parameterized.TestCase):
 
   def get_tempdir(self):
     try:
       flags.FLAGS.test_tmpdir
     except flags.UnparsedFlagAccessError:
       # Sometimes need to initialize flags when running `pytest`.
@@ -126,16 +129,17 @@
       # `auto_config` checks that a Buildable is returned, to avoid user errors.
       has_buildables = any(
           isinstance(value, fdl.Buildable)
           for value, _ in daglish.iterate(config)
       )
       if has_buildables:
         with self.subTest(f"rng_{i}"):
+          sub_fixtures = create_random_sub_fixture(config, random.Random(i))
           code = experimental_top_level_api.auto_config_codegen(
-              config, **kwargs
+              config, sub_fixtures=sub_fixtures, **kwargs
           )
           module = self._load_code_as_module(code)
           generated_config = module.config_fixture.as_buildable()
           self.assertDagEqual(config, generated_config)
 
   def test_config_contains_tags_wo_default(self):
     @dataclasses.dataclass
@@ -272,10 +276,28 @@
             sub_fixtures={"model_fixture": config.model},
             max_expression_complexity=complexity,
         )
         module = self._load_code_as_module(code)
         generated_config = module.config_fixture.as_buildable()
         self.assertDagEqual(config, generated_config)
 
+  def test_nesting_shared_nodes(self):
+    config = demo_configs.nested_node_sharing_config.as_buildable()
+    for complexity in [None, 2, 3]:
+      with self.subTest(f"max_complexity_as_{complexity}"):
+        code = experimental_top_level_api.auto_config_codegen(
+            config,
+            sub_fixtures={
+                "fx_a": config.x,
+                "fx_f1": config.x.x,
+                "fx_f2": config.x.y,
+                "fx_f3": config.x.z,
+            },
+            max_expression_complexity=complexity,
+        )
+        module = self._load_code_as_module(code)
+        generated_config = module.config_fixture.as_buildable()
+        self.assertDagEqual(config, generated_config)
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/get_history_comments.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/get_history_comments.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/get_history_comments_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/get_history_comments_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/init_task.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/init_task.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/init_task_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/init_task_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_printer.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,17 @@
       arguments = ", ".join(
           f"{name}={sub_value}" for name, sub_value in arguments.items()
       )
       buildable_type = format_py_reference(type(value))
       fn = format_py_reference(fdl.get_callable(value))
       return f"{buildable_type}({fn}, {arguments})"
     elif isinstance(value, (list, tuple)):
-      children = ", ".join(sub_value for sub_value in state.map_children(value))
+      children = ", ".join(
+          str(sub_value) for sub_value in state.map_children(value)
+      )
       if isinstance(value, tuple):
         if len(value) == 1:
           children += ","
         return f"({children})"
       else:
         return f"[{children}]"
     elif isinstance(value, dict):
```

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_printer_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_printer_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_to_cst.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_to_cst.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_to_cst_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_to_cst_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/make_symbolic_references.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/make_symbolic_references.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/naming.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/naming.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,18 +128,15 @@
         pass
       else:
         candidates.append(_camel_to_snake(cls_name))
 
     if not candidates and not paths:
       candidates.append("root")
     if not candidates:
-      raise NameGenerationError(
-          f"Could not generate any candidate names for {value!r} with "
-          f"paths {paths!r}"
-      )
+      candidates.append("unnamed_var")
     return self.name_from_candidates(candidates)
 
 
 @dataclasses.dataclass
 class TypeFirstNamer(Namer):
   """Namer that chooses type names over path names.
```

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/naming_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/naming_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,21 +130,27 @@
         ".bar": "bar",
         ".bar['qux']": "bar_qux"
     })
 
   def test_names_as_documented_example_2(self):
     config = [{1: "hi"}]
     namer = new_path_first_namer()
-    with self.assertRaises(ValueError):
-      namer.name_for(config[0][1], [(
-          daglish.Index(0),
-          daglish.Key(1),
-      )])
-    with self.assertRaises(ValueError):
-      namer.name_for(config[0], [(daglish.Index(0),)])
+    self.assertEqual(
+        namer.name_for(
+            config[0][1],
+            [(
+                daglish.Index(0),
+                daglish.Key(1),
+            )],
+        ),
+        "unnamed_var",
+    )
+    self.assertEqual(
+        namer.name_for(config[0], [(daglish.Index(0),)]), "unnamed_var_2"
+    )
     self.assertEqual(namer.name_for(config, [()]), "root")
 
 
 class TypeFirstNamerTest(absltest.TestCase):
 
   def test_name_for_doesnt_add_root_unnecessarily(self):
     config = fake_encoder_decoder.fixture.as_buildable()
```

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/parents_first_traversal.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/parents_first_traversal.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from fiddle._src.codegen.auto_config import parents_first_traversal
 from fiddle._src.testing import nested_values
 
 
 def get_traversal_order(structure) -> List[Any]:
   result = []
 
-  def traverse_fn(value, parent_values):
-    del parent_values  # unused
+  def traverse_fn(value, parent_results):
+    del parent_results  # unused
     result.append(value)
 
   parents_first_traversal.traverse_parents_first(traverse_fn, structure)
   return result
 
 
 class ParentsFirstTraversalTest(absltest.TestCase):
@@ -77,10 +77,25 @@
   def test_can_traverse_all(self):
     for rng_seed in range(100):
       with self.subTest(f"rng_seed={rng_seed}"):
         rng = random.Random(rng_seed)
         structure = nested_values.generate_nested_value(rng)
         get_traversal_order(structure)
 
+  def test_parent_results(self):
+    shared = {"a": 1, "b": 2}
+    x = {"a": 3, "b": shared}
+    y = {"a": 4, "b": shared}
+    config = {"a": x, "b": y}
+
+    def traverse_fn(value, parent_results):
+      if value is shared:
+        self.assertLen(parent_results, 2)
+        self.assertIn(x, parent_results)
+        self.assertIn(y, parent_results)
+      return value
+
+    parents_first_traversal.traverse_parents_first(traverse_fn, config)
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/shared_to_variables.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/shared_to_variables.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/shared_to_variables_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/shared_to_variables_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/split_arg_factories.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/split_arg_factories.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/split_arg_factories_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/split_arg_factories_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/sub_fixture_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/new_codegen_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,87 +9,99 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for transform_sub_fixtures pass."""
+"""Tests for new_codegen."""
 
+import importlib
+import os
+import re
+import sys
+import types
+import uuid
+
+from absl import flags
 from absl.testing import absltest
-import fiddle as fdl
-from fiddle._src.codegen.auto_config import init_task
-from fiddle._src.codegen.auto_config import sub_fixture
-from fiddle._src.codegen.auto_config import test_fixtures
+from fiddle._src.codegen import new_codegen
 from fiddle._src.testing.example import fake_encoder_decoder
 
 
-class SubFixtureTest(absltest.TestCase):
-
-  def test_find_shared_nodes(self):
-    config = fake_encoder_decoder.fixture.as_buildable()
-    fixtures = {"fake_encoder": config.encoder, "fake_decoder": config.decoder}
-    shared_node_lib, fixture_share_nodes_lib = sub_fixture._find_shared_nodes(
-        config, sub_fixtures=fixtures
-    )
-    shared_node = config.encoder.embedders["tokens"]
+class NewCodegenTest(absltest.TestCase):
 
-    with self.subTest("shared_node_lib"):
-      self.assertIn(id(shared_node), shared_node_lib)
-      self.assertLen(shared_node_lib, 1)
-
-    with self.subTest("fixture_share_nodes_lib"):
-      self.assertLen(fixture_share_nodes_lib, 2)
-      for fixture in fixtures.values():
-        self.assertIn(id(fixture), fixture_share_nodes_lib)
-        self.assertSetEqual(
-            fixture_share_nodes_lib[id(fixture)], {id(shared_node)}
-        )
+  def get_tempdir(self):
+    try:
+      flags.FLAGS.test_tmpdir
+    except flags.UnparsedFlagAccessError:
+      # Sometimes need to initialize flags when running `pytest`.
+      program, *rest = sys.argv
+      rest = [flag for flag in rest if "test_tmpdir" in flag]
+      flags.FLAGS([program, *rest])
+    return self.create_tempdir().full_path
+
+  def _load_code_as_module(self, code: str) -> types.ModuleType:
+    # Write the generated config to a module, and load it. We can't just exec()
+    # it because auto_config needs access to the source code.
+    temp_dir = self.get_tempdir()
+    sys.path.append(temp_dir)
+    uuid_str = str(hash(uuid.uuid4()))
+    file_path = os.path.join(temp_dir, f"config_{uuid_str}.py")
+    with open(file_path, "w") as f:
+      f.write(code)
+    return importlib.import_module(f"config_{uuid_str}")
 
-  def test_fake_encoder_decoder(self):
+  def test_codegen(self):
     config = fake_encoder_decoder.fixture.as_buildable()
-    config.encoder.embedders = None
-    config.decoder.embedders = None
+    code = new_codegen.new_codegen(config=config, max_expression_complexity=4)
+    self.assertNotIn(code, "auto_config")
+    fixture = self._load_code_as_module(code).config_fixture
+    self.assertEqual(fixture(), config)
 
-    task = init_task.init_task(config)
-    sub_fixture.transform_sub_fixtures(
-        task, {"fake_encoder": config.encoder, "fake_decoder": config.decoder}
+  def test_sub_fixtures(self):
+    config = fake_encoder_decoder.fixture.as_buildable()
+    code = new_codegen.new_codegen(
+        config=config,
+        max_expression_complexity=4,
+        sub_fixtures={
+            "encoder_fixture": config.encoder,
+            "decoder_fixture": config.decoder,
+        },
     )
-    self.assertLen(task.top_level_call.children, 2)
 
-  def test_nested_sub_fixture(self):
-    config = fake_encoder_decoder.fixture.as_buildable()
-    task = init_task.init_task(config)
-    sub_fixture.transform_sub_fixtures(
-        task,
-        {"fake_encoder": config.encoder, "attention": config.encoder.attention},
+    self.assertNotIn(code, "auto_config")
+
+    # Ensure that sub-fixtures were actually created.
+    matches = re.findall(r"def\ (?P<name>[\w_]+)\(", code)
+    self.assertEqual(
+        matches, ["config_fixture", "encoder_fixture", "decoder_fixture"]
     )
-    self.assertLen(task.top_level_call.children, 2)
 
-  def test_conflicting_name_raises_errors(self):
-    config = fake_encoder_decoder.fixture.as_buildable()
-    task = init_task.init_task(config)
-    with self.assertRaisesRegex(
-        ValueError, "already exists in the top level fixture"
-    ):
-      sub_fixture.transform_sub_fixtures(
-          task, {"config_fixture": config.encoder}
-      )
-
-  # TODO(b/284359119): Support fdl.ArgFactory as sub-fixture.
-  def test_arg_factory_raises_errors(self):
-    config = fdl.Partial(
-        test_fixtures.EncoderLayer,
-        attention=fdl.ArgFactory(
-            test_fixtures.Attention,
-            kernel_init=fdl.ArgFactory(
-                test_fixtures.initializer, name="const", dtype="float32"
-            ),
-        ),
+    fixture = self._load_code_as_module(code).config_fixture
+    self.assertEqual(fixture(), config)
+
+  def test_code_output(self):
+    config = fake_encoder_decoder.fixture.as_buildable().encoder
+    code = new_codegen.new_codegen(
+        config=config,
+        max_expression_complexity=4,
     )
-    task = init_task.init_task(config)
-    with self.assertRaisesRegex(ValueError, "fdl.ArgFactory is not supported"):
-      sub_fixture.transform_sub_fixtures(task, {"attention": config.attention})
+    expected = """
+    import fiddle as fdl
+    from fiddle._src.testing.example import fake_encoder_decoder
+
+
+    def config_fixture():
+        mlp = fdl.Config(fake_encoder_decoder.Mlp, dtype='float32',
+          use_bias=False, sharding_axes=['embed', 'num_heads', 'head_dim'])
+        return fdl.Config(fake_encoder_decoder.FakeEncoder, embedders={'tokens':
+          fdl.Config(fake_encoder_decoder.TokenEmbedder, dtype='float32'),
+          'position': None},
+          attention=fdl.Config(fake_encoder_decoder.Attention, dtype='float32',
+          kernel_init='uniform()', bias_init='zeros()'), mlp=mlp)
+    """
+    self.assertEqual(code.split(), expected.split())
 
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/auto_config/test_fixtures.py` & `fiddle-0.2.9/fiddle/_src/codegen/auto_config/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/codegen_diff.py` & `fiddle-0.2.9/fiddle/_src/codegen/codegen_diff.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/formatting_utilities.py` & `fiddle-0.2.9/fiddle/_src/codegen/formatting_utilities.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/import_manager.py` & `fiddle-0.2.9/fiddle/_src/codegen/import_manager.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/import_manager_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/import_manager_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/legacy_codegen.py` & `fiddle-0.2.9/fiddle/_src/codegen/legacy_codegen.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/legacy_codegen_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/legacy_codegen_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/mini_ast.py` & `fiddle-0.2.9/fiddle/_src/codegen/mini_ast.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/namespace.py` & `fiddle-0.2.9/fiddle/_src/codegen/namespace.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/namespace_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/namespace_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/new_codegen.py` & `fiddle-0.2.9/fiddle/_src/codegen/new_codegen.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/newcg_symbolic_references.py` & `fiddle-0.2.9/fiddle/_src/codegen/newcg_symbolic_references.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/newcg_symbolic_references_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/newcg_symbolic_references_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/py_val_to_cst_converter.py` & `fiddle-0.2.9/fiddle/_src/codegen/py_val_to_cst_converter.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/py_val_to_cst_converter_test.py` & `fiddle-0.2.9/fiddle/_src/codegen/py_val_to_cst_converter_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/special_value_codegen.py` & `fiddle-0.2.9/fiddle/_src/codegen/special_value_codegen.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/test_submodule/__init__.py` & `fiddle-0.2.9/fiddle/_src/codegen/test_submodule/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/test_submodule/test_util.py` & `fiddle-0.2.9/fiddle/_src/codegen/test_submodule/test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/codegen/test_util.py` & `fiddle-0.2.9/fiddle/_src/codegen/test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/config.py` & `fiddle-0.2.9/fiddle/_src/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 import itertools
 import logging
 import types
 from typing import Any, Callable, Collection, Dict, FrozenSet, Generic, Iterable, Mapping, NamedTuple, Optional, Set, Tuple, Type, TypeVar, Union
 
 from fiddle._src import arg_factory
 from fiddle._src import daglish
-from fiddle._src import field_metadata
 from fiddle._src import history
 from fiddle._src import signatures
 from fiddle._src import tag_type
 
 
 T = TypeVar('T')
 TypeOrCallableProducingT = Union[Callable[..., T], Type[T]]
@@ -255,19 +254,14 @@
             'Variable positional arguments (aka `*args`) not supported. '
             f'Found param `{name}` in `{fn_or_cls}`.'
         )
         raise NotImplementedError(err_msg)
       elif param.kind == param.VAR_KEYWORD:
         arguments.update(arguments.pop(param.name))
 
-    if dataclasses.is_dataclass(self.__fn_or_cls__):
-      fields = dataclasses.fields(self.__fn_or_cls__)
-      _add_dataclass_tags(self, fields)
-      _expand_dataclass_default_factories(self, fields, arguments)
-
     for name, value in arguments.items():
       setattr(self, name, value)
 
     for name, tags in tag_type.find_tags_from_annotations(fn_or_cls).items():
       self.__argument_tags__[name].update(tags)
       self.__argument_history__.add_updated_tags(
           name, self.__argument_tags__[name]
@@ -558,186 +552,14 @@
     self.__dict__.update(state)  # Support unpickle.
     if '__signature__' not in self.__dict__:
       object.__setattr__(
           self, '__signature__', signatures.get_signature(self.__fn_or_cls__)
       )
 
 
-def _add_dataclass_tags(buildable, fields):
-  """Adds tags to arguments as indicated by dataclass fields.
-
-  If any dataclass field in ``fields`` has metadata indicating that the field
-  should be given one or more tags, then add those tags to the argument
-  corresponding to the field.
-
-  Args:
-    buildable: The buildable that should be updated.
-    fields: The dataclass fields for buildable.__fn_or_cls__.
-  """
-  for field in fields:
-    metadata = field_metadata.field_metadata(field)
-    if metadata:
-      for tag in metadata.tags:
-        add_tag(buildable, field.name, tag)
-
-
-def _expand_dataclass_default_factories(buildable, fields, arguments):
-  """Expand default-valued args for dataclass fields with default-factories.
-
-  If an argument has no value supplied when initializing a dataclass, but the
-  corresponding field has a default factory, then that factory will be used to
-  construct the argument's value. Thus, when creating a ``fdl.Buildable`` for
-  the dataclass, it may be possible to fill in the value for the argument with
-  ``Config(factory)``, without changing the value that will be built by
-  ``buildable`` when calling ``fdl.build``.  This is useful because it makes the
-  argument "deeply configurable" -- i.e., if the factory has any optional
-  arguments, then this makes it possible to configure those objects. And in the
-  special case where ``factory`` is an ``@auto_config``'d function, we can make
-  the argument even more deeply configurable by inlining the factory.
-
-  However, expanding default-valued args into `Buildable`s should only be
-  performed when it can be done safely -- i.e., without changing the value
-  that will be built by ``buildable``. In particular, we need to be careful
-  not to create any "unintentional sharing," where the value built by the
-  default factory is used by multiple instances of the dataclass.
-
-  If we are not able to do the expansion safely, then we raise an exception.
-  Note that it would be "safe" to leave the argument empty, in so far as the
-  original semantics would be preserved.  But having the argument be
-  unexpectedly unconfigurable could lead to difficult-to-diagnose issues.
-  E.g., any nested dataclasses with `fdl.Tag`s associated with fields will
-  not be accessable.
-
-  One case where it *is* safe to expand default factories is when
-  ``type(buildable)`` is ``fdl.Config``.  In that case, we know that a single
-  dataclass object will be built from `buildable`, so we are guaranteed that the
-  value built by the default factory will only be used by that one object.
-
-  However, if ``type(buildable)`` is ``fdl.Partial``, then the function built
-  from ``buildable`` can be used to generate multiple dataclass instances; and
-  we need to ensure that the default factory is called for each instance.  For
-  this case, we use ``ArgFactory(factory)`` rather than ``Config(factory)`` to
-  expand the argument.  This ensures that the factory is called each time the
-  partial is called.  We also need to replace any nested ``Config``'s with
-  ``ArgFactory``'s, to ensure that the nested values are created each time as
-  well.
-
-  Similarly, if ``type(buildable) is fdl.ArgFactory``, then the factory function
-  built from ``buildable`` can be used to generate multiple dataclass instances,
-  so we use ``ArgFactory(factory)`` to expand arguments.
-
-  In the case where ``type(buildable)`` is ``fdl.Partial`` or
-  ``fdl.ArgFactory``, there is one additional corner case to consider, which
-  occurs when multiple nested partials makes it impossible for Fiddle to
-  describe the correct instance sharing pattern with its current ``Buildable``
-  subclasses.  This corner case is demonstrated by the following example:
-
-  ```
-  def f(x):
-    return x
-  def g():
-    return object()
-  @auto_config.auto_config
-  def make_fn():
-    return functools.partial(f, x=g())
-  @dataclasses.dataclass
-  class A:
-    fn: Callable[[], object] = fdl_field(default_factory=make_fn)
-  p = functools.partial(A)
-  ```
-
-  Here, if we write ``a1 = p()`` to create an instance of ``A``, then calling
-  ``a1.fn()`` multiple times will always return the same object, while another
-  instance ``a2 = p()`` will return a different object when calling ``a2.fn()``:
-
-  ```
-  a1, a2 = p(), p()              # call the partial function twice.
-  assert a1.fn() is a1.fn()      # a1.fn always returns the same object.
-  assert a1.fn() is not a2.fn()  # a1 and a2 return different objects.
-  ```
-
-  However, if we construct ``fdl.Partial(A)``, and try to make ``f`` and ``g``
-  deeply configurable, then there's no way to generate the same behavior
-  using Fiddle ``Buildable``'s:
-
-  * If we use ``fdl.Partial(A, fdl.Partial(f, fdl.Config(g)))``, then all
-    instances of ``A`` generated by ``p`` will return the same instance
-    (namely, the instance constructed by ``fdl.build(fdl.Config(g))``).
-  * If we use ``fdl.Partial(A, fdl.Partial(f, fdl.ArgFactory(g)))``, then
-    every call to ``A.fn`` will return a new object.
-
-  Therefore, since is not possible to make the field ``A.fn`` deeply
-  configurable while preserving the original semantics, we instead raise
-  an exception.  If you believe you have a valid use-case for this, please
-  contact the Fiddle team.
-
-  The precise circumstances that cause this problem are: when we are building
-  a ``Partial`` (or ``ArgFactory``), and the default factory expands into an
-  expression containing a ``Partial`` (or ``ArgFactory``) that contains a
-  ``Config`` -- in that case, the object built for the `Config` should be shared
-  for each call to the inner partial; but should *not* be shared for each call
-  to the outer partial.
-
-  Args:
-    buildable: The buildable that should be updated.
-    fields: The dataclass fields for ``buildable.__fn_or_cls__``.
-    arguments: The arguments that are being used to construct this
-      ``Buildable``. If any argument has no value, and the corresponding field
-      has a default factory, then the argument will be expanded into an
-      equivalent ``Buildable`` if it's possible to do so without changing the
-      semantics of ``fdl.build(buildable)``.
-  """
-
-  def convert_to_arg_factory(value, state):
-    """Converts `cfg` and any nested `Config` objects to ArgFactory."""
-    if not isinstance(value, Partial):  # Don't recurse into partials.
-      value = state.map_children(value)
-    if isinstance(value, Config):
-      value = cast(ArgFactory, value)
-    return value
-
-  def contains_partial_that_contains_config(value, state):
-    """True if value contains a Partial/ArgFactory that contains a Config."""
-    if isinstance(value, (Partial, ArgFactory)):
-      return any(isinstance(v, Config) for v, _ in daglish.iterate(value))
-    elif state.is_traversable(value):
-      return any(state.flattened_map_children(value).values)
-    else:
-      return False
-
-  for field in fields:
-    if field.name in arguments:
-      continue  # We have an explicit value for this argument.
-    metadata = field_metadata.field_metadata(field)
-    if not (metadata and metadata.buildable_initializer):
-      continue
-    field_config = metadata.buildable_initializer()
-    if daglish.MemoizedTraversal.run(
-        contains_partial_that_contains_config, field_config
-    ):
-      cls_name = getattr(
-          buildable.__fn_or_cls__, '__qualname__', repr(buildable.__fn_or_cls__)
-      )
-      raise ValueError(
-          f'Unable to safely replace {cls_name}.{field.name} with '
-          'a `fdl.Buildable`, because its default factory contains a '
-          '`fdl.Partial` that contains a `fdl.Config`.  This makes it '
-          'difficult for Fiddle to describe the correct instance-sharing '
-          'pattern. If you believe that you have a valid use-case for this, '
-          'please contact the Fiddle team.'
-      )
-    if isinstance(field_config, Config) and isinstance(
-        buildable, (Partial, ArgFactory)
-    ):
-      field_config = daglish.MemoizedTraversal.run(
-          convert_to_arg_factory, field_config
-      )
-    arguments[field.name] = field_config
-
-
 class Config(Generic[T], Buildable[T]):
   """A mutable representation of a function or class's parameters.
 
   This class represents the configuration for a given function or class,
   exposing configured parameters as mutable attributes. For example, given a
   class::
 
@@ -1154,21 +976,14 @@
         )
 
   object.__setattr__(buildable, '__fn_or_cls__', new_callable)
   object.__setattr__(buildable, '__signature__', signature)
   object.__setattr__(buildable, '_has_var_keyword', has_var_keyword)
   buildable.__argument_history__.add_new_value('__fn_or_cls__', new_callable)
 
-  if dataclasses.is_dataclass(buildable.__fn_or_cls__):
-    fields = dataclasses.fields(buildable.__fn_or_cls__)
-    _add_dataclass_tags(buildable, fields)
-    _expand_dataclass_default_factories(
-        buildable, fields, buildable.__arguments__
-    )
-
 
 def assign(buildable: Buildable, **kwargs):
   """Assigns multiple arguments to ``buildable``.
 
   Although this function does not enable a caller to do something they can't
   already do with other syntax, this helper function can be useful when
   manipulating deeply nested configs. Example::
```

### Comparing `fiddle-0.2.8/fiddle/_src/config_test.py` & `fiddle-0.2.9/fiddle/_src/config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/daglish.py` & `fiddle-0.2.9/fiddle/_src/daglish.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/daglish_extensions.py` & `fiddle-0.2.9/fiddle/_src/daglish_extensions.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/daglish_extensions_test.py` & `fiddle-0.2.9/fiddle/_src/daglish_extensions_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/daglish_test.py` & `fiddle-0.2.9/fiddle/_src/daglish_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/diffing.py` & `fiddle-0.2.9/fiddle/_src/diffing.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/diffing_test.py` & `fiddle-0.2.9/fiddle/_src/diffing_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/__init__.py` & `fiddle-0.2.9/fiddle/_src/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/auto_config.py` & `fiddle-0.2.9/fiddle/_src/experimental/auto_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import builtins
 import dataclasses
 import functools
 import inspect
 import linecache
 import textwrap
 import types
-from typing import Any, Callable, cast, Optional
+from typing import Any, Callable, Optional, Type, cast
 
 from fiddle._src import arg_factory
 from fiddle._src import building
 from fiddle._src import config
 from fiddle._src import mutate_buildable
 from fiddle._src.experimental import auto_config_policy
 from fiddle._src.experimental import daglish_legacy
@@ -473,15 +473,15 @@
   else:
     # For earlier versions of Python, build a dummy function to get CellType.
     dummy_fn = lambda: contents
     cell_type = type(dummy_fn.__closure__[0])
     return cell_type(contents)
 
 
-def _convert_callable_to_fiddle_arg_factory(arg):
+def _maybe_as_arg_factory(arg_factory_cls, arg):
   """Converts an argument of an arg_factory partial() to Fiddle buildables.
 
   In normal Python, one expresses arg factories like,
 
   my_fn = arg_factory.partial(fn, foo=foo_factory, bar=bar_factory)
 
   where `foo_factory` produces a `foo` and `bar_factory` produces a `bar`. These
@@ -498,34 +498,38 @@
 
   If `foo_factory` or `bar_factory` is not a callable or fdl.Partial, then we
   raise an error. It's techincally possible to pass `foo_factory` as a
   fdl.Config object that, when called, returns another fucntion, but this is
   most likely a mistake in configuration, so we don't allow it.
 
   Args:
+    arg_factory_cls: The type to use when creating the ArgFactory (normally this
+      will just be `fdl.ArgFactory`, but can potentially be customized).
     arg: Intermediate value passed to `arg_factory.partial`.
 
   Returns:
     ArgFactory version of a configuration or callable.
   """
   if isinstance(arg, config.Partial):
-    return config.cast(config.ArgFactory, arg)
+    return config.cast(arg_factory_cls, arg)
   elif callable(arg):
-    return config.ArgFactory(arg)
+    return arg_factory_cls(arg)
   else:
     raise ValueError(
         "Couldn't figure out how to handle arg_factory argument; please "
         f'bind any constant args with a nested functools.partial. Arg: {arg!r}'
     )
 
 
-def _make_partial(buildable_or_callable, *args, **kwargs):
-  """Makes a fdl Partial, but calling appropriate APIs if casting is required.
+def _make_partial(partial_cls, buildable_or_callable, *args, **kwargs):
+  """Makes a fdl.Partial, but calling appropriate APIs if casting is required.
 
   Args:
+    partial_cls: The type to use when creating the Partial (normally this will
+      just be `fdl.Partial`, but can potentially be customized).
     buildable_or_callable: Callable or existing configuration object to update.
     *args: Positional arguments, only supported when `config_or_callable` is a
       Partial already.
     **kwargs: Keyword arguments.
 
   Returns:
     New callable.
@@ -539,15 +543,15 @@
       raise ValueError(
           'For chained functools.partial calls inside auto_config, e.g. '
           'functools.partial(functools.partial(foo, ...), ...), only keyword '
           f'arguments can be supplied to the outer call. Got: {args!r}'
       )
     return config.copy_with(buildable_or_callable, **kwargs)
   else:
-    return config.Partial(buildable_or_callable, *args, **kwargs)
+    return partial_cls(buildable_or_callable, *args, **kwargs)
 
 
 def exempt(fn_or_cls: Callable[..., Any]) -> Callable[..., Any]:
   """Wrap a callable so that it's exempted from auto_config.
 
   This can be used either as a decorator to exempt a function, or used inside
   an auto_config function to inline exempt certain calls to a function.
@@ -573,22 +577,29 @@
     config if called inside an auto_config function.
   """
   return AutoConfig(
       func=fn_or_cls, buildable_func=fn_or_cls, always_inline=True
   )
 
 
+@dataclasses.dataclass(frozen=True)
+class ConfigTypes:
+  config_cls: Type[config.Config] = config.Config
+  partial_cls: Type[config.Partial] = config.Partial
+  arg_factory_cls: Type[config.ArgFactory] = config.ArgFactory
+
+
 def auto_config(
     fn=None,
     *,
     experimental_allow_dataclass_attribute_access=False,
     experimental_allow_control_flow: bool = False,
     experimental_always_inline: Optional[bool] = None,
     experimental_exemption_policy: Optional[auto_config_policy.Policy] = None,
-    experimental_config_cls=config.Config,
+    experimental_config_types: ConfigTypes = ConfigTypes(),
     experimental_result_must_contain_buildable: bool = True,
 ) -> Any:  # TODO(b/272377821): More precise return type.
   """Rewrites the given function to make it generate a ``Config``.
 
   This function creates a new function from ``fn`` by rewriting its AST
   (abstract syntax tree), replacing all ``Call`` nodes with a custom call
   handler. When the rewritten function is run, the call handler intercepts calls
@@ -667,18 +678,20 @@
       documentation on ``inline`` for an example. The default (if unspecified)
       is currently ``False``, but this may change in the future.
     experimental_exemption_policy: An optional policy to control which function
       calls within the body of ``fn`` should be turned into ``fdl.Config``'s and
       which ones should simply be executed normally during the ``as_buildable``
       interpretation of ``fn``. This predicate should return ``True`` if the
       given callable should be exempted from auto-configuration.
-    experimental_config_cls: The class to use to generate configs. By default,
-      this is just ``fdl.Config``, but projects with custom ``Config``
-      subclasses can use this to override the default. This is experimental and
-      may be removed in the future.
+    experimental_config_types: A ``ConfigTypes`` instance containing the types
+      to use when generating configs. By default, this just supplies the
+      standard Fiddle types ()``fdl.Config``, ``fdl.Partial``, and
+      ``fdl.ArgFactory``), but projects with custom subclasses can use this to
+      override the default. This is experimental and may be removed in the
+      future.
     experimental_result_must_contain_buildable: If true, then raise an error if
       `fn.as_buildable` returns a result that does not contain any `Buildable`
       values -- e.g., if it returns an empty dict.
 
   Returns:
     A wrapped version of ``fn``, but with an additional ``as_buildable``
     attribute containing the rewritten function.
@@ -708,32 +721,35 @@
     Returns:
       Depending on `fn_or_cls`, either `Partial`, a `Config`, or the result of
       calling `fn_or_cls` with the provided arguments.
     """
     if isinstance(fn_or_cls, AutoConfig) and fn_or_cls.always_inline:
       return fn_or_cls.as_buildable(*args, **kwargs)
 
+    partial_cls = experimental_config_types.partial_cls
     if fn_or_cls is functools.partial:
-      return _make_partial(args[0], *args[1:], **kwargs)
+      return _make_partial(partial_cls, args[0], *args[1:], **kwargs)
     elif fn_or_cls is arg_factory.partial:
+      arg_factory_cls = experimental_config_types.arg_factory_cls
       return _make_partial(
+          partial_cls,
           args[0],
-          *[_convert_callable_to_fiddle_arg_factory(arg) for arg in args[1:]],
+          *[_maybe_as_arg_factory(arg_factory_cls, arg) for arg in args[1:]],
           **{
-              name: _convert_callable_to_fiddle_arg_factory(arg)
+              name: _maybe_as_arg_factory(arg_factory_cls, arg)
               for name, arg in kwargs.items()
           },
       )
 
     if fn_or_cls is exempt:
       return fn_or_cls(*args, **kwargs)
     if experimental_exemption_policy(fn_or_cls):
       return fn_or_cls(*args, **kwargs)
 
-    return experimental_config_cls(fn_or_cls, *args, **kwargs)
+    return experimental_config_types.config_cls(fn_or_cls, *args, **kwargs)
 
   def auto_config_attr_load_handler(value, attr, allow_dataclass=True):
     """Handles attribute access in auto_config'ed functions."""
     if isinstance(value, config.Buildable):
       fn_or_cls = value.__fn_or_cls__
       if allow_dataclass and dataclasses.is_dataclass(fn_or_cls):
         return getattr(value, attr)
```

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/auto_config_policy.py` & `fiddle-0.2.9/fiddle/_src/experimental/auto_config_policy.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/auto_config_test.py` & `fiddle-0.2.9/fiddle/_src/experimental/auto_config_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,30 +468,49 @@
 
     with self.assertRaisesRegex(
         TypeError, r'The `auto_config` rewritten version of '
         r'`AutoConfigTest\.\w+\.<locals>\.test_config` returned a `dict`, '
         r'which is not \(or did not contain\) a `fdl\.Buildable`\.'):
       test_config.as_buildable()
 
-  def test_experimental_config_cls(self):
-
+  def test_experimental_config_types(self):
     class CustomConfig(fdl.Config):
       pass
 
-    @auto_config.auto_config(experimental_config_cls=CustomConfig)
+    class CustomPartial(fdl.Partial):
+      pass
+
+    class CustomArgFactory(fdl.ArgFactory):
+      pass
+
+    config_types = auto_config.ConfigTypes(
+        config_cls=CustomConfig,
+        partial_cls=CustomPartial,
+        arg_factory_cls=CustomArgFactory,
+    )
+
+    def make_int() -> int:
+      return 42
+
+    @auto_config.auto_config(experimental_config_types=config_types)
     def fn():
-      return FrozenSampleClass(arg1=basic_fn(3), arg2=4)
+      return FrozenSampleClass(
+          arg1=functools.partial(basic_fn, make_int()),
+          arg2=arg_factory.partial(basic_fn, make_int),
+      )
 
     expected = CustomConfig(
-        FrozenSampleClass, arg1=CustomConfig(basic_fn, 3), arg2=4
+        FrozenSampleClass,
+        arg1=CustomPartial(basic_fn, CustomConfig(make_int)),
+        arg2=CustomPartial(basic_fn, CustomArgFactory(make_int)),
     )
     cfg = fn.as_buildable()
+    # This assertion ensures that the correct types were produced (in addition
+    # to the leaf/parameter values in the config).
     self.assertDagEqual(cfg, expected)
-    self.assertIsInstance(cfg, CustomConfig)
-    self.assertIsInstance(cfg.arg1, CustomConfig)
 
   def test_staticmethod_nullary(self):
 
     class MyClass:
 
       @auto_config.auto_config
       @staticmethod
@@ -895,15 +914,15 @@
         auto_config.UnsupportedLanguageConstructError,
         r'Control flow \(Try\) is unsupported by auto_config\.'):
       auto_config.auto_config(test_config)
 
   def test_disallow_raise(self):
 
     def test_config():
-      raise Exception()
+      raise ValueError('Some message.')
 
     with self.assertRaisesRegex(
         auto_config.UnsupportedLanguageConstructError,
         r'Control flow \(Raise\) is unsupported by auto_config\.'):
       auto_config.auto_config(test_config)
 
     auto_config.auto_config(test_config, experimental_allow_control_flow=True)
```

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/autobuilders/__init__.py` & `fiddle-0.2.9/fiddle/_src/experimental/autobuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/autobuilders/autobuilders.py` & `fiddle-0.2.9/fiddle/_src/experimental/autobuilders/autobuilders.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/autobuilders/autobuilders_test.py` & `fiddle-0.2.9/fiddle/_src/experimental/autobuilders/autobuilders_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py` & `fiddle-0.2.9/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/configurator.py` & `fiddle-0.2.9/fiddle/_src/experimental/configurator.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/daglish_legacy.py` & `fiddle-0.2.9/fiddle/_src/experimental/daglish_legacy.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/daglish_legacy_test.py` & `fiddle-0.2.9/fiddle/_src/experimental/daglish_legacy_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/dict_config.py` & `fiddle-0.2.9/fiddle/_src/experimental/dict_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/dict_config_test.py` & `fiddle-0.2.9/fiddle/_src/experimental/dict_config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/namespace_config.py` & `fiddle-0.2.9/fiddle/_src/experimental/namespace_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/namespace_config_test.py` & `fiddle-0.2.9/fiddle/_src/experimental/namespace_config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/serialization.py` & `fiddle-0.2.9/fiddle/_src/experimental/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 import types
 from typing import Any, Dict, Iterable, List, Optional, Type
 
 from fiddle import daglish
 from fiddle._src import config as config_lib
 from fiddle._src import reraised_exception
 from fiddle._src.experimental import daglish_legacy
+from fiddle._src.experimental import lazy_imports
 
 
 _VERSION = '0.0.1'
 
 
 def clear_argument_history(buildable: config_lib.Buildable):
   """Creates a copy of a buildable, clearing its history.
@@ -408,14 +409,32 @@
 
 # Type identifier and keys used for Python reference values.
 _PYREF_TYPE = 'pyref'
 _MODULE_KEY = 'module'
 _NAME_KEY = 'name'
 
 
+def _serialize_lazy_imports(proxy_object):
+  """Serialize proxy object for lazy imports."""
+  qualname = proxy_object.__qualname__
+  parts = qualname.split(':')
+  if len(parts) == 2:
+    module_name, symbol_name = parts
+  elif len(parts) == 1:
+    module_name, symbol_name = qualname.rsplit('.', maxsplit=1)
+  else:
+    raise ValueError(f'Invalid qualname {qualname} for ProxyObject.')
+  output = {
+      _TYPE_KEY: _PYREF_TYPE,
+      _MODULE_KEY: module_name,
+      _NAME_KEY: symbol_name,
+  }
+  return output
+
+
 class Serialization:
   """Maintains state for an in-progress serialization.
 
   This class is used to recursively assemble a JSON-serializable dictionary
   representation of a given value. This class manages the state maintained
   during this process. The resulting dictionary representation can be obtained
   from the result property once an instance has been created:
@@ -514,15 +533,18 @@
 
   def _unique_name(self, value: Any) -> str:
     """Creates a unique and informative name for `value`."""
     try:
       hint_type = type(value)
       if isinstance(value, config_lib.Buildable):
         hint_type = config_lib.get_callable(value)
-      hint = hint_type.__name__
+      if isinstance(hint_type, lazy_imports.ProxyObject):
+        hint = hint_type.name
+      else:
+        hint = hint_type.__name__
     except AttributeError:
       hint = re.sub(r"[<>()\[\] '\"]", '', str(type(value)))
 
     hint = _to_snake_case(hint)
     for i in itertools.count(1):
       name = f'{hint}_{i}'
       if name not in self._objects:
@@ -608,14 +630,16 @@
       # the value.
       if _is_leaf_type(type(value)):
         if all_paths is None:
           return value  # If we don't need to add paths, just return the value.
         output = self._leaf(value)
       elif isinstance(value, (type, types.FunctionType, enum.Enum)):
         output = self._pyref(value, current_path)
+      elif isinstance(value, lazy_imports.ProxyObject):
+        output = _serialize_lazy_imports(value)
       elif id(value) in _serialization_constants_by_id:
         output = _serialization_constants_by_id[id(value)].to_pyref()
       elif (isinstance(value, collections.abc.Hashable) and
             value in _serialization_constants_by_value):
         output = _serialization_constants_by_value[value].to_pyref()
       else:
         msg = (f'Unserializable value {value} of type {type(value)}. Error '
```

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/transform.py` & `fiddle-0.2.9/fiddle/_src/experimental/transform.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/transform_test.py` & `fiddle-0.2.9/fiddle/_src/experimental/transform_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/visualize.py` & `fiddle-0.2.9/fiddle/_src/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/with_tags.py` & `fiddle-0.2.9/fiddle/_src/experimental/with_tags.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/with_tags_test.py` & `fiddle-0.2.9/fiddle/_src/experimental/with_tags_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/yaml_serialization.py` & `fiddle-0.2.9/fiddle/_src/experimental/yaml_serialization.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/experimental/yaml_serialization_test.py` & `fiddle-0.2.9/fiddle/_src/experimental/yaml_serialization_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/extensions/__init__.py` & `fiddle-0.2.9/fiddle/_src/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/extensions/flax_test.py` & `fiddle-0.2.9/fiddle/_src/extensions/flax_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/extensions/jax.py` & `fiddle-0.2.9/fiddle/_src/extensions/jax.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/extensions/seqio.py` & `fiddle-0.2.9/fiddle/_src/extensions/seqio.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/extensions/seqio_test.py` & `fiddle-0.2.9/fiddle/_src/extensions/seqio_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/extensions/tf.py` & `fiddle-0.2.9/fiddle/_src/extensions/tf.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/extensions/tf_test.py` & `fiddle-0.2.9/fiddle/_src/extensions/tf_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/graphviz.py` & `fiddle-0.2.9/fiddle/_src/graphviz.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/graphviz_custom_object.py` & `fiddle-0.2.9/fiddle/_src/graphviz_custom_object.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/history.py` & `fiddle-0.2.9/fiddle/_src/history.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/history_test.py` & `fiddle-0.2.9/fiddle/_src/history_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/materialize.py` & `fiddle-0.2.9/fiddle/_src/materialize.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/materialize_test.py` & `fiddle-0.2.9/fiddle/_src/materialize_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/module_reflection.py` & `fiddle-0.2.9/fiddle/_src/module_reflection.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/module_reflection_test.py` & `fiddle-0.2.9/fiddle/_src/module_reflection_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/module_reflection_test_module.py` & `fiddle-0.2.9/fiddle/_src/module_reflection_test_module.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/mutate_buildable.py` & `fiddle-0.2.9/fiddle/_src/mutate_buildable.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/mutate_buildable_test.py` & `fiddle-0.2.9/fiddle/_src/mutate_buildable_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/printing.py` & `fiddle-0.2.9/fiddle/_src/printing.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/printing_test.py` & `fiddle-0.2.9/fiddle/_src/printing_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/reraised_exception.py` & `fiddle-0.2.9/fiddle/_src/reraised_exception.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/reraised_exception_test.py` & `fiddle-0.2.9/fiddle/_src/reraised_exception_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/selectors.py` & `fiddle-0.2.9/fiddle/_src/selectors.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/selectors_test.py` & `fiddle-0.2.9/fiddle/_src/selectors_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/signatures.py` & `fiddle-0.2.9/fiddle/_src/signatures.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/signatures_test.py` & `fiddle-0.2.9/fiddle/_src/signatures_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/signatures_test_helper.py` & `fiddle-0.2.9/fiddle/_src/signatures_test_helper.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/tag_type.py` & `fiddle-0.2.9/fiddle/_src/tag_type.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/tagging.py` & `fiddle-0.2.9/fiddle/_src/tagging.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/tagging_test.py` & `fiddle-0.2.9/fiddle/_src/tagging_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 
 from absl.testing import absltest
 import cloudpickle
 import fiddle as fdl
 from fiddle import selectors
 from fiddle._src import tagging
 from fiddle._src import tagging_test_module as tst
-from fiddle.experimental import auto_config
-from fiddle.experimental import dataclasses as fdl_dc
 
 
 @dataclasses.dataclass
 class Foo:
   bar: int
   qux: str
 
@@ -48,25 +46,14 @@
   return kwargs
 
 
 def sample_function(x, y):
   return (x, y)
 
 
-@auto_config.auto_config
-def custom_default_factory():
-  return Foo(1, "2")
-
-
-@dataclasses.dataclass
-class Baz:
-  foo: Foo = fdl_dc.field(default_factory=custom_default_factory)
-  baz: int = 2
-
-
 def get_single_tag(tagged_value: tagging.TaggedValueCls) -> tagging.TagType:
   """Gets a single tag from a TaggedValue, errors if there are multiple."""
   assert isinstance(tagged_value, tagging.TaggedValueCls)
   assert len(tagged_value.tags) == 1
   return next(iter(tagged_value.tags))
 
 
@@ -175,21 +162,14 @@
         return_kwargs,
         foo=tst.ParameterDType.new(default=None),
         bar=tst.LinearParamDType.new(),
     )
     tagging.set_tagged(cfg, tag=tst.LinearParamDType, value=1)
     self.assertDictEqual(fdl.build(cfg), {"foo": None, "bar": 1})
 
-  def test_tagging_dataclass_field_defaults(self):
-    cfg = fdl.Config(Baz, foo=RedTag.new())
-    obj = fdl.build(cfg)
-    self.assertEqual(
-        obj.foo.bar, 1, "Default values from dataclass field missing."
-    )
-
   def test_set_two_taggedvalues(self):
     cfg = fdl.Config(
         return_kwargs,
         foo=tst.ParameterDType.new(default=None),
         bar=tst.LinearParamDType.new())
     tagging.set_tagged(cfg, tag=tst.ParameterDType, value=1)
     tagging.set_tagged(cfg, tag=tst.LinearParamDType, value=2)
```

### Comparing `fiddle-0.2.8/fiddle/_src/tagging_test_module.py` & `fiddle-0.2.9/fiddle/_src/tagging_test_module.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/testing/__init__.py` & `fiddle-0.2.9/fiddle/_src/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/testing/autotest.py` & `fiddle-0.2.9/fiddle/_src/testing/autotest.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/testing/example/__init__.py` & `fiddle-0.2.9/fiddle/_src/testing/example/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/testing/example/fake_encoder_decoder.py` & `fiddle-0.2.9/fiddle/_src/testing/example/fake_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/testing/example/person_friend_toy.py` & `fiddle-0.2.9/fiddle/_src/testing/example/person_friend_toy.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/testing/nested_values.py` & `fiddle-0.2.9/fiddle/_src/testing/nested_values.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/testing/nested_values_test.py` & `fiddle-0.2.9/fiddle/_src/testing/nested_values_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/testing/test_util.py` & `fiddle-0.2.9/fiddle/_src/testing/test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/_src/testing/test_util_test.py` & `fiddle-0.2.9/fiddle/_src/testing/test_util_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/absl_flags/__init__.py` & `fiddle-0.2.9/fiddle/absl_flags/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/absl_flags/example/__init__.py` & `fiddle-0.2.9/fiddle/absl_flags/example/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/absl_flags/example/business_logic.py` & `fiddle-0.2.9/fiddle/absl_flags/example/business_logic.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/absl_flags/example/configs.py` & `fiddle-0.2.9/fiddle/absl_flags/example/configs.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/absl_flags/example/example.py` & `fiddle-0.2.9/fiddle/absl_flags/example/example.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/absl_flags/example/tags.py` & `fiddle-0.2.9/fiddle/absl_flags/example/tags.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/arg_factory.py` & `fiddle-0.2.9/fiddle/arg_factory.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/building.py` & `fiddle-0.2.9/fiddle/building.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/codegen/__init__.py` & `fiddle-0.2.9/fiddle/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/codegen/auto_config/__init__.py` & `fiddle-0.2.9/fiddle/codegen/auto_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/codegen/auto_config/experimental_top_level_api.py` & `fiddle-0.2.9/fiddle/codegen/auto_config/experimental_top_level_api.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/codegen/codegen.py` & `fiddle-0.2.9/fiddle/codegen/codegen.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/codegen/codegen_diff.py` & `fiddle-0.2.9/fiddle/codegen/codegen_diff.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/codegen/py_val_to_cst_converter.py` & `fiddle-0.2.9/fiddle/codegen/py_val_to_cst_converter.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/config.py` & `fiddle-0.2.9/fiddle/config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/config_test.py` & `fiddle-0.2.9/fiddle/config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/daglish.py` & `fiddle-0.2.9/fiddle/daglish.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/diffing.py` & `fiddle-0.2.9/fiddle/diffing.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/examples/__init__.py` & `fiddle-0.2.9/fiddle/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/examples/colabs/__init__.py` & `fiddle-0.2.9/fiddle/examples/colabs/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/experimental/__init__.py` & `fiddle-0.2.9/fiddle/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/experimental/auto_config.py` & `fiddle-0.2.9/fiddle/experimental/auto_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,12 +23,13 @@
 """
 
 # pylint: disable=unused-import
 from fiddle._src.experimental.auto_config import auto_config
 from fiddle._src.experimental.auto_config import auto_config_policy
 from fiddle._src.experimental.auto_config import auto_unconfig
 from fiddle._src.experimental.auto_config import AutoConfig
+from fiddle._src.experimental.auto_config import ConfigTypes
 from fiddle._src.experimental.auto_config import exempt
 from fiddle._src.experimental.auto_config import inline
 from fiddle._src.experimental.auto_config import is_auto_config
 from fiddle._src.experimental.auto_config import UnsupportedLanguageConstructError
 from fiddle._src.experimental.with_tags import with_tags
```

### Comparing `fiddle-0.2.8/fiddle/experimental/auto_config_policy.py` & `fiddle-0.2.9/fiddle/experimental/auto_config_policy.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/experimental/autobuilders/__init__.py` & `fiddle-0.2.9/fiddle/experimental/autobuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/experimental/configurator.py` & `fiddle-0.2.9/fiddle/experimental/configurator.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/experimental/dict_config.py` & `fiddle-0.2.9/fiddle/experimental/dict_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/experimental/namespace_config.py` & `fiddle-0.2.9/fiddle/experimental/namespace_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/experimental/serialization.py` & `fiddle-0.2.9/fiddle/experimental/serialization.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/experimental/transform.py` & `fiddle-0.2.9/fiddle/experimental/transform.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/experimental/visualize.py` & `fiddle-0.2.9/fiddle/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/experimental/yaml_serialization.py` & `fiddle-0.2.9/fiddle/experimental/yaml_serialization.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/extensions/__init__.py` & `fiddle-0.2.9/fiddle/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/extensions/jax.py` & `fiddle-0.2.9/fiddle/extensions/jax.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/extensions/seqio.py` & `fiddle-0.2.9/fiddle/extensions/seqio.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/extensions/tf.py` & `fiddle-0.2.9/fiddle/extensions/tf.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/graphviz.py` & `fiddle-0.2.9/fiddle/graphviz.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/history.py` & `fiddle-0.2.9/fiddle/history.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/printing.py` & `fiddle-0.2.9/fiddle/printing.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/selectors.py` & `fiddle-0.2.9/fiddle/selectors.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/signatures.py` & `fiddle-0.2.9/fiddle/signatures.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/tag_type.py` & `fiddle-0.2.9/fiddle/tag_type.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/tagging.py` & `fiddle-0.2.9/fiddle/tagging.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/testing/__init__.py` & `fiddle-0.2.9/fiddle/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/testing/autotest.py` & `fiddle-0.2.9/fiddle/testing/autotest.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/testing/test_util.py` & `fiddle-0.2.9/fiddle/testing/test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.8/fiddle/version.py` & `fiddle-0.2.9/fiddle/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Current Fiddle version at head on Github."""
-__version__ = "0.2.8"
+__version__ = "0.2.9"
```

### Comparing `fiddle-0.2.8/fiddle.egg-info/PKG-INFO` & `fiddle-0.2.9/fiddle.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddle
-Version: 0.2.8
+Version: 0.2.9
 Summary: Fiddle: A Python-first configuration library
 Home-page: https://github.com/google/fiddle
 Author: The Fiddle Team
 Author-email: noreply@google.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/google/fiddle/docs
 Project-URL: Bug Reports, https://github.com/google/fiddle/issues
```

### Comparing `fiddle-0.2.8/fiddle.egg-info/SOURCES.txt` & `fiddle-0.2.9/fiddle.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 fiddle/_src/config_test.py
 fiddle/_src/daglish.py
 fiddle/_src/daglish_extensions.py
 fiddle/_src/daglish_extensions_test.py
 fiddle/_src/daglish_test.py
 fiddle/_src/diffing.py
 fiddle/_src/diffing_test.py
-fiddle/_src/field_metadata.py
 fiddle/_src/graphviz.py
 fiddle/_src/graphviz_custom_object.py
 fiddle/_src/history.py
 fiddle/_src/history_test.py
 fiddle/_src/materialize.py
 fiddle/_src/materialize_test.py
 fiddle/_src/module_reflection.py
@@ -57,15 +56,17 @@
 fiddle/_src/signatures_test_helper.py
 fiddle/_src/tag_type.py
 fiddle/_src/tagging.py
 fiddle/_src/tagging_test.py
 fiddle/_src/tagging_test_module.py
 fiddle/_src/absl_flags/__init__.py
 fiddle/_src/absl_flags/flags.py
+fiddle/_src/absl_flags/legacy_flags.py
 fiddle/_src/absl_flags/sample_module_for_flags_test.py
+fiddle/_src/absl_flags/utils.py
 fiddle/_src/codegen/__init__.py
 fiddle/_src/codegen/codegen_diff.py
 fiddle/_src/codegen/formatting_utilities.py
 fiddle/_src/codegen/import_manager.py
 fiddle/_src/codegen/import_manager_test.py
 fiddle/_src/codegen/legacy_codegen.py
 fiddle/_src/codegen/legacy_codegen_test.py
@@ -117,14 +118,17 @@
 fiddle/_src/experimental/configurator.py
 fiddle/_src/experimental/daglish_legacy.py
 fiddle/_src/experimental/daglish_legacy_test.py
 fiddle/_src/experimental/dataclasses.py
 fiddle/_src/experimental/dataclasses_test.py
 fiddle/_src/experimental/dict_config.py
 fiddle/_src/experimental/dict_config_test.py
+fiddle/_src/experimental/lazy_imports.py
+fiddle/_src/experimental/lazy_imports_test.py
+fiddle/_src/experimental/lazy_imports_test_example.py
 fiddle/_src/experimental/namespace_config.py
 fiddle/_src/experimental/namespace_config_test.py
 fiddle/_src/experimental/serialization.py
 fiddle/_src/experimental/transform.py
 fiddle/_src/experimental/transform_test.py
 fiddle/_src/experimental/visualize.py
 fiddle/_src/experimental/with_tags.py
@@ -168,14 +172,15 @@
 fiddle/examples/colabs/__init__.py
 fiddle/experimental/__init__.py
 fiddle/experimental/auto_config.py
 fiddle/experimental/auto_config_policy.py
 fiddle/experimental/configurator.py
 fiddle/experimental/dataclasses.py
 fiddle/experimental/dict_config.py
+fiddle/experimental/lazy_imports.py
 fiddle/experimental/namespace_config.py
 fiddle/experimental/serialization.py
 fiddle/experimental/transform.py
 fiddle/experimental/visualize.py
 fiddle/experimental/yaml_serialization.py
 fiddle/experimental/autobuilders/__init__.py
 fiddle/extensions/__init__.py
```

### Comparing `fiddle-0.2.8/setup.py` & `fiddle-0.2.9/setup.py`

 * *Files identical despite different names*

