# Comparing `tmp/openllm-0.2.0.tar.gz` & `tmp/openllm-0.2.1.tar.gz`

## Comparing `openllm-0.2.0.tar` & `openllm-0.2.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 openllm-0.2.0/.DS_Store
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.0/.gitattributes
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 openllm-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.0/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0    12013 2020-02-02 00:00:00.000000 openllm-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.0/CITATION.cff
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.0/DEVELOPMENT.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.0/nightly-requirements-gpu.txt
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.0/nightly-requirements.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.0/package.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.0/pyoxidizer.bzl
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.0/taplo.toml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/__about__.py
--rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/__main__.py
--rw-r--r--   0        0        0    90069 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/_configuration.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/_generation.py
--rw-r--r--   0        0        0    66372 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/_llm.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/_prompt.py
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/_quantisation.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/_schema.py
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/_service.py
--rw-r--r--   0        0        0    18572 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/_strategies.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/_types.py
--rw-r--r--   0        0        0    97622 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/cli.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/client.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/py.typed
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/testing.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/bundle/__init__.py
--rw-r--r--   0        0        0    14378 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/bundle/_package.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/bundle/oci/Dockerfile-builder
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/bundle/oci/Dockerfile-vllm
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/bundle/oci/__init__.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/auto/modeling_vllm_auto.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/baichuan/__init__.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/baichuan/configuration_baichuan.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/baichuan/modeling_baichuan.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/gpt_neox/configuration_gpt_neox.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/gpt_neox/modeling_gpt_neox.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/llama/configuration_llama.py
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/llama/modeling_llama.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/llama/modeling_vllm_llama.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/mpt/__init__.py
--rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/mpt/configuration_mpt.py
--rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/mpt/modeling_mpt.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/opt/__init__.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/opt/configuration_opt.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/opt/modeling_flax_opt.py
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/opt/modeling_opt.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/opt/modeling_tf_opt.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/playground/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/playground/__init__.py
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/playground/_meta.yml
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/playground/falcon_tuned.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/playground/features.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/playground/opt_tuned.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/serialisation/__init__.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/serialisation/constants.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/serialisation/ggml.py
--rw-r--r--   0        0        0    16729 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/serialisation/transformers.py
--rw-r--r--   0        0        0    16991 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0    11276 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    19990 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/dummy_pt_and_triton_objects.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/dummy_vllm_objects.py
--rw-r--r--   0        0        0    20414 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm/utils/representation.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.0/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/client_test.py
--rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/configuration_test.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/llm_test.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/models_test.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/package_test.py
--rw-r--r--   0        0        0    10402 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/strategies_test.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/models/__init__.py
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/models/conftest.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/models/flan_t5_test.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/models/opt_test.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.0/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.0/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.0/LICENSE.md
--rw-r--r--   0        0        0    24685 2020-02-02 00:00:00.000000 openllm-0.2.0/README.md
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 openllm-0.2.0/hatch.toml
--rw-r--r--   0        0        0    10577 2020-02-02 00:00:00.000000 openllm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 openllm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 openllm-0.2.1/.DS_Store
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.1/.gitattributes
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 openllm-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.1/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0    12098 2020-02-02 00:00:00.000000 openllm-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.1/CITATION.cff
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.1/DEVELOPMENT.md
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.1/nightly-requirements-gpu.txt
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.1/nightly-requirements.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.1/package.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.1/pyoxidizer.bzl
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.1/taplo.toml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/__about__.py
+-rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/__main__.py
+-rw-r--r--   0        0        0    90069 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_configuration.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_generation.py
+-rw-r--r--   0        0        0    67199 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_llm.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_quantisation.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_schema.py
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_service.py
+-rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_strategies.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_types.py
+-rw-r--r--   0        0        0   101301 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/cli.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/client.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/py.typed
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/testing.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/bundle/__init__.py
+-rw-r--r--   0        0        0    14379 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/bundle/_package.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/bundle/oci/Dockerfile-builder
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/bundle/oci/Dockerfile-vllm
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/bundle/oci/__init__.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/modeling_vllm_auto.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/baichuan/__init__.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/baichuan/configuration_baichuan.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/baichuan/modeling_baichuan.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/gpt_neox/configuration_gpt_neox.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/gpt_neox/modeling_gpt_neox.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/llama/configuration_llama.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/llama/modeling_llama.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/llama/modeling_vllm_llama.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/mpt/__init__.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/mpt/configuration_mpt.py
+-rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/mpt/modeling_mpt.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/opt/__init__.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/opt/configuration_opt.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/opt/modeling_flax_opt.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/opt/modeling_opt.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/opt/modeling_tf_opt.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/playground/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/playground/__init__.py
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/playground/_meta.yml
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/playground/falcon_tuned.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/playground/features.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/playground/opt_tuned.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/serialisation/__init__.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/serialisation/constants.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/serialisation/ggml.py
+-rw-r--r--   0        0        0    16729 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/serialisation/transformers.py
+-rw-r--r--   0        0        0    16991 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0    11276 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    19990 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_pt_and_triton_objects.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_vllm_objects.py
+-rw-r--r--   0        0        0    20528 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/representation.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/client_test.py
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/configuration_test.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/llm_test.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models_test.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/package_test.py
+-rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/strategies_test.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/__init__.py
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/conftest.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/flan_t5_test.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/opt_test.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.1/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.1/README.md
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 openllm-0.2.1/hatch.toml
+-rw-r--r--   0        0        0    10577 2020-02-02 00:00:00.000000 openllm-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    30137 2020-02-02 00:00:00.000000 openllm-0.2.1/PKG-INFO
```

### Comparing `openllm-0.2.0/.DS_Store` & `openllm-0.2.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/.pre-commit-config.yaml` & `openllm-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/ADDING_NEW_MODEL.md` & `openllm-0.2.1/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/CHANGELOG.md` & `openllm-0.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.2.1](https://github.com/bentoml/openllm/tree/v0.2.1)
+No significant changes.
+
+
 ## [0.2.0](https://github.com/bentoml/openllm/tree/v0.2.0)
 
 ### Features
 
 - Added support for GPTNeoX models. All variants of GPTNeoX, including Dolly-V2
   and StableLM can now also use `openllm start gpt-neox`
```

### Comparing `openllm-0.2.0/CITATION.cff` & `openllm-0.2.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/DEVELOPMENT.md` & `openllm-0.2.1/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/nightly-requirements.txt` & `openllm-0.2.1/nightly-requirements.txt`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/package.json` & `openllm-0.2.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.2.0",
+    "version": "0.2.1",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.2.0/pyoxidizer.bzl` & `openllm-0.2.1/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/__about__.py` & `openllm-0.2.1/src/openllm/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `openllm-0.2.0/src/openllm/__init__.py` & `openllm-0.2.1/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/__main__.py` & `openllm-0.2.1/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/_configuration.py` & `openllm-0.2.1/src/openllm/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/_generation.py` & `openllm-0.2.1/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/_llm.py` & `openllm-0.2.1/src/openllm/_llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         model_version = getattr(config, "_commit_hash", None)
         if model_version is None:
             raise ValueError(
                 f"Internal errors when parsing config for pretrained {model_id} ('commit_hash' not found)"
             )
 
     return bentoml.Tag.from_taglike(
-        f"{model_name if in_docker() and os.getenv('BENTO_PATH') is not None else implementation + '-' + model_name}:{model_version}".strip()
+        f"{model_name if in_docker() and os.getenv('BENTO_PATH') is not None else implementation + '-' + model_name}:{model_version}".strip().lower()
     )
 
 
 @functools.lru_cache(maxsize=128)
 def generate_hash_from_file(f: str, algorithm: t.Literal["md5", "sha1"] = "sha1") -> str:
     """Generate a hash from given file's modification time.
 
@@ -667,14 +667,24 @@
         if model_id is None:
             model_id = first_not_none(
                 cfg_cls.__openllm_env__["model_id_value"], default=cfg_cls.__openllm_default_id__
             )
         if runtime is None:
             runtime = cfg_cls.__openllm_runtime__
 
+        model_id, *maybe_revision = model_id.rsplit(":")
+        if len(maybe_revision) > 0:
+            if model_version is not None:
+                logger.warning(
+                    "revision is specified within 'model_id' (%s), which will override the 'model_version=%s'",
+                    maybe_revision[0],
+                    model_version,
+                )
+            model_version = maybe_revision[0]
+
         # quantization setup
         if quantization_config and quantize:
             raise ValueError(
                 """'quantization_config' and 'quantize' are mutually exclusive. Either customise
             your quantization_config or use the 'quantize' argument."""
             )
         if quantization_config is None and quantize is not None:
@@ -722,24 +732,29 @@
             _tag=_tag,
             _serialisation_format=serialisation,
             **attrs,
         )
 
     @classmethod
     def _infer_tag_from_model_id(cls, model_id: str, model_version: str | None) -> bentoml.Tag:
+        # XXX: Fix me later, if the model is a valid tag, then we return it directly
+        # instead of creating a new tag from the model_id. this branch will be hit during `openllm build`
         try:
-            return bentoml.Tag.from_taglike(model_id)
-        except ValueError:
-            return make_tag(
-                model_id,
-                model_version=model_version,
-                trust_remote_code=cls.config_class.__openllm_trust_remote_code__,
-                implementation=cls.__llm_implementation__,
-                quiet=True,
-            )
+            return bentoml.models.get(model_id).tag
+        except (ValueError, bentoml.exceptions.BentoMLException):
+            try:
+                return bentoml.Tag.from_taglike(model_id)
+            except (ValueError, bentoml.exceptions.BentoMLException):
+                return make_tag(
+                    model_id,
+                    model_version=model_version,
+                    trust_remote_code=cls.config_class.__openllm_trust_remote_code__,
+                    implementation=cls.__llm_implementation__,
+                    quiet=True,
+                )
 
     def __init__(
         self,
         *args: t.Any,
         model_id: str,
         llm_config: openllm.LLMConfig,
         bettertransformer: bool | None,
```

### Comparing `openllm-0.2.0/src/openllm/_prompt.py` & `openllm-0.2.1/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/_quantisation.py` & `openllm-0.2.1/src/openllm/_quantisation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/_schema.py` & `openllm-0.2.1/src/openllm/_schema.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/_service.py` & `openllm-0.2.1/src/openllm/_service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/_strategies.py` & `openllm-0.2.1/src/openllm/_strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,34 +20,31 @@
 import sys
 import types
 import typing as t
 import warnings
 
 import psutil
 
-from bentoml._internal.resource import Resource
+import bentoml
 from bentoml._internal.resource import get_resource
 from bentoml._internal.resource import system_resources
 from bentoml._internal.runner.strategy import THREAD_ENVS
-from bentoml._internal.runner.strategy import Strategy
 
 from .utils import LazyType
 from .utils import ReprMixin
 
 
 if t.TYPE_CHECKING:
-    import bentoml
-
     ListIntStr = list[int | str]
 
-    class DynResource(Resource[t.List[str]], resource_id=""):
+    class DynResource(bentoml.Resource[t.List[str]], resource_id=""):
         resource_id: t.ClassVar[str]
 
 else:
-    DynResource = Resource[t.List[str]]
+    DynResource = bentoml.Resource[t.List[str]]
     ListIntStr = list
 
 # NOTE: We need to do this so that overload can register
 # correct overloads to typing registry
 if sys.version_info[:2] >= (3, 11):
     from typing import overload
 else:
@@ -325,15 +322,15 @@
     """AMD GPU resource.
 
     Since ROCm will respect CUDA_VISIBLE_DEVICES, the behaviour of from_spec, from_system are similar to
     ``NvidiaGpuResource``. Currently ``validate`` is not yet supported.""",
 )
 
 
-class CascadingResourceStrategy(Strategy, ReprMixin):
+class CascadingResourceStrategy(bentoml.Strategy, ReprMixin):
     """This is extends the default BentoML strategy where we check for NVIDIA GPU resource -> AMD GPU resource -> CPU resource.
 
     It also respect CUDA_VISIBLE_DEVICES for both AMD and NVIDIA GPU.
     See https://rocm.docs.amd.com/en/develop/understand/gpu_isolation.html#cuda-visible-devices
     for ROCm's support for CUDA_VISIBLE_DEVICES.
 
     TODO: Support CloudTPUResource
```

### Comparing `openllm-0.2.0/src/openllm/_types.py` & `openllm-0.2.1/src/openllm/_types.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/cli.py` & `openllm-0.2.1/src/openllm/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 import subprocess
 import sys
 import tempfile
 import time
 import traceback
 import typing as t
 
+import attr
 import click
 import click_option_group as cog
 import fs
 import fs.errors
 import inflection
 import orjson
 import psutil
@@ -66,14 +67,15 @@
 import openllm
 from bentoml._internal.configuration.containers import BentoMLContainer
 from bentoml._internal.models.model import ModelStore
 
 from .__about__ import __version__
 from .exceptions import OpenLLMException
 from .utils import DEBUG
+from .utils import ENV_VARS_TRUE_VALUES
 from .utils import EnvVarMixin
 from .utils import LazyLoader
 from .utils import LazyType
 from .utils import analytics
 from .utils import bentoml_cattr
 from .utils import codegen
 from .utils import configure_logging
@@ -169,15 +171,15 @@
     call = click.echo
     if _with_style:
         attrs["fg"] = fg if not get_debug_mode() else None
         call = click.secho
     call(text, **attrs)
 
 
-output_option: t.Callable[[FC], FC] = click.option(
+output_option: t.Callable[[_AnyCallable], _AnyCallable] = click.option(
     "-o",
     "--output",
     type=click.Choice(["json", "pretty", "porcelain"]),
     default="pretty",
     help="Showing output type.",
     show_default=True,
     envvar="OPENLLM_OUTPUT",
@@ -195,14 +197,23 @@
         default=None,
         help="Optional model_id name or path for (fine-tune) weight.",
         envvar=envvar,
         show_envvar=True if envvar is not None else False,
     )
 
 
+def model_version_option(factory: t.Any) -> t.Callable[[FC], FC]:
+    return factory.option(
+        "--model-version",
+        type=click.STRING,
+        default=None,
+        help="Optional model version to save for this model. It will be inferred automatically from model-id.",
+    )
+
+
 def workers_per_resource_option(factory: t.Any, build: bool = False) -> t.Callable[[FC], FC]:
     help_str = """Number of workers per resource assigned.
     See https://docs.bentoml.org/en/latest/guides/scheduling.html#resource-scheduling-strategy
     for more information. By default, this is set to 1.
 
     **Note**: ``--workers-per-resource`` will also accept the following strategies:
 
@@ -291,44 +302,69 @@
             adapter_id = resolve_user_filepath(adapter_id, os.getcwd())
         except FileNotFoundError:
             pass
         ctx.params[_adapter_mapping_key][adapter_id] = adapter_name[0] if len(adapter_name) > 0 else None
     return None
 
 
+@attr.define
+class CliContext:
+    cloud_context: str | None = attr.field(default=None, converter=attr.converters.default_if_none("default"))
+
+    def with_options(self, **attrs: t.Any) -> t.Self:
+        return attr.evolve(self, **attrs)
+
+
 class OpenLLMCommandGroup(BentoMLCommandGroup):
-    NUMBER_OF_COMMON_PARAMS = 4  # parameters in common_params + 1 faked group option header
+    NUMBER_OF_COMMON_PARAMS = 5  # parameters in common_params + 1 faked group option header
 
     @staticmethod
     def common_params(f: FC) -> t.Callable[[FC], FC]:
         """This is not supposed to be used with unprocessed click function.
 
         This should be used a the last currying from common_params -> usage_tracking -> exception_handling.
         """
         # The following logics is similar to one of BentoMLCommandGroup
 
         from bentoml._internal.configuration import DEBUG_ENV_VAR
         from bentoml._internal.configuration import QUIET_ENV_VAR
 
-        @cog.optgroup.group("Miscellaneous options")
+        @cog.optgroup.group("Global options")
         @cog.optgroup.option(
             "-q", "--quiet", envvar=QUIET_ENV_VAR, is_flag=True, default=False, help="Suppress all output."
         )
         @cog.optgroup.option(
-            "--debug", "--verbose", envvar=DEBUG_ENV_VAR, is_flag=True, default=False, help="Print out debug logs."
+            "--debug",
+            "--verbose",
+            "debug",
+            envvar=DEBUG_ENV_VAR,
+            is_flag=True,
+            default=False,
+            help="Print out debug logs.",
         )
         @cog.optgroup.option(
             "--do-not-track",
             is_flag=True,
             default=False,
             envvar=analytics.OPENLLM_DO_NOT_TRACK,
             help="Do not send usage info",
         )
+        @cog.optgroup.option(
+            "--context",
+            "cloud_context",
+            type=click.STRING,
+            default=None,
+            help="BentoCloud context name.",
+        )
+        @click.pass_context
         @functools.wraps(f)
-        def wrapper(quiet: bool, debug: bool, *args: P.args, **attrs: P.kwargs) -> t.Any:
+        def wrapper(
+            ctx: click.Context, quiet: bool, debug: bool, cloud_context: str | None, *args: P.args, **attrs: P.kwargs
+        ) -> t.Any:
+            ctx.obj = CliContext(cloud_context=cloud_context)
             if quiet:
                 set_quiet_mode(True)
                 if debug:
                     logger.warning("'--quiet' passed; ignoring '--verbose/--debug'")
             elif debug:
                 set_debug_mode(True)
 
@@ -528,16 +564,20 @@
         f"Start a {'HTTP' if not serve_grpc else 'gRPC'} server options",
         help=f"Related to serving the model [synonymous to `bentoml {'serve-http' if not serve_grpc else command }`]",
     )
 
     def decorator(f: t.Callable[t.Concatenate[int, str | None, P], openllm.LLMConfig]):
         serve_command = cli.commands[command]
         # The first variable is the argument bento
-        # and the last three are shared default, which we don't need.
-        serve_options = [p for p in serve_command.params[1:-3] if p.name not in _IGNORED_OPTIONS]
+        # The last five is from BentoMLCommandGroup.NUMBER_OF_COMMON_PARAMS
+        serve_options = [
+            p
+            for p in serve_command.params[1 : -BentoMLCommandGroup.NUMBER_OF_COMMON_PARAMS]
+            if p.name not in _IGNORED_OPTIONS
+        ]
         for options in reversed(serve_options):
             attrs = options.to_info_dict()
             # we don't need param_type_name, since it should all be options
             attrs.pop("param_type_name")
             # name is not a valid args
             attrs.pop("name")
             # type can be determine from default value
@@ -565,14 +605,15 @@
             "--server-timeout",
             type=int,
             default=None,
             help="Server timeout in seconds",
         ),
         workers_per_resource_option(cog.optgroup),
         model_id_option(cog.optgroup, model_env=llm_config["env"]),
+        model_version_option(cog.optgroup),
         cog.optgroup.option(
             "--fast",
             is_flag=True,
             default=False,
             help="Bypass auto model checks and setup. This option is ahead-of-serving time.",
         ),
         cog.optgroup.group(
@@ -726,18 +767,20 @@
             short_help=f"Start a LLMServer for '{model_name_or_bento}'",
             aliases=[llm_config["start_name"]] if llm_config["name_type"] == "dasherize" else None,
             help=f"""\
 {llm_config['env'].start_docstring}
 
 \b
 Note: ``{llm_config['start_name']}`` can also be run with any other models available on HuggingFace
-or fine-tuned variants as long as it belongs to the architecture generation ``{llm_config['architecture']}`` (trust_remote_code={llm_config['trust_remote_code']}). For example:
+or fine-tuned variants as long as it belongs to the architecture generation ``{llm_config['architecture']}`` (trust_remote_code={llm_config['trust_remote_code']}).
+
+\b
+For example: One can start [Fastchat-T5](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0) with ``openllm start flan-t5``:
 
 \b
-Start [Fastchat-T5](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0) with ``openllm start flan-t5``:
 $ openllm start flan-t5 --model-id lmsys/fastchat-t5-3b-v1.0
 
 \b
 Available official model_id(s): [default: {llm_config['default_id']}]
 
 \b
 {orjson.dumps(llm_config['model_ids'], option=orjson.OPT_INDENT_2).decode()}
@@ -885,14 +928,15 @@
     @group.command(**command_attrs)
     @start_decorator(llm_config, serve_grpc=serve_grpc)
     @click.pass_context
     def start_cmd(
         ctx: click.Context,
         server_timeout: int,
         model_id: str | None,
+        model_version: str | None,
         workers_per_resource: t.LiteralString | float,
         device: tuple[str, ...],
         quantize: t.Literal["int8", "int4", "gptq"] | None,
         bettertransformer: bool | None,
         runtime: t.Literal["ggml", "transformers"],
         fast: bool,
         adapter_id: str | None,
@@ -1033,25 +1077,32 @@
     @group.command(**command_attrs)
     @start_decorator(llm_config, serve_grpc=serve_grpc)
     @click.pass_context
     def start_cmd(
         ctx: click.Context,
         server_timeout: int,
         model_id: str | None,
+        model_version: str | None,
         workers_per_resource: t.LiteralString | float,
         device: tuple[str, ...],
         quantize: t.Literal["int8", "int4", "gptq"] | None,
         bettertransformer: bool | None,
         runtime: t.Literal["ggml", "transformers"],
         fast: bool,
         serialisation_format: t.Literal["safetensors", "legacy"],
         adapter_id: str | None,
         return_process: bool,
         **attrs: t.Any,
     ) -> openllm.LLMConfig | subprocess.Popen[bytes]:
+        if serialisation_format == "safetensors" and quantize is not None:
+            if os.getenv("OPENLLM_SERIALIZATION_WARNING", str(True)).upper() in ENV_VARS_TRUE_VALUES:
+                _echo(
+                    f"'--quantize={quantize}' might not work with 'safetensors' serialisation format. Use with caution!. To silence this warning, set \"OPENLLM_SERIALIZATION_WARNING=True\"\nNote: You can always fallback to '--serialisation legacy' when running quantisation.",
+                    fg="yellow",
+                )
         adapter_map: dict[str, str | None] | None = attrs.pop(_adapter_mapping_key, None)
 
         config, server_attrs = llm_config.model_validate_click(**attrs)
         server_timeout = first_not_none(server_timeout, default=config["timeout"])
 
         server_attrs.update({"working_dir": os.path.dirname(__file__), "timeout": server_timeout})
         if serve_grpc:
@@ -1114,14 +1165,15 @@
 
         if adapter_map:
             _echo(f"OpenLLM will convert '{model_name}' to use provided adapters layers: {list(adapter_map)}")
 
         llm = openllm.infer_auto_class(env.framework_value).for_model(
             model_name,
             model_id=model_id,
+            model_version=model_version,
             llm_config=config,
             ensure_available=not fast,
             return_runner_kwargs=False,
             quantize=quantize,
             bettertransformer=bettertransformer,
             adapter_map=adapter_map,
             runtime=runtime,
@@ -1211,20 +1263,15 @@
     "model_id",
     type=click.STRING,
     default=None,
     metavar="Optional[REMOTE_REPO/MODEL_ID | /path/to/local/model]",
     required=False,
 )
 @click.argument("converter", envvar="CONVERTER", type=click.STRING, default=None, required=False, metavar=None)
-@click.option(
-    "--model-version",
-    type=click.STRING,
-    default=None,
-    help="Optional model version to save for this model. It will be inferred automatically from model-id.",
-)
+@model_version_option(click)
 @click.option(
     "--runtime",
     type=click.Choice(["ggml", "transformers"]),
     default="transformers",
     help="The runtime to use for the given model. Default is transformers.",
 )
 @output_option
@@ -1760,20 +1807,15 @@
     "--adapter-id",
     default=None,
     help="Optional adapters id to be included within the Bento. Note that if you are using relative path, '--build-ctx' must be passed.",
     multiple=True,
     metavar="[PATH | [remote/][adapter_name:]adapter_id][, ...]",
 )
 @click.option("--build-ctx", default=".", help="Build context. This is required if --adapter-id uses relative path")
-@click.option(
-    "--model-version",
-    default=None,
-    type=click.STRING,
-    help="Model version provided for this 'model-id' if it is a custom path.",
-)
+@model_version_option(click)
 @click.option(
     "--dockerfile-template",
     default=None,
     type=click.File(),
     help="Optional custom dockerfile template to be used with this BentoLLM.",
 )
 @serialisation_option(click)
@@ -1977,15 +2019,15 @@
     elif output == "json":
         _echo(orjson.dumps(bento.info.to_dict(), option=orjson.OPT_INDENT_2).decode())
     else:
         _echo(bento.tag)
 
     if push:
         client = BentoMLContainer.bentocloud_client.get()
-        client.push_bento(bento)
+        client.push_bento(bento, context=t.cast(CliContext, ctx.obj).cloud_context)
     elif containerize:
         backend = t.cast("DefaultBuilder", os.getenv("BENTOML_CONTAINERIZE_BACKEND", "docker"))
         _echo(f"Building {bento} into a LLMContainer using backend '{backend}'", fg="magenta")
         try:
             bentoml.container.health(backend)
         except subprocess.CalledProcessError:
             raise OpenLLMException(f"Failed to use backend {backend}") from None
@@ -2205,27 +2247,44 @@
                 ).decode(),
                 fg="white",
             )
     ctx.exit(0)
 
 
 @cli.command()
+@click.argument(
+    "model_name",
+    type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]),
+    required=False,
+)
 @click.option(
     "-y",
     "--yes",
     "--assume-yes",
     is_flag=True,
     help="Skip confirmation when deleting a specific model",
 )
 @inject
-def prune_command(yes: bool, model_store: ModelStore = Provide[BentoMLContainer.model_store]) -> None:
-    """Remove all saved models locally."""
+def prune_command(
+    model_name: str | None, yes: bool, model_store: ModelStore = Provide[BentoMLContainer.model_store]
+) -> None:
+    """Remove all saved models locally.
+
+    \b
+    If a model type is passed, then only prune models for that given model type.
+    """
     available = [
         m for m in bentoml.models.list() if "framework" in m.info.labels and m.info.labels["framework"] == "openllm"
     ]
+    if model_name is not None:
+        available = [
+            m
+            for m in available
+            if "model_name" in m.info.labels and m.info.labels["model_name"] == inflection.underscore(model_name)
+        ]
 
     for model in available:
         if yes:
             delete_confirmed = True
         else:
             delete_confirmed = click.confirm(f"delete model {model.tag}?")
 
@@ -2369,36 +2428,77 @@
         endpoint = re.sub(r"http://", "", endpoint)
     client = (
         openllm.client.HTTPClient(endpoint, timeout=timeout)
         if server_type == "http"
         else openllm.client.GrpcClient(endpoint, timeout=timeout)
     )
 
-    input_fg = "yellow"
+    input_fg = "magenta"
     generated_fg = "cyan"
 
     if output != "porcelain":
         _echo("Input prompt: ", nl=False, fg="white")
-        _echo(f"{prompt}", fg="magenta", nl=False)
+        _echo(f"{prompt}", fg=input_fg, nl=False)
 
     res = client.query(prompt, return_raw_response=True)
 
     if output == "pretty":
-        formatted = client.llm.postprocess_generate(prompt, res["responses"])
+        full_formatted = client.llm.postprocess_generate(prompt, res["responses"])
+        response = full_formatted[len(prompt) + 1 :]
         _echo("\n\n==Responses==\n", fg="white")
         _echo(f"{prompt} ", fg=input_fg, nl=False)
-        _echo(formatted, fg=generated_fg)
+        _echo(response, fg=generated_fg)
     elif output == "json":
         _echo(orjson.dumps(res, option=orjson.OPT_INDENT_2).decode(), fg="white")
     else:
         _echo(res["responses"], fg="white")
 
     ctx.exit(0)
 
 
+@cli.group(name="utils")
+def utils_command() -> None:
+    """Utilities Subcommand group."""
+
+
+@utils_command.command()
+@click.argument(
+    "model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()])
+)
+@click.argument("prompt", type=click.STRING)
+@output_option
+@click.option("--format", type=click.STRING, default=None)
+def get_prompt(model_name: str, prompt: str, format: str | None, output: OutputLiteral):
+    """Get the default prompt used by OpenLLM."""
+    try:
+        module = openllm.utils.EnvVarMixin(model_name).module
+        template = module.DEFAULT_PROMPT_TEMPLATE
+        if callable(template):
+            if format is None:
+                raise click.BadOptionUsage(
+                    "format",
+                    f"{model_name} prompt requires passing '--format' (available format: {module.PROMPT_MAPPING})",
+                )
+            _prompt = template(format)
+        else:
+            _prompt = template
+
+        fully_formatted = _prompt.format(instruction=prompt)
+
+        if output == "porcelain":
+            _echo(f'__prompt__:"{fully_formatted}"', fg="white")
+        elif output == "json":
+            _echo(orjson.dumps({"prompt": fully_formatted}, option=orjson.OPT_INDENT_2).decode(), fg="white")
+        else:
+            _echo(f"== Prompt for {model_name} ==\n", fg="magenta")
+            _echo(fully_formatted, fg="white")
+    except AttributeError:
+        raise click.ClickException(f"{model_name} does not have default prompt template.") from None
+
+
 def load_notebook_metadata() -> DictStrAny:
     with open(os.path.join(os.path.dirname(openllm.playground.__file__), "_meta.yml"), "r") as f:
         content = yaml.safe_load(f)
     if not all("description" in k for k in content.values()):
         raise ValueError("Invalid metadata file. All entries must have a 'description' key.")
     return content
```

### Comparing `openllm-0.2.0/src/openllm/client.py` & `openllm-0.2.1/src/openllm/client.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/exceptions.py` & `openllm-0.2.1/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/testing.py` & `openllm-0.2.1/src/openllm/testing.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/bundle/__init__.py` & `openllm-0.2.1/src/openllm/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/bundle/_package.py` & `openllm-0.2.1/src/openllm/bundle/_package.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         packages.extend([handle_package_version("torch", has_dockerfile_template)])
 
     wheels: list[str] = []
     built_wheels = build_editable(llm_fs.getsyspath("/"))
     if built_wheels is not None:
         wheels.append(llm_fs.getsyspath(f"/{built_wheels.split('/')[-1]}"))
 
-    return PythonOptions(packages=packages, wheels=wheels, lock_packages=True)
+    return PythonOptions(packages=packages, wheels=wheels, lock_packages=False)
 
 
 def construct_docker_options(
     llm: openllm.LLM[t.Any, t.Any],
     _: FS,
     workers_per_resource: int | float,
     quantize: t.LiteralString | None,
```

### Comparing `openllm-0.2.0/src/openllm/bundle/oci/Dockerfile-builder` & `openllm-0.2.1/src/openllm/bundle/oci/Dockerfile-builder`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/bundle/oci/__init__.py` & `openllm-0.2.1/src/openllm/bundle/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/__init__.py` & `openllm-0.2.1/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/auto/__init__.py` & `openllm-0.2.1/src/openllm/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/auto/configuration_auto.py` & `openllm-0.2.1/src/openllm/models/auto/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/auto/factory.py` & `openllm-0.2.1/src/openllm/models/auto/factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/auto/modeling_auto.py` & `openllm-0.2.1/src/openllm/models/auto/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.2.1/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.2.1/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/auto/modeling_vllm_auto.py` & `openllm-0.2.1/src/openllm/models/auto/modeling_vllm_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/baichuan/__init__.py` & `openllm-0.2.1/src/openllm/models/baichuan/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/baichuan/configuration_baichuan.py` & `openllm-0.2.1/src/openllm/models/baichuan/configuration_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/baichuan/modeling_baichuan.py` & `openllm-0.2.1/src/openllm/models/baichuan/modeling_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/chatglm/__init__.py` & `openllm-0.2.1/src/openllm/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.2.1/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.2.1/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.2.1/src/openllm/models/dolly_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.2.1/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.2.1/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/falcon/__init__.py` & `openllm-0.2.1/src/openllm/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.2.1/src/openllm/models/falcon/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.2.1/src/openllm/models/falcon/modeling_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/flan_t5/__init__.py` & `openllm-0.2.1/src/openllm/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.2.1/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.2.1/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.2.1/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.2.1/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.2.1/src/openllm/models/gpt_neox/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/gpt_neox/configuration_gpt_neox.py` & `openllm-0.2.1/src/openllm/models/gpt_neox/configuration_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/gpt_neox/modeling_gpt_neox.py` & `openllm-0.2.1/src/openllm/models/gpt_neox/modeling_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/llama/__init__.py` & `openllm-0.2.1/src/openllm/models/llama/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,20 @@
 from ...exceptions import MissingDependencyError
 from ...utils import LazyModule
 from ...utils import is_torch_available
 from ...utils import is_vllm_available
 
 
 _import_structure: dict[str, list[str]] = {
-    "configuration_llama": ["LlaMAConfig", "START_LLAMA_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
+    "configuration_llama": [
+        "LlaMAConfig",
+        "START_LLAMA_COMMAND_DOCSTRING",
+        "DEFAULT_PROMPT_TEMPLATE",
+        "PROMPT_MAPPING",
+    ],
 }
 
 try:
     if not is_vllm_available():
         raise MissingDependencyError
 except MissingDependencyError:
     pass
@@ -40,14 +45,15 @@
     pass
 else:
     _import_structure["modeling_llama"] = ["LlaMA"]
 
 
 if t.TYPE_CHECKING:
     from .configuration_llama import DEFAULT_PROMPT_TEMPLATE as DEFAULT_PROMPT_TEMPLATE
+    from .configuration_llama import PROMPT_MAPPING as PROMPT_MAPPING
     from .configuration_llama import START_LLAMA_COMMAND_DOCSTRING as START_LLAMA_COMMAND_DOCSTRING
     from .configuration_llama import LlaMAConfig as LlaMAConfig
 
     try:
         if not is_vllm_available():
             raise MissingDependencyError
     except MissingDependencyError:
```

### Comparing `openllm-0.2.0/src/openllm/models/llama/configuration_llama.py` & `openllm-0.2.1/src/openllm/models/opt/configuration_opt.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,88 +13,84 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import openllm
 
 
-class LlaMAConfig(openllm.LLMConfig):
-    """LLaMA model was proposed in [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/abs/2302.13971) by Hugo Touvron, Thibaut Lavril, Gautier Izacard, Xavier Martinet, Marie-Anne Lachaux, Timothée Lacroix, Baptiste Rozière, Naman Goyal, Eric Hambro, Faisal Azhar, Aurelien Rodriguez, Armand Joulin, Edouard Grave, Guillaume Lample.
+class OPTConfig(openllm.LLMConfig):
+    """OPT was first introduced in [Open Pre-trained Transformer Language Models](https://arxiv.org/abs/2205.01068) and first released in [metaseq's repository](https://github.com/facebookresearch/metaseq) on May 3rd 2022 by Meta AI.
 
-    It is a collection of foundation language models ranging from 7B to 65B parameters.
+    OPT was predominantly pretrained with English text, but a small amount of non-English data is still present
+    within the training corpus via CommonCrawl. The model was pretrained using a causal language modeling (CLM)
+    objective. OPT belongs to the same family of decoder-only models like GPT-3. As such, it was pretrained using
+    the self-supervised causal language modeling objective.
 
-    LlaMA also include support for the recent propsed [LlaMA-2](https://ai.meta.com/research/publications/llama-2-open-foundation-and-fine-tuned-chat-models/)
-
-    Note that all variants of LlaMA including fine-tuning, quantisation format are all supported with ``openllm.LlaMA``.
-
-    Refer to [LlaMA's model card](https://huggingface.co/docs/transformers/main/model_doc/llama)
-    for more information.
+    Refer to [OPT's HuggingFace page](https://huggingface.co/docs/transformers/model_doc/opt) for more information.
     """
 
     __config__ = {
-        "model_name": "llama",
-        "start_name": "llama",
-        "url": "https://github.com/facebookresearch/llama",
-        "default_id": "huggyllama/llama-7b",
-        "default_implementation": "pt",  # XXX: needs vLLM implementation
-        "architecture": "LlamaForCausalLM",
-        "requirements": ["openllm[vllm]", "fairscale", "sentencepiece"],
+        "name_type": "lowercase",
+        "trust_remote_code": False,
+        "url": "https://huggingface.co/docs/transformers/model_doc/opt",
+        "default_id": "facebook/opt-1.3b",
+        "architecture": "MPTForCausalLM",
         "model_ids": [
-            "meta-llama/llama-2-70b-chat-hf",
-            "meta-llama/llama-2-13b-chat-hf",
-            "meta-llama/llama-2-7b-chat-hf",
-            "meta-llama/llama-2-70b-hf",
-            "meta-llama/llama-2-13b-hf",
-            "meta-llama/llama-2-7b-hf",
-            "openlm-research/open_llama_7b_v2",
-            "openlm-research/open_llama_3b_v2",
-            "openlm-research/open_llama_13b",
-            "huggyllama/llama-65b",
-            "huggyllama/llama-30b",
-            "huggyllama/llama-13b",
-            "huggyllama/llama-7b",
+            "facebook/opt-125m",
+            "facebook/opt-350m",
+            "facebook/opt-1.3b",
+            "facebook/opt-2.7b",
+            "facebook/opt-6.7b",
+            "facebook/opt-66b",
         ],
-        "tokenizer_class": "LlamaTokenizerFast",
+        "fine_tune_strategies": (
+            {
+                "adapter_type": "lora",
+                "r": 16,
+                "lora_alpha": 32,
+                "target_modules": ["q_proj", "v_proj"],
+                "lora_dropout": 0.05,
+                "bias": "none",
+            },
+        ),
     }
 
-    class GenerationConfig:
-        max_new_tokens: int = 256
-        temperature: float = 0.8
-        top_p: float = 0.95
+    format_outputs: bool = openllm.LLMConfig.Field(
+        False,
+        description="""Whether to format the outputs. This
+    can be used when num_return_sequences > 1.""",
+    )
 
-    class SamplingParams:
-        best_of: int = 1
-        presence_penalty: float = 0.5
+    class GenerationConfig:
+        top_k: int = 15
+        temperature: float = 0.75
+        max_new_tokens: int = 1024
+        num_return_sequences: int = 1
 
 
-START_LLAMA_COMMAND_DOCSTRING = """\
-Run a LLMServer for LlaMA model.
+START_OPT_COMMAND_DOCSTRING = """\
+Run a LLMServer for OPT model.
 
 \b
-> See more information about LlaMA at [LlaMA's model card](https://huggingface.co/docs/transformers/main/model_doc/llama
+> See more information about falcon at [facebook/opt-66b](https://huggingface.co/facebook/opt-66b)
 
 \b
 ## Usage
 
-By default, this model will use [vLLM](https://github.com/vllm-project/vllm) for inference.
-This model will also supports PyTorch.
+By default, this model will use the PyTorch model for inference. However, this model supports both Flax and Tensorflow.
 
 \b
-- To use PyTorch, set the environment variable ``OPENLLM_LLAMA_FRAMEWORK="pt"``
+- To use Flax, set the environment variable ``OPENLLM_OPT_FRAMEWORK="flax"``
 
 \b
-LlaMA Runner will use decapoda-research/llama-7b-hf as the default model. To change to any other LlaMA
-saved pretrained, or a fine-tune LlaMA, provide ``OPENLLM_LLAMA_MODEL_ID='openlm-research/open_llama_7b_v2'``
-or provide `--model-id` flag when running ``openllm start llama``:
+- To use Tensorflow, set the environment variable ``OPENLLM_OPT_FRAMEWORK="tf"``
 
 \b
-$ openllm start llama --model-id 'openlm-research/open_llama_7b_v2'
+OPT Runner will use facebook/opt-2.7b as the default model. To change to any other OPT
+saved pretrained, or a fine-tune OPT, provide ``OPENLLM_OPT_MODEL_ID='facebook/opt-6.7b'``
+or provide `--model-id` flag when running ``openllm start opt``:
 
 \b
-OpenLLM also supports running LlaMA-2 and its fine-tune and variants. To import the LlaMA weights, one can use the following:
-
-\b
-$ CONVERTER=hf-llama2 openllm import llama /path/to/llama-2
+$ openllm start opt --model-id facebook/opt-6.7b
 """
 
-
 DEFAULT_PROMPT_TEMPLATE = """{instruction}"""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openllm-0.2.0/src/openllm/models/llama/modeling_llama.py` & `openllm-0.2.1/src/openllm/models/llama/modeling_llama.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,39 +42,47 @@
 
     def llm_post_init(self):
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     def sanitize_parameters(
         self,
         prompt: str,
+        top_k: int | None = None,
         top_p: float | None = None,
         temperature: float | None = None,
         max_new_tokens: int | None = None,
         use_default_prompt_template: bool = True,
+        use_llama2_prompt: bool = True,
         **attrs: t.Any,
     ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
         if use_default_prompt_template:
-            template_variables = default_formatter.extract_template_variables(DEFAULT_PROMPT_TEMPLATE)
+            _PROMPT = DEFAULT_PROMPT_TEMPLATE("v2" if use_llama2_prompt else "v1")
+            template_variables = default_formatter.extract_template_variables(_PROMPT)
             prompt_variables = {k: v for k, v in attrs.items() if k in template_variables}
             if "instruction" in prompt_variables:
                 raise RuntimeError(
                     "'instruction' should be passed as the first argument "
                     "instead of kwargs when 'use_default_prompt_template=True'"
                 )
             try:
-                prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
+                prompt_text = _PROMPT.format(instruction=prompt, **prompt_variables)
             except KeyError as e:
                 raise RuntimeError(
                     f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. "
                     "Use 'use_default_prompt_template=False' to disable the default prompt template."
                 ) from None
         else:
             prompt_text = prompt
 
-        generation_config = {"max_new_tokens": max_new_tokens, "temperature": temperature, "top_p": top_p}
+        generation_config = {
+            "max_new_tokens": max_new_tokens,
+            "temperature": temperature,
+            "top_p": top_p,
+            "top_k": top_k,
+        }
 
         return prompt_text, generation_config, {}
 
     @property
     def import_kwargs(self):
         model_kwds = {"device_map": "auto" if torch.cuda.device_count() > 1 else None}
         tokenizer_kwds: dict[str, t.Any] = {}
@@ -83,22 +91,21 @@
     def postprocess_generate(self, prompt: str, generation_result: list[str], **_: t.Any) -> str:
         return generation_result[0]
 
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
         from ..._generation import StopOnTokens
 
         generation_kwargs = {
-            "do_sample": True,
             "generation_config": self.config.model_construct_env(**attrs).to_generation_config(),
             "stopping_criteria": transformers.StoppingCriteriaList([StopOnTokens()]),
         }
 
         inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
         with torch.inference_mode():
-            gen_tokens = self.model.generate(inputs.input_ids, **generation_kwargs)
+            gen_tokens = self.model.generate(**inputs, **generation_kwargs)
             return self.tokenizer.batch_decode(gen_tokens, skip_special_tokens=True, clean_up_tokenization_spaces=True)
 
     def embeddings(self, prompts: list[str]) -> LLMEmbeddings:
         encoding = self.tokenizer(prompts, padding=True, return_tensors="pt").to(self.device)
         input_ids = encoding["input_ids"]
         attention_mask = encoding["attention_mask"]
         with torch.inference_mode():
```

### Comparing `openllm-0.2.0/src/openllm/models/llama/modeling_vllm_llama.py` & `openllm-0.2.1/src/openllm/models/llama/modeling_vllm_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/mpt/__init__.py` & `openllm-0.2.1/src/openllm/models/mpt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,28 +17,29 @@
 
 from ...exceptions import MissingDependencyError
 from ...utils import LazyModule
 from ...utils import is_torch_available
 
 
 _import_structure: dict[str, list[str]] = {
-    "configuration_mpt": ["MPTConfig", "START_MPT_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
+    "configuration_mpt": ["MPTConfig", "START_MPT_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE", "PROMPT_MAPPING"],
 }
 
 try:
     if not is_torch_available():
         raise MissingDependencyError
 except MissingDependencyError:
     pass
 else:
     _import_structure["modeling_mpt"] = ["MPT"]
 
 
 if t.TYPE_CHECKING:
     from .configuration_mpt import DEFAULT_PROMPT_TEMPLATE as DEFAULT_PROMPT_TEMPLATE
+    from .configuration_mpt import PROMPT_MAPPING as PROMPT_MAPPING
     from .configuration_mpt import START_MPT_COMMAND_DOCSTRING as START_MPT_COMMAND_DOCSTRING
     from .configuration_mpt import MPTConfig as MPTConfig
 
     try:
         if not is_torch_available():
             raise MissingDependencyError
     except MissingDependencyError:
```

### Comparing `openllm-0.2.0/src/openllm/models/mpt/configuration_mpt.py` & `openllm-0.2.1/src/openllm/models/mpt/configuration_mpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,20 +123,20 @@
 )
 
 _default_prompt = """{instruction}"""
 
 # TODO: XXX implement me
 _chat_prompt = """{instruction}"""
 
-_PROMPT_MAPPING = {
+PROMPT_MAPPING = {
     "default": _default_prompt,
     "instruct": _instruct_prompt,
     "storywriter": _default_prompt,
     "chat": _chat_prompt,
 }
 
 
 def _get_prompt(model_type: str) -> str:
-    return _PROMPT_MAPPING[model_type]
+    return PROMPT_MAPPING[model_type]
 
 
 DEFAULT_PROMPT_TEMPLATE = _get_prompt
```

### Comparing `openllm-0.2.0/src/openllm/models/mpt/modeling_mpt.py` & `openllm-0.2.1/src/openllm/models/mpt/modeling_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/opt/__init__.py` & `openllm-0.2.1/src/openllm/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/opt/modeling_flax_opt.py` & `openllm-0.2.1/src/openllm/models/opt/modeling_flax_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/opt/modeling_opt.py` & `openllm-0.2.1/src/openllm/models/opt/modeling_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/opt/modeling_tf_opt.py` & `openllm-0.2.1/src/openllm/models/opt/modeling_tf_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/stablelm/__init__.py` & `openllm-0.2.1/src/openllm/models/stablelm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.2.1/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.2.1/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/starcoder/__init__.py` & `openllm-0.2.1/src/openllm/models/starcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.2.1/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.2.1/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/playground/__init__.py` & `openllm-0.2.1/src/openllm/playground/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/playground/_meta.yml` & `openllm-0.2.1/src/openllm/playground/_meta.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/playground/falcon_tuned.py` & `openllm-0.2.1/src/openllm/playground/falcon_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/playground/features.py` & `openllm-0.2.1/src/openllm/playground/features.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/playground/opt_tuned.py` & `openllm-0.2.1/src/openllm/playground/opt_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/serialisation/__init__.py` & `openllm-0.2.1/src/openllm/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/serialisation/constants.py` & `openllm-0.2.1/src/openllm/serialisation/constants.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/serialisation/ggml.py` & `openllm-0.2.1/src/openllm/serialisation/ggml.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/serialisation/transformers.py` & `openllm-0.2.1/src/openllm/serialisation/transformers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/utils/__init__.py` & `openllm-0.2.1/src/openllm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/utils/analytics.py` & `openllm-0.2.1/src/openllm/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/utils/codegen.py` & `openllm-0.2.1/src/openllm/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/utils/dantic.py` & `openllm-0.2.1/src/openllm/utils/dantic.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.2.1/src/openllm/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.2.1/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.2.1/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/utils/dummy_pt_and_triton_objects.py` & `openllm-0.2.1/src/openllm/utils/dummy_pt_and_triton_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.2.1/src/openllm/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.2.1/src/openllm/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/utils/dummy_vllm_objects.py` & `openllm-0.2.1/src/openllm/utils/dummy_vllm_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/utils/import_utils.py` & `openllm-0.2.1/src/openllm/utils/import_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,19 @@
 else:
     from typing_extensions import overload
 
 if t.TYPE_CHECKING:
     BackendOrderredDict = OrderedDict[str, tuple[t.Callable[[], bool], str]]
     from .._types import LiteralRuntime
     from .._types import P
+    from .._types import T
 
-    class _AnnotatedLazyLoader(LazyLoader):
-        DEFAULT_PROMPT_TEMPLATE: t.LiteralString | None | t.Callable[..., t.LiteralString]
+    class _AnnotatedLazyLoader(LazyLoader, t.Generic[T]):
+        DEFAULT_PROMPT_TEMPLATE: t.LiteralString | None | t.Callable[[T], t.LiteralString]
+        PROMPT_MAPPING: dict[T, t.LiteralString] | None
 
 else:
     _AnnotatedLazyLoader = LazyLoader
     BackendOrderredDict = OrderedDict
 
 logger = logging.getLogger(__name__)
 
@@ -530,9 +532,9 @@
         return res
 
     @property
     def start_docstring(self) -> str:
         return getattr(self.module, f"START_{self.model_name.upper()}_COMMAND_DOCSTRING")
 
     @property
-    def module(self) -> _AnnotatedLazyLoader:
+    def module(self) -> _AnnotatedLazyLoader[t.LiteralString]:
         return _AnnotatedLazyLoader(self.model_name, globals(), f"openllm.models.{self.model_name}")
```

### Comparing `openllm-0.2.0/src/openllm/utils/lazy.py` & `openllm-0.2.1/src/openllm/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm/utils/representation.py` & `openllm-0.2.1/src/openllm/utils/representation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm_client/__init__.py` & `openllm-0.2.1/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm_client/_prompt.py` & `openllm-0.2.1/src/openllm_client/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm_client/runtimes/__init__.py` & `openllm-0.2.1/src/openllm_client/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm_client/runtimes/base.py` & `openllm-0.2.1/src/openllm_client/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm_client/runtimes/grpc.py` & `openllm-0.2.1/src/openllm_client/runtimes/grpc.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/src/openllm_client/runtimes/http.py` & `openllm-0.2.1/src/openllm_client/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/__init__.py` & `openllm-0.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/client_test.py` & `openllm-0.2.1/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/configuration_test.py` & `openllm-0.2.1/tests/configuration_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """All configuration-related tests for openllm.LLMConfig. This will include testing
 for ModelEnv construction and parsing environment variables.
 """
 from __future__ import annotations
 import contextlib
 import logging
 import os
+import sys
 import typing as t
 from unittest import mock
 
 import attr
 import pytest
 from hypothesis import assume
 from hypothesis import given
@@ -42,42 +43,41 @@
 
 if t.TYPE_CHECKING:
     DictStrAny = dict[str, t.Any]
 else:
     DictStrAny = dict
 
 
+# XXX: @aarnphm fixes TypedDict behaviour in 3.11
+@pytest.mark.skipif(
+    sys.version_info[:2] == (3, 11), reason="TypedDict in 3.11 behaves differently, so we need to fix this"
+)
 def test_missing_default():
-    assert pytest.raises(
-        ValueError, make_llm_config, "MissingDefaultId", {"name_type": "lowercase", "requirements": ["bentoml"]}
-    ).match("Missing required fields *")
-    assert pytest.raises(
-        ValueError,
-        make_llm_config,
-        "MissingModelId",
-        {"default_id": "huggingface/t5-tiny-testing", "requirements": ["bentoml"]},
-    ).match("Missing required fields *")
-    assert pytest.raises(
-        ValueError,
-        make_llm_config,
-        "MissingArchitecture",
-        {
-            "default_id": "huggingface/t5-tiny-testing",
-            "model_ids": ["huggingface/t5-tiny-testing"],
-            "requirements": ["bentoml"],
-        },
-    ).match("Missing required fields *")
+    with pytest.raises(ValueError, match="Missing required fields *"):
+        make_llm_config("MissingDefaultId", {"name_type": "lowercase", "requirements": ["bentoml"]})
+    with pytest.raises(ValueError, match="Missing required fields *"):
+        make_llm_config("MissingModelId", {"default_id": "huggingface/t5-tiny-testing", "requirements": ["bentoml"]})
+    with pytest.raises(ValueError, match="Missing required fields *"):
+        make_llm_config(
+            "MissingArchitecture",
+            {
+                "default_id": "huggingface/t5-tiny-testing",
+                "model_ids": ["huggingface/t5-tiny-testing"],
+                "requirements": ["bentoml"],
+            },
+        )
 
 
 def test_forbidden_access():
     cl_ = make_llm_config(
         "ForbiddenAccess",
         {
             "default_id": "huggingface/t5-tiny-testing",
             "model_ids": ["huggingface/t5-tiny-testing", "bentoml/t5-tiny-testing"],
+            "architecture": "PreTrainedModel",
             "requirements": ["bentoml"],
         },
     )
 
     assert pytest.raises(
         openllm.exceptions.ForbiddenAttributeError,
         cl_.__getattribute__,
@@ -86,14 +86,20 @@
     )
     assert pytest.raises(
         openllm.exceptions.ForbiddenAttributeError,
         cl_.__getattribute__,
         cl_(),
         "GenerationConfig",
     )
+    assert pytest.raises(
+        openllm.exceptions.ForbiddenAttributeError,
+        cl_.__getattribute__,
+        cl_(),
+        "SamplingParams",
+    )
 
     assert openllm.utils.lenient_issubclass(cl_.__openllm_generation_class__, GenerationConfig)
 
 
 @given(model_settings())
 def test_class_normal_gen(gen_settings: ModelSettings):
     assume(gen_settings["default_id"] and all(i for i in gen_settings["model_ids"]))
@@ -166,15 +172,19 @@
         **{
             field_env_key("env_llm", "field1"): "4",
             field_env_key("env_llm", "temperature", suffix="generation"): "0.2",
         }
     ):
 
         class EnvLLM(openllm.LLMConfig):
-            __config__ = {"default_id": "asdfasdf", "model_ids": ["asdf", "asdfasdfads"]}
+            __config__ = {
+                "default_id": "asdfasdf",
+                "model_ids": ["asdf", "asdfasdfads"],
+                "architecture": "PreTrainedModel",
+            }
             field1: int = 2
 
             class GenerationConfig:
                 temperature: float = 0.8
 
         sent = EnvLLM.model_construct_env()
         assert sent.field1 == 4
@@ -183,15 +193,19 @@
         overwrite_default = EnvLLM()
         assert overwrite_default.field1 == 4
         assert overwrite_default["temperature"] == 0.2
 
 
 def test_struct_provided_fields():
     class EnvLLM(openllm.LLMConfig):
-        __config__ = {"default_id": "asdfasdf", "model_ids": ["asdf", "asdfasdfads"]}
+        __config__ = {
+            "default_id": "asdfasdf",
+            "model_ids": ["asdf", "asdfasdfads"],
+            "architecture": "PreTrainedModel",
+        }
         field1: int = 2
 
         class GenerationConfig:
             temperature: float = 0.8
 
     sent = EnvLLM.model_construct_env(field1=20, temperature=0.4)
     assert sent.field1 == 20
@@ -200,15 +214,15 @@
 
 def test_struct_envvar_with_overwrite_provided_env(monkeypatch: pytest.MonkeyPatch):
     with monkeypatch.context() as mk:
         mk.setenv(field_env_key("overwrite_with_env_available", "field1"), str(4.0))
         mk.setenv(field_env_key("overwrite_with_env_available", "temperature", suffix="generation"), str(0.2))
         sent = make_llm_config(
             "OverwriteWithEnvAvailable",
-            {"default_id": "asdfasdf", "model_ids": ["asdf", "asdfasdfads"]},
+            {"default_id": "asdfasdf", "model_ids": ["asdf", "asdfasdfads"], "architecture": "PreTrainedModel"},
             fields=(("field1", "float", 3.0),),
         ).model_construct_env(field1=20.0, temperature=0.4)
         assert sent.generation_config.temperature == 0.4
         assert sent.field1 == 20.0
 
 
 @given(model_settings())
```

### Comparing `openllm-0.2.0/tests/conftest.py` & `openllm-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/llm_test.py` & `openllm-0.2.1/tests/llm_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/models_test.py` & `openllm-0.2.1/tests/models_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 import pytest
 
 
 if t.TYPE_CHECKING:
     import openllm
 
 
-@pytest.mark.skipif(os.getenv("GITHUB_ACTIONS") is not None, "Model is too large for CI")
+@pytest.mark.skipif(os.getenv("GITHUB_ACTIONS") is not None, reason="Model is too large for CI")
 def test_flan_t5_implementation(prompt: str, llm: openllm.LLM[t.Any, t.Any]):
     assert llm(prompt)
 
     assert llm(prompt, temperature=0.8, top_p=0.23)
 
 
-@pytest.mark.skipif(os.getenv("GITHUB_ACTIONS") is not None, "Model is too large for CI")
+@pytest.mark.skipif(os.getenv("GITHUB_ACTIONS") is not None, reason="Model is too large for CI")
 def test_opt_implementation(prompt: str, llm: openllm.LLM[t.Any, t.Any]):
     assert llm(prompt)
 
     assert llm(prompt, temperature=0.9, top_k=8)
 
 
-@pytest.mark.skipif(os.getenv("GITHUB_ACTIONS") is not None, "Model is too large for CI")
+@pytest.mark.skipif(os.getenv("GITHUB_ACTIONS") is not None, reason="Model is too large for CI")
 def test_baichuan_implementation(prompt: str, llm: openllm.LLM[t.Any, t.Any]):
     assert llm(prompt)
 
     assert llm(prompt, temperature=0.95)
```

### Comparing `openllm-0.2.0/tests/package_test.py` & `openllm-0.2.1/tests/package_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/strategies_test.py` & `openllm-0.2.1/tests/strategies_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
+import os
 import sys
 import typing as t
 
 import pytest
 
 
 if t.TYPE_CHECKING:
@@ -79,14 +80,15 @@
         mcls.setenv("CUDA_VISIBLE_DEVICES", "MIG-GPU-5ebe9f43-ac33420d4628")
         resource = NvidiaGpuResource.from_system()
         assert len(resource) == 1
         assert resource == ["MIG-GPU-5ebe9f43-ac33420d4628"]
         mcls.delenv("CUDA_VISIBLE_DEVICES")
 
 
+@pytest.mark.skipif(os.getenv("GITHUB_ACTIONS") is not None, reason="skip GPUs test on CI")
 def test_nvidia_gpu_validate(monkeypatch: pytest.MonkeyPatch):
     with monkeypatch.context() as mcls:
         # to make this tests works with system that has GPU
         mcls.setenv("CUDA_VISIBLE_DEVICES", "")
         assert len(NvidiaGpuResource.from_system()) >= 0  # TODO: real from_system tests
 
         assert pytest.raises(
```

### Comparing `openllm-0.2.0/tests/_strategies/__init__.py` & `openllm-0.2.1/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/_strategies/_configuration.py` & `openllm-0.2.1/tests/_strategies/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/models/__init__.py` & `openllm-0.2.1/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/models/conftest.py` & `openllm-0.2.1/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/models/flan_t5_test.py` & `openllm-0.2.1/tests/models/flan_t5_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/models/opt_test.py` & `openllm-0.2.1/tests/models/opt_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json` & `openllm-0.2.1/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json` & `openllm-0.2.1/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/models/__snapshots__/opt_test/test_opt_125m[container].json` & `openllm-0.2.1/tests/models/__snapshots__/opt_test/test_opt_125m[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/tests/models/__snapshots__/opt_test/test_opt_125m[local].json` & `openllm-0.2.1/tests/models/__snapshots__/opt_test/test_opt_125m[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/.gitignore` & `openllm-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/LICENSE.md` & `openllm-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/README.md` & `openllm-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -125,140 +125,133 @@
 
 <table align='center'>
 <tr>
 <th>Model</th>
 <th>Architecture</th>
 <th>CPU</th>
 <th>GPU</th>
-<th>Installation</th>
 <th>Model Ids</th>
+<th>Installation</th>
 </tr>
 <tr>
 
 <td><a href=https://github.com/THUDM/ChatGLM-6B>chatglm</a></td>
 <td><a href=https://github.com/THUDM/ChatGLM-6B><code>ChatGLMForConditionalGeneration</code></a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[chatglm]"
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/thudm/chatglm-6b><code>thudm/chatglm-6b</code></a></li>
 <li><a href=https://huggingface.co/thudm/chatglm-6b-int8><code>thudm/chatglm-6b-int8</code></a></li>
 <li><a href=https://huggingface.co/thudm/chatglm-6b-int4><code>thudm/chatglm-6b-int4</code></a></li>
 <li><a href=https://huggingface.co/thudm/chatglm2-6b><code>thudm/chatglm2-6b</code></a></li>
 <li><a href=https://huggingface.co/thudm/chatglm2-6b-int4><code>thudm/chatglm2-6b-int4</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install "openllm[chatglm]"
+```
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/databrickslabs/dolly>dolly-v2</a></td>
 <td><a href=https://huggingface.co/docs/transformers/main/model_doc/gpt_neox#transformers.GPTNeoXForCausalLM><code>GPTNeoXForCausalLM</code></a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install openllm
-```
+<ul><li><a href=https://huggingface.co/databricks/dolly-v2-3b><code>databricks/dolly-v2-3b</code></a></li>
+<li><a href=https://huggingface.co/databricks/dolly-v2-7b><code>databricks/dolly-v2-7b</code></a></li>
+<li><a href=https://huggingface.co/databricks/dolly-v2-12b><code>databricks/dolly-v2-12b</code></a></li></ul>
 
 </td>
 <td>
 
-<ul><li><a href=https://huggingface.co/databricks/dolly-v2-3b><code>databricks/dolly-v2-3b</code></a></li>
-<li><a href=https://huggingface.co/databricks/dolly-v2-7b><code>databricks/dolly-v2-7b</code></a></li>
-<li><a href=https://huggingface.co/databricks/dolly-v2-12b><code>databricks/dolly-v2-12b</code></a></li></ul>
+```bash
+pip install openllm
+```
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://falconllm.tii.ae/>falcon</a></td>
 <td><a href=https://falconllm.tii.ae/><code>FalconForCausalLM</code></a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[falcon]"
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/tiiuae/falcon-7b><code>tiiuae/falcon-7b</code></a></li>
 <li><a href=https://huggingface.co/tiiuae/falcon-40b><code>tiiuae/falcon-40b</code></a></li>
 <li><a href=https://huggingface.co/tiiuae/falcon-7b-instruct><code>tiiuae/falcon-7b-instruct</code></a></li>
 <li><a href=https://huggingface.co/tiiuae/falcon-40b-instruct><code>tiiuae/falcon-40b-instruct</code></a></li></ul>
 
 </td>
-</tr>
-<tr>
-
-<td><a href=https://huggingface.co/docs/transformers/model_doc/flan-t5>flan-t5</a></td>
-<td><a href=https://huggingface.co/docs/transformers/main/model_doc/flan_t5#transformers.T5ForConditionalGeneration><code>T5ForConditionalGeneration</code></a></td>
-<td>✅</td>
-<td>✅</td>
 <td>
 
 ```bash
-pip install "openllm[flan-t5]"
+pip install "openllm[falcon]"
 ```
 
 </td>
+</tr>
+<tr>
+
+<td><a href=https://huggingface.co/docs/transformers/model_doc/flan-t5>flan-t5</a></td>
+<td><a href=https://huggingface.co/docs/transformers/main/model_doc/t5#transformers.T5ForConditionalGeneration><code>T5ForConditionalGeneration</code></a></td>
+<td>✅</td>
+<td>✅</td>
 <td>
 
 <ul><li><a href=https://huggingface.co/google/flan-t5-small><code>google/flan-t5-small</code></a></li>
 <li><a href=https://huggingface.co/google/flan-t5-base><code>google/flan-t5-base</code></a></li>
 <li><a href=https://huggingface.co/google/flan-t5-large><code>google/flan-t5-large</code></a></li>
 <li><a href=https://huggingface.co/google/flan-t5-xl><code>google/flan-t5-xl</code></a></li>
 <li><a href=https://huggingface.co/google/flan-t5-xxl><code>google/flan-t5-xxl</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install "openllm[flan-t5]"
+```
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/EleutherAI/gpt-neox>gpt-neox</a></td>
 <td><a href=https://huggingface.co/docs/transformers/main/model_doc/gpt_neox#transformers.GPTNeoXForCausalLM><code>GPTNeoXForCausalLM</code></a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install openllm
-```
+<ul><li><a href=https://huggingface.co/eleutherai/gpt-neox-20b><code>eleutherai/gpt-neox-20b</code></a></li></ul>
 
 </td>
 <td>
 
-<ul><li><a href=https://huggingface.co/eleutherai/gpt-neox-20b><code>eleutherai/gpt-neox-20b</code></a></li></ul>
+```bash
+pip install openllm
+```
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/facebookresearch/llama>llama</a></td>
 <td><a href=https://huggingface.co/docs/transformers/main/model_doc/llama#transformers.LlamaForCausalLM><code>LlamaForCausalLM</code></a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[llama]"
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/meta-llama/llama-2-70b-chat-hf><code>meta-llama/llama-2-70b-chat-hf</code></a></li>
 <li><a href=https://huggingface.co/meta-llama/llama-2-13b-chat-hf><code>meta-llama/llama-2-13b-chat-hf</code></a></li>
 <li><a href=https://huggingface.co/meta-llama/llama-2-7b-chat-hf><code>meta-llama/llama-2-7b-chat-hf</code></a></li>
 <li><a href=https://huggingface.co/meta-llama/llama-2-70b-hf><code>meta-llama/llama-2-70b-hf</code></a></li>
 <li><a href=https://huggingface.co/meta-llama/llama-2-13b-hf><code>meta-llama/llama-2-13b-hf</code></a></li>
 <li><a href=https://huggingface.co/meta-llama/llama-2-7b-hf><code>meta-llama/llama-2-7b-hf</code></a></li>
 <li><a href=https://huggingface.co/openlm-research/open_llama_7b_v2><code>openlm-research/open_llama_7b_v2</code></a></li>
@@ -266,129 +259,136 @@
 <li><a href=https://huggingface.co/openlm-research/open_llama_13b><code>openlm-research/open_llama_13b</code></a></li>
 <li><a href=https://huggingface.co/huggyllama/llama-65b><code>huggyllama/llama-65b</code></a></li>
 <li><a href=https://huggingface.co/huggyllama/llama-30b><code>huggyllama/llama-30b</code></a></li>
 <li><a href=https://huggingface.co/huggyllama/llama-13b><code>huggyllama/llama-13b</code></a></li>
 <li><a href=https://huggingface.co/huggyllama/llama-7b><code>huggyllama/llama-7b</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install "openllm[llama]"
+```
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://huggingface.co/mosaicml>mpt</a></td>
 <td><a href=https://huggingface.co/mosaicml><code>MPTForCausalLM</code></a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[mpt]"
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/mosaicml/mpt-7b><code>mosaicml/mpt-7b</code></a></li>
 <li><a href=https://huggingface.co/mosaicml/mpt-7b-instruct><code>mosaicml/mpt-7b-instruct</code></a></li>
 <li><a href=https://huggingface.co/mosaicml/mpt-7b-chat><code>mosaicml/mpt-7b-chat</code></a></li>
 <li><a href=https://huggingface.co/mosaicml/mpt-7b-storywriter><code>mosaicml/mpt-7b-storywriter</code></a></li>
 <li><a href=https://huggingface.co/mosaicml/mpt-30b><code>mosaicml/mpt-30b</code></a></li>
 <li><a href=https://huggingface.co/mosaicml/mpt-30b-instruct><code>mosaicml/mpt-30b-instruct</code></a></li>
 <li><a href=https://huggingface.co/mosaicml/mpt-30b-chat><code>mosaicml/mpt-30b-chat</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install "openllm[mpt]"
+```
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://huggingface.co/docs/transformers/model_doc/opt>opt</a></td>
 <td><a href=https://huggingface.co/docs/transformers/main/model_doc/opt#transformers.MPTForCausalLM><code>MPTForCausalLM</code></a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[opt]"
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/facebook/opt-125m><code>facebook/opt-125m</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-350m><code>facebook/opt-350m</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-1.3b><code>facebook/opt-1.3b</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-2.7b><code>facebook/opt-2.7b</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-6.7b><code>facebook/opt-6.7b</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-66b><code>facebook/opt-66b</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install "openllm[opt]"
+```
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/Stability-AI/StableLM>stablelm</a></td>
 <td><a href=https://huggingface.co/docs/transformers/main/model_doc/gpt_neox#transformers.GPTNeoXForCausalLM><code>GPTNeoXForCausalLM</code></a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install openllm
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/stabilityai/stablelm-tuned-alpha-3b><code>stabilityai/stablelm-tuned-alpha-3b</code></a></li>
 <li><a href=https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b><code>stabilityai/stablelm-tuned-alpha-7b</code></a></li>
 <li><a href=https://huggingface.co/stabilityai/stablelm-base-alpha-3b><code>stabilityai/stablelm-base-alpha-3b</code></a></li>
 <li><a href=https://huggingface.co/stabilityai/stablelm-base-alpha-7b><code>stabilityai/stablelm-base-alpha-7b</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install openllm
+```
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/bigcode-project/starcoder>starcoder</a></td>
 <td><a href=https://huggingface.co/docs/transformers/main/model_doc/gpt_bigcode#transformers.GPTBigCodeForCausalLM><code>GPTBigCodeForCausalLM</code></a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[starcoder]"
-```
+<ul><li><a href=https://huggingface.co/bigcode/starcoder><code>bigcode/starcoder</code></a></li>
+<li><a href=https://huggingface.co/bigcode/starcoderbase><code>bigcode/starcoderbase</code></a></li></ul>
 
 </td>
 <td>
 
-<ul><li><a href=https://huggingface.co/bigcode/starcoder><code>bigcode/starcoder</code></a></li>
-<li><a href=https://huggingface.co/bigcode/starcoderbase><code>bigcode/starcoderbase</code></a></li></ul>
+```bash
+pip install "openllm[starcoder]"
+```
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/baichuan-inc/Baichuan-7B>baichuan</a></td>
 <td><a href=https://github.com/baichuan-inc/Baichuan-7B><code>BaiChuanForCausalLM</code></a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[baichuan]"
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/baichuan-inc/baichuan-7b><code>baichuan-inc/baichuan-7b</code></a></li>
 <li><a href=https://huggingface.co/baichuan-inc/baichuan-13b-base><code>baichuan-inc/baichuan-13b-base</code></a></li>
 <li><a href=https://huggingface.co/baichuan-inc/baichuan-13b-chat><code>baichuan-inc/baichuan-13b-chat</code></a></li>
 <li><a href=https://huggingface.co/fireballoon/baichuan-vicuna-chinese-7b><code>fireballoon/baichuan-vicuna-chinese-7b</code></a></li>
 <li><a href=https://huggingface.co/fireballoon/baichuan-vicuna-7b><code>fireballoon/baichuan-vicuna-7b</code></a></li>
 <li><a href=https://huggingface.co/hiyouga/baichuan-7b-sft><code>hiyouga/baichuan-7b-sft</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install "openllm[baichuan]"
+```
+
+</td>
 </tr>
 </table>
 
 <!-- update-readme.py: stop -->
 
 ### Runtime Implementations (Experimental)
```

#### html2text {}

```diff
@@ -54,135 +54,135 @@
 Users can also specify different variants of the model to be served, by
 providing the `--model-id` argument, e.g.: ```bash openllm start flan-t5 --
 model-id google/flan-t5-large ``` Use the `openllm models` command to see the
 list of models and their variants supported in OpenLLM. ## ð§© Supported
 Models The following models are currently supported in OpenLLM. By default,
 OpenLLM doesn't include dependencies to run all models. The extra model-
 specific dependencies can be installed with the instructions below:
-Model     Architecture                    CPU GPU Installation Model Ids
-                                                                   * thudm/chatglm-6b
-                                                                   * thudm/chatglm-
-                                                  ```bash pip        6b-int8
-                                                  install          * thudm/chatglm-
-chatglm   ChatGLMForConditionalGeneration ââ"openllm           6b-int4
-                                                  [chatglm]"       * thudm/chatglm2-
-                                                  ```                6b
-                                                                   * thudm/chatglm2-
-                                                                     6b-int4
-                                                                   * databricks/
-                                                  ```bash pip        dolly-v2-3b
-dolly-v2  GPTNeoXForCausalLM              ââinstall          * databricks/
-                                                  openllm ```        dolly-v2-7b
-                                                                   * databricks/
-                                                                     dolly-v2-12b
-                                                                   * tiiuae/falcon-7b
-                                                  ```bash pip      * tiiuae/falcon-
-                                                  install            40b
-falcon    FalconForCausalLM               ââ"openllm         * tiiuae/falcon-
-                                                  [falcon]"          7b-instruct
-                                                  ```              * tiiuae/falcon-
-                                                                     40b-instruct
-                                                                   * google/flan-t5-
-                                                                     small
-                                                  ```bash pip      * google/flan-t5-
-                                                  install            base
-flan-t5   T5ForConditionalGeneration      ââ"openllm         * google/flan-t5-
-                                                  [flan-t5]"         large
-                                                  ```              * google/flan-t5-
-                                                                     xl
-                                                                   * google/flan-t5-
-                                                                     xxl
-                                                  ```bash pip      * eleutherai/gpt-
-gpt-neox  GPTNeoXForCausalLM              ââinstall            neox-20b
-                                                  openllm ```
-                                                                   * meta-llama/
-                                                                     llama-2-70b-
-                                                                     chat-hf
-                                                                   * meta-llama/
-                                                                     llama-2-13b-
-                                                                     chat-hf
-                                                                   * meta-llama/
-                                                                     llama-2-7b-chat-
-                                                                     hf
-                                                                   * meta-llama/
-                                                                     llama-2-70b-hf
-                                                                   * meta-llama/
-                                                  ```bash pip        llama-2-13b-hf
-                                                  install          * meta-llama/
-llama     LlamaForCausalLM                ââ"openllm           llama-2-7b-hf
-                                                  [llama]" ```     * openlm-research/
-                                                                     open_llama_7b_v2
-                                                                   * openlm-research/
-                                                                     open_llama_3b_v2
-                                                                   * openlm-research/
-                                                                     open_llama_13b
-                                                                   * huggyllama/
-                                                                     llama-65b
-                                                                   * huggyllama/
-                                                                     llama-30b
-                                                                   * huggyllama/
-                                                                     llama-13b
-                                                                   * huggyllama/
-                                                                     llama-7b
-                                                                   * mosaicml/mpt-7b
-                                                                   * mosaicml/mpt-7b-
-                                                                     instruct
-                                                                   * mosaicml/mpt-7b-
-                                                  ```bash pip        chat
-mpt       MPTForCausalLM                  ââinstall          * mosaicml/mpt-7b-
-                                                  "openllm           storywriter
-                                                  [mpt]" ```       * mosaicml/mpt-30b
-                                                                   * mosaicml/mpt-
-                                                                     30b-instruct
-                                                                   * mosaicml/mpt-
-                                                                     30b-chat
-                                                                   * facebook/opt-
-                                                                     125m
-                                                                   * facebook/opt-
-                                                  ```bash pip        350m
-                                                  install          * facebook/opt-
-opt       MPTForCausalLM                  ââ"openllm           1.3b
-                                                  [opt]" ```       * facebook/opt-
-                                                                     2.7b
-                                                                   * facebook/opt-
-                                                                     6.7b
-                                                                   * facebook/opt-66b
-                                                                   * stabilityai/
-                                                                     stablelm-tuned-
-                                                                     alpha-3b
-                                                                   * stabilityai/
-                                                  ```bash pip        stablelm-tuned-
-stablelm  GPTNeoXForCausalLM              ââinstall            alpha-7b
-                                                  openllm ```      * stabilityai/
-                                                                     stablelm-base-
-                                                                     alpha-3b
-                                                                   * stabilityai/
-                                                                     stablelm-base-
-                                                                     alpha-7b
-                                                  ```bash pip      * bigcode/
-                                                  install            starcoder
-starcoder GPTBigCodeForCausalLM           ââ"openllm         * bigcode/
-                                                  [starcoder]"       starcoderbase
-                                                  ```
-                                                                   * baichuan-inc/
-                                                                     baichuan-7b
-                                                                   * baichuan-inc/
-                                                                     baichuan-13b-
-                                                                     base
-                                                  ```bash pip      * baichuan-inc/
-                                                  install            baichuan-13b-
-baichuan  BaiChuanForCausalLM             ââ"openllm           chat
-                                                  [baichuan]"      * fireballoon/
-                                                  ```                baichuan-vicuna-
-                                                                     chinese-7b
-                                                                   * fireballoon/
-                                                                     baichuan-vicuna-
-                                                                     7b
-                                                                   * hiyouga/
-                                                                     baichuan-7b-sft
+Model     Architecture                    CPU GPU Model Ids              Installation
+                                                      * thudm/chatglm-6b
+                                                      * thudm/chatglm-
+                                                        6b-int8          ```bash pip
+                                                      * thudm/chatglm-   install
+chatglm   ChatGLMForConditionalGeneration ââ      6b-int4          "openllm
+                                                      * thudm/chatglm2-  [chatglm]"
+                                                        6b               ```
+                                                      * thudm/chatglm2-
+                                                        6b-int4
+                                                      * databricks/
+                                                        dolly-v2-3b      ```bash pip
+dolly-v2  GPTNeoXForCausalLM              ââ    * databricks/      install
+                                                        dolly-v2-7b      openllm ```
+                                                      * databricks/
+                                                        dolly-v2-12b
+                                                      * tiiuae/falcon-7b
+                                                      * tiiuae/falcon-   ```bash pip
+                                                        40b              install
+falcon    FalconForCausalLM               ââ    * tiiuae/falcon-   "openllm
+                                                        7b-instruct      [falcon]"
+                                                      * tiiuae/falcon-   ```
+                                                        40b-instruct
+                                                      * google/flan-t5-
+                                                        small
+                                                      * google/flan-t5-  ```bash pip
+                                                        base             install
+flan-t5   T5ForConditionalGeneration      ââ    * google/flan-t5-  "openllm
+                                                        large            [flan-t5]"
+                                                      * google/flan-t5-  ```
+                                                        xl
+                                                      * google/flan-t5-
+                                                        xxl
+                                                      * eleutherai/gpt-  ```bash pip
+gpt-neox  GPTNeoXForCausalLM              ââ      neox-20b         install
+                                                                         openllm ```
+                                                      * meta-llama/
+                                                        llama-2-70b-
+                                                        chat-hf
+                                                      * meta-llama/
+                                                        llama-2-13b-
+                                                        chat-hf
+                                                      * meta-llama/
+                                                        llama-2-7b-chat-
+                                                        hf
+                                                      * meta-llama/
+                                                        llama-2-70b-hf
+                                                      * meta-llama/
+                                                        llama-2-13b-hf   ```bash pip
+                                                      * meta-llama/      install
+llama     LlamaForCausalLM                ââ      llama-2-7b-hf    "openllm
+                                                      * openlm-research/ [llama]" ```
+                                                        open_llama_7b_v2
+                                                      * openlm-research/
+                                                        open_llama_3b_v2
+                                                      * openlm-research/
+                                                        open_llama_13b
+                                                      * huggyllama/
+                                                        llama-65b
+                                                      * huggyllama/
+                                                        llama-30b
+                                                      * huggyllama/
+                                                        llama-13b
+                                                      * huggyllama/
+                                                        llama-7b
+                                                      * mosaicml/mpt-7b
+                                                      * mosaicml/mpt-7b-
+                                                        instruct
+                                                      * mosaicml/mpt-7b-
+                                                        chat             ```bash pip
+mpt       MPTForCausalLM                  ââ    * mosaicml/mpt-7b- install
+                                                        storywriter      "openllm
+                                                      * mosaicml/mpt-30b [mpt]" ```
+                                                      * mosaicml/mpt-
+                                                        30b-instruct
+                                                      * mosaicml/mpt-
+                                                        30b-chat
+                                                      * facebook/opt-
+                                                        125m
+                                                      * facebook/opt-
+                                                        350m             ```bash pip
+                                                      * facebook/opt-    install
+opt       MPTForCausalLM                  ââ      1.3b             "openllm
+                                                      * facebook/opt-    [opt]" ```
+                                                        2.7b
+                                                      * facebook/opt-
+                                                        6.7b
+                                                      * facebook/opt-66b
+                                                      * stabilityai/
+                                                        stablelm-tuned-
+                                                        alpha-3b
+                                                      * stabilityai/
+                                                        stablelm-tuned-  ```bash pip
+stablelm  GPTNeoXForCausalLM              ââ      alpha-7b         install
+                                                      * stabilityai/     openllm ```
+                                                        stablelm-base-
+                                                        alpha-3b
+                                                      * stabilityai/
+                                                        stablelm-base-
+                                                        alpha-7b
+                                                      * bigcode/         ```bash pip
+                                                        starcoder        install
+starcoder GPTBigCodeForCausalLM           ââ    * bigcode/         "openllm
+                                                        starcoderbase    [starcoder]"
+                                                                         ```
+                                                      * baichuan-inc/
+                                                        baichuan-7b
+                                                      * baichuan-inc/
+                                                        baichuan-13b-
+                                                        base
+                                                      * baichuan-inc/    ```bash pip
+                                                        baichuan-13b-    install
+baichuan  BaiChuanForCausalLM             ââ      chat             "openllm
+                                                      * fireballoon/     [baichuan]"
+                                                        baichuan-vicuna- ```
+                                                        chinese-7b
+                                                      * fireballoon/
+                                                        baichuan-vicuna-
+                                                        7b
+                                                      * hiyouga/
+                                                        baichuan-7b-sft
  ### Runtime Implementations (Experimental) Different LLMs may have multiple
 runtime implementations. For instance, they might use Pytorch (`pt`),
 Tensorflow (`tf`), or Flax (`flax`). If you wish to specify a particular
 runtime for a model, you can do so by setting the `OPENLLM_
 {MODEL_NAME}_FRAMEWORK={runtime}` environment variable before running `openllm
 start`. For example, if you want to use the Tensorflow (`tf`) implementation
 for the `flan-t5` model, you can use the following command: ```bash
```

### Comparing `openllm-0.2.0/hatch.toml` & `openllm-0.2.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.0/pyproject.toml` & `openllm-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "bentoml[grpc,io]>=1.0.24",
+    "bentoml[grpc,io]>=1.0.25",
     "transformers[torch,tokenizers,accelerate]>=4.29.0",
     "safetensors",
     "optimum",
     "attrs>=23.1.0",
     "cattrs>=23.1.0",
     "orjson",
     "inflection",
```

### Comparing `openllm-0.2.0/PKG-INFO` & `openllm-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.2.0
+Version: 0.2.1
 Summary: OpenLLM: Operating LLMs in production
 Project-URL: Blog, https://modelserving.com
 Project-URL: Discord, https://l.bentoml.com/join-openllm-discord
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: GitHub, https://github.com/bentoml/openllm
 Project-URL: History, https://github.com/bentoml/openllm/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
@@ -35,15 +35,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: attrs>=23.1.0
-Requires-Dist: bentoml[grpc,io]>=1.0.24
+Requires-Dist: bentoml[grpc,io]>=1.0.25
 Requires-Dist: bitsandbytes<0.40
 Requires-Dist: cattrs>=23.1.0
 Requires-Dist: cuda-python; platform_system != 'Darwin'
 Requires-Dist: httpx
 Requires-Dist: inflection
 Requires-Dist: optimum
 Requires-Dist: orjson
@@ -253,140 +253,133 @@
 
 <table align='center'>
 <tr>
 <th>Model</th>
 <th>Architecture</th>
 <th>CPU</th>
 <th>GPU</th>
-<th>Installation</th>
 <th>Model Ids</th>
+<th>Installation</th>
 </tr>
 <tr>
 
 <td><a href=https://github.com/THUDM/ChatGLM-6B>chatglm</a></td>
 <td><a href=https://github.com/THUDM/ChatGLM-6B><code>ChatGLMForConditionalGeneration</code></a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[chatglm]"
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/thudm/chatglm-6b><code>thudm/chatglm-6b</code></a></li>
 <li><a href=https://huggingface.co/thudm/chatglm-6b-int8><code>thudm/chatglm-6b-int8</code></a></li>
 <li><a href=https://huggingface.co/thudm/chatglm-6b-int4><code>thudm/chatglm-6b-int4</code></a></li>
 <li><a href=https://huggingface.co/thudm/chatglm2-6b><code>thudm/chatglm2-6b</code></a></li>
 <li><a href=https://huggingface.co/thudm/chatglm2-6b-int4><code>thudm/chatglm2-6b-int4</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install "openllm[chatglm]"
+```
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/databrickslabs/dolly>dolly-v2</a></td>
 <td><a href=https://huggingface.co/docs/transformers/main/model_doc/gpt_neox#transformers.GPTNeoXForCausalLM><code>GPTNeoXForCausalLM</code></a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install openllm
-```
+<ul><li><a href=https://huggingface.co/databricks/dolly-v2-3b><code>databricks/dolly-v2-3b</code></a></li>
+<li><a href=https://huggingface.co/databricks/dolly-v2-7b><code>databricks/dolly-v2-7b</code></a></li>
+<li><a href=https://huggingface.co/databricks/dolly-v2-12b><code>databricks/dolly-v2-12b</code></a></li></ul>
 
 </td>
 <td>
 
-<ul><li><a href=https://huggingface.co/databricks/dolly-v2-3b><code>databricks/dolly-v2-3b</code></a></li>
-<li><a href=https://huggingface.co/databricks/dolly-v2-7b><code>databricks/dolly-v2-7b</code></a></li>
-<li><a href=https://huggingface.co/databricks/dolly-v2-12b><code>databricks/dolly-v2-12b</code></a></li></ul>
+```bash
+pip install openllm
+```
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://falconllm.tii.ae/>falcon</a></td>
 <td><a href=https://falconllm.tii.ae/><code>FalconForCausalLM</code></a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[falcon]"
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/tiiuae/falcon-7b><code>tiiuae/falcon-7b</code></a></li>
 <li><a href=https://huggingface.co/tiiuae/falcon-40b><code>tiiuae/falcon-40b</code></a></li>
 <li><a href=https://huggingface.co/tiiuae/falcon-7b-instruct><code>tiiuae/falcon-7b-instruct</code></a></li>
 <li><a href=https://huggingface.co/tiiuae/falcon-40b-instruct><code>tiiuae/falcon-40b-instruct</code></a></li></ul>
 
 </td>
-</tr>
-<tr>
-
-<td><a href=https://huggingface.co/docs/transformers/model_doc/flan-t5>flan-t5</a></td>
-<td><a href=https://huggingface.co/docs/transformers/main/model_doc/flan_t5#transformers.T5ForConditionalGeneration><code>T5ForConditionalGeneration</code></a></td>
-<td>✅</td>
-<td>✅</td>
 <td>
 
 ```bash
-pip install "openllm[flan-t5]"
+pip install "openllm[falcon]"
 ```
 
 </td>
+</tr>
+<tr>
+
+<td><a href=https://huggingface.co/docs/transformers/model_doc/flan-t5>flan-t5</a></td>
+<td><a href=https://huggingface.co/docs/transformers/main/model_doc/t5#transformers.T5ForConditionalGeneration><code>T5ForConditionalGeneration</code></a></td>
+<td>✅</td>
+<td>✅</td>
 <td>
 
 <ul><li><a href=https://huggingface.co/google/flan-t5-small><code>google/flan-t5-small</code></a></li>
 <li><a href=https://huggingface.co/google/flan-t5-base><code>google/flan-t5-base</code></a></li>
 <li><a href=https://huggingface.co/google/flan-t5-large><code>google/flan-t5-large</code></a></li>
 <li><a href=https://huggingface.co/google/flan-t5-xl><code>google/flan-t5-xl</code></a></li>
 <li><a href=https://huggingface.co/google/flan-t5-xxl><code>google/flan-t5-xxl</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install "openllm[flan-t5]"
+```
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/EleutherAI/gpt-neox>gpt-neox</a></td>
 <td><a href=https://huggingface.co/docs/transformers/main/model_doc/gpt_neox#transformers.GPTNeoXForCausalLM><code>GPTNeoXForCausalLM</code></a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install openllm
-```
+<ul><li><a href=https://huggingface.co/eleutherai/gpt-neox-20b><code>eleutherai/gpt-neox-20b</code></a></li></ul>
 
 </td>
 <td>
 
-<ul><li><a href=https://huggingface.co/eleutherai/gpt-neox-20b><code>eleutherai/gpt-neox-20b</code></a></li></ul>
+```bash
+pip install openllm
+```
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/facebookresearch/llama>llama</a></td>
 <td><a href=https://huggingface.co/docs/transformers/main/model_doc/llama#transformers.LlamaForCausalLM><code>LlamaForCausalLM</code></a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[llama]"
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/meta-llama/llama-2-70b-chat-hf><code>meta-llama/llama-2-70b-chat-hf</code></a></li>
 <li><a href=https://huggingface.co/meta-llama/llama-2-13b-chat-hf><code>meta-llama/llama-2-13b-chat-hf</code></a></li>
 <li><a href=https://huggingface.co/meta-llama/llama-2-7b-chat-hf><code>meta-llama/llama-2-7b-chat-hf</code></a></li>
 <li><a href=https://huggingface.co/meta-llama/llama-2-70b-hf><code>meta-llama/llama-2-70b-hf</code></a></li>
 <li><a href=https://huggingface.co/meta-llama/llama-2-13b-hf><code>meta-llama/llama-2-13b-hf</code></a></li>
 <li><a href=https://huggingface.co/meta-llama/llama-2-7b-hf><code>meta-llama/llama-2-7b-hf</code></a></li>
 <li><a href=https://huggingface.co/openlm-research/open_llama_7b_v2><code>openlm-research/open_llama_7b_v2</code></a></li>
@@ -394,129 +387,136 @@
 <li><a href=https://huggingface.co/openlm-research/open_llama_13b><code>openlm-research/open_llama_13b</code></a></li>
 <li><a href=https://huggingface.co/huggyllama/llama-65b><code>huggyllama/llama-65b</code></a></li>
 <li><a href=https://huggingface.co/huggyllama/llama-30b><code>huggyllama/llama-30b</code></a></li>
 <li><a href=https://huggingface.co/huggyllama/llama-13b><code>huggyllama/llama-13b</code></a></li>
 <li><a href=https://huggingface.co/huggyllama/llama-7b><code>huggyllama/llama-7b</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install "openllm[llama]"
+```
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://huggingface.co/mosaicml>mpt</a></td>
 <td><a href=https://huggingface.co/mosaicml><code>MPTForCausalLM</code></a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[mpt]"
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/mosaicml/mpt-7b><code>mosaicml/mpt-7b</code></a></li>
 <li><a href=https://huggingface.co/mosaicml/mpt-7b-instruct><code>mosaicml/mpt-7b-instruct</code></a></li>
 <li><a href=https://huggingface.co/mosaicml/mpt-7b-chat><code>mosaicml/mpt-7b-chat</code></a></li>
 <li><a href=https://huggingface.co/mosaicml/mpt-7b-storywriter><code>mosaicml/mpt-7b-storywriter</code></a></li>
 <li><a href=https://huggingface.co/mosaicml/mpt-30b><code>mosaicml/mpt-30b</code></a></li>
 <li><a href=https://huggingface.co/mosaicml/mpt-30b-instruct><code>mosaicml/mpt-30b-instruct</code></a></li>
 <li><a href=https://huggingface.co/mosaicml/mpt-30b-chat><code>mosaicml/mpt-30b-chat</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install "openllm[mpt]"
+```
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://huggingface.co/docs/transformers/model_doc/opt>opt</a></td>
 <td><a href=https://huggingface.co/docs/transformers/main/model_doc/opt#transformers.MPTForCausalLM><code>MPTForCausalLM</code></a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[opt]"
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/facebook/opt-125m><code>facebook/opt-125m</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-350m><code>facebook/opt-350m</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-1.3b><code>facebook/opt-1.3b</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-2.7b><code>facebook/opt-2.7b</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-6.7b><code>facebook/opt-6.7b</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-66b><code>facebook/opt-66b</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install "openllm[opt]"
+```
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/Stability-AI/StableLM>stablelm</a></td>
 <td><a href=https://huggingface.co/docs/transformers/main/model_doc/gpt_neox#transformers.GPTNeoXForCausalLM><code>GPTNeoXForCausalLM</code></a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install openllm
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/stabilityai/stablelm-tuned-alpha-3b><code>stabilityai/stablelm-tuned-alpha-3b</code></a></li>
 <li><a href=https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b><code>stabilityai/stablelm-tuned-alpha-7b</code></a></li>
 <li><a href=https://huggingface.co/stabilityai/stablelm-base-alpha-3b><code>stabilityai/stablelm-base-alpha-3b</code></a></li>
 <li><a href=https://huggingface.co/stabilityai/stablelm-base-alpha-7b><code>stabilityai/stablelm-base-alpha-7b</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install openllm
+```
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/bigcode-project/starcoder>starcoder</a></td>
 <td><a href=https://huggingface.co/docs/transformers/main/model_doc/gpt_bigcode#transformers.GPTBigCodeForCausalLM><code>GPTBigCodeForCausalLM</code></a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[starcoder]"
-```
+<ul><li><a href=https://huggingface.co/bigcode/starcoder><code>bigcode/starcoder</code></a></li>
+<li><a href=https://huggingface.co/bigcode/starcoderbase><code>bigcode/starcoderbase</code></a></li></ul>
 
 </td>
 <td>
 
-<ul><li><a href=https://huggingface.co/bigcode/starcoder><code>bigcode/starcoder</code></a></li>
-<li><a href=https://huggingface.co/bigcode/starcoderbase><code>bigcode/starcoderbase</code></a></li></ul>
+```bash
+pip install "openllm[starcoder]"
+```
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/baichuan-inc/Baichuan-7B>baichuan</a></td>
 <td><a href=https://github.com/baichuan-inc/Baichuan-7B><code>BaiChuanForCausalLM</code></a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
-```bash
-pip install "openllm[baichuan]"
-```
-
-</td>
-<td>
-
 <ul><li><a href=https://huggingface.co/baichuan-inc/baichuan-7b><code>baichuan-inc/baichuan-7b</code></a></li>
 <li><a href=https://huggingface.co/baichuan-inc/baichuan-13b-base><code>baichuan-inc/baichuan-13b-base</code></a></li>
 <li><a href=https://huggingface.co/baichuan-inc/baichuan-13b-chat><code>baichuan-inc/baichuan-13b-chat</code></a></li>
 <li><a href=https://huggingface.co/fireballoon/baichuan-vicuna-chinese-7b><code>fireballoon/baichuan-vicuna-chinese-7b</code></a></li>
 <li><a href=https://huggingface.co/fireballoon/baichuan-vicuna-7b><code>fireballoon/baichuan-vicuna-7b</code></a></li>
 <li><a href=https://huggingface.co/hiyouga/baichuan-7b-sft><code>hiyouga/baichuan-7b-sft</code></a></li></ul>
 
 </td>
+<td>
+
+```bash
+pip install "openllm[baichuan]"
+```
+
+</td>
 </tr>
 </table>
 
 <!-- update-readme.py: stop -->
 
 ### Runtime Implementations (Experimental)
```

