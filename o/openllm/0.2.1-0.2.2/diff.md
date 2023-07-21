# Comparing `tmp/openllm-0.2.1.tar.gz` & `tmp/openllm-0.2.2.tar.gz`

## Comparing `openllm-0.2.1.tar` & `openllm-0.2.2.tar`

### file list

```diff
@@ -1,137 +1,138 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 openllm-0.2.1/.DS_Store
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.1/.gitattributes
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 openllm-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.1/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0    12098 2020-02-02 00:00:00.000000 openllm-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.1/CITATION.cff
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.1/DEVELOPMENT.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.1/nightly-requirements-gpu.txt
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.1/nightly-requirements.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.1/package.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.1/pyoxidizer.bzl
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.1/taplo.toml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/__about__.py
--rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/__main__.py
--rw-r--r--   0        0        0    90069 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_configuration.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_generation.py
--rw-r--r--   0        0        0    67199 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_llm.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_prompt.py
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_quantisation.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_schema.py
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_service.py
--rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_strategies.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/_types.py
--rw-r--r--   0        0        0   101301 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/cli.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/client.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/py.typed
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/testing.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/bundle/__init__.py
--rw-r--r--   0        0        0    14379 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/bundle/_package.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/bundle/oci/Dockerfile-builder
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/bundle/oci/Dockerfile-vllm
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/bundle/oci/__init__.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/auto/modeling_vllm_auto.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/baichuan/__init__.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/baichuan/configuration_baichuan.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/baichuan/modeling_baichuan.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/gpt_neox/configuration_gpt_neox.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/gpt_neox/modeling_gpt_neox.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/llama/configuration_llama.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/llama/modeling_llama.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/llama/modeling_vllm_llama.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/mpt/__init__.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/mpt/configuration_mpt.py
--rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/mpt/modeling_mpt.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/opt/__init__.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/opt/configuration_opt.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/opt/modeling_flax_opt.py
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/opt/modeling_opt.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/opt/modeling_tf_opt.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/playground/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/playground/__init__.py
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/playground/_meta.yml
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/playground/falcon_tuned.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/playground/features.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/playground/opt_tuned.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/serialisation/__init__.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/serialisation/constants.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/serialisation/ggml.py
--rw-r--r--   0        0        0    16729 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/serialisation/transformers.py
--rw-r--r--   0        0        0    16991 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0    11276 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    19990 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_pt_and_triton_objects.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/dummy_vllm_objects.py
--rw-r--r--   0        0        0    20528 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm/utils/representation.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.1/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/client_test.py
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/configuration_test.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/llm_test.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models_test.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/package_test.py
--rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/strategies_test.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/__init__.py
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/conftest.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/flan_t5_test.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/opt_test.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.1/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.1/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.1/LICENSE.md
--rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.1/README.md
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 openllm-0.2.1/hatch.toml
--rw-r--r--   0        0        0    10577 2020-02-02 00:00:00.000000 openllm-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    30137 2020-02-02 00:00:00.000000 openllm-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 openllm-0.2.2/.DS_Store
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.2/.gitattributes
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 openllm-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.2/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0    12183 2020-02-02 00:00:00.000000 openllm-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.2/CITATION.cff
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.2/DEVELOPMENT.md
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.2/nightly-requirements-gpu.txt
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.2/nightly-requirements.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.2/package.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.2/pyoxidizer.bzl
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.2/taplo.toml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/__about__.py
+-rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/__main__.py
+-rw-r--r--   0        0        0    90069 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_configuration.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_generation.py
+-rw-r--r--   0        0        0    67405 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_llm.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_quantisation.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_schema.py
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_service.py
+-rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_strategies.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_types.py
+-rw-r--r--   0        0        0   101267 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/cli.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/client.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/py.typed
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/testing.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/bundle/__init__.py
+-rw-r--r--   0        0        0    14379 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/bundle/_package.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/bundle/oci/Dockerfile-builder
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/bundle/oci/Dockerfile-vllm
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/bundle/oci/__init__.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/modeling_vllm_auto.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/baichuan/__init__.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/baichuan/configuration_baichuan.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/baichuan/modeling_baichuan.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/gpt_neox/configuration_gpt_neox.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/gpt_neox/modeling_gpt_neox.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/llama/configuration_llama.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/llama/modeling_llama.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/llama/modeling_vllm_llama.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/mpt/__init__.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/mpt/configuration_mpt.py
+-rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/mpt/modeling_mpt.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/opt/__init__.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/opt/configuration_opt.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/opt/modeling_flax_opt.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/opt/modeling_opt.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/opt/modeling_tf_opt.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/__init__.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/_meta.yml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/falcon_tuned.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/features.py
+-rw-r--r--   0        0        0     8507 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/llama2_qlora.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/opt_tuned.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/serialisation/__init__.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/serialisation/constants.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/serialisation/ggml.py
+-rw-r--r--   0        0        0    16729 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/serialisation/transformers.py
+-rw-r--r--   0        0        0    16991 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    19990 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_pt_and_triton_objects.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_vllm_objects.py
+-rw-r--r--   0        0        0    20528 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/representation.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/client_test.py
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/configuration_test.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/llm_test.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models_test.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/package_test.py
+-rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/strategies_test.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/__init__.py
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/conftest.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/flan_t5_test.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/opt_test.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.2/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.2/README.md
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 openllm-0.2.2/hatch.toml
+-rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 openllm-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    30090 2020-02-02 00:00:00.000000 openllm-0.2.2/PKG-INFO
```

### Comparing `openllm-0.2.1/.DS_Store` & `openllm-0.2.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/.pre-commit-config.yaml` & `openllm-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/ADDING_NEW_MODEL.md` & `openllm-0.2.2/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/CHANGELOG.md` & `openllm-0.2.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.2.2](https://github.com/bentoml/openllm/tree/v0.2.2)
+No significant changes.
+
+
 ## [0.2.1](https://github.com/bentoml/openllm/tree/v0.2.1)
 No significant changes.
 
 
 ## [0.2.0](https://github.com/bentoml/openllm/tree/v0.2.0)
 
 ### Features
```

### Comparing `openllm-0.2.1/CITATION.cff` & `openllm-0.2.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/DEVELOPMENT.md` & `openllm-0.2.2/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/nightly-requirements.txt` & `openllm-0.2.2/nightly-requirements.txt`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/package.json` & `openllm-0.2.2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.2.1",
+    "version": "0.2.2",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.2.1/pyoxidizer.bzl` & `openllm-0.2.2/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/__about__.py` & `openllm-0.2.2/src/openllm/__about__.py`

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
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

### Comparing `openllm-0.2.1/src/openllm/__init__.py` & `openllm-0.2.2/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/__main__.py` & `openllm-0.2.2/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/_configuration.py` & `openllm-0.2.2/src/openllm/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/_generation.py` & `openllm-0.2.2/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/_llm.py` & `openllm-0.2.2/src/openllm/_llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,15 +690,15 @@
         if quantization_config is None and quantize is not None:
             quantization_config, attrs = infer_quantisation_config(cls, quantize, **attrs)
 
         if quantize == "gptq":
             # We will use safetensors for gptq
             serialisation = "safetensors"
 
-        # NOTE: Fine-tuning setup
+        # NOTE: LoRA adapter setup
         if adapter_map and adapter_id:
             raise ValueError(
                 """'adapter_map' and 'adapter_id' are mutually exclusive. Either provide a
                 'adapter_map' ({adapter_id: adapter_name | None, ...}) or use
                 the combination of adapter_id/adapter_name arguments.
                 """
             )
@@ -853,16 +853,16 @@
         # low_cpu_mem_usage is only available for model
         # this is helpful on system with low memory to avoid OOM
         low_cpu_mem_usage = attrs.pop("low_cpu_mem_usage", True)
 
         if self.__llm_implementation__ == "pt":
             attrs.update({"low_cpu_mem_usage": low_cpu_mem_usage, "quantization_config": quantization_config})
 
-        model_kwds: dict[str, t.Any] = {}
-        tokenizer_kwds: dict[str, t.Any] = {}
+        model_kwds: DictStrAny = {}
+        tokenizer_kwds: DictStrAny = {}
         if self.import_kwargs is not None:
             model_kwds, tokenizer_kwds = self.import_kwargs
 
         # parsing tokenizer and model kwargs, as the hierachy is param pass > default
         normalized_model_kwds, normalized_tokenizer_kwds = normalize_attrs_to_model_tokenizer_pair(**attrs)
         # NOTE: Save the args and kwargs for latter load
 
@@ -1064,15 +1064,20 @@
                 adapter_map[_adapter_type][name] = (peft_config, adapter.adapter_id)
 
         if self.__llm_adapter_map__ is None and use_cache:
             self.__llm_adapter_map__ = adapter_map
         return adapter_map
 
     @requires_dependencies("peft", extra="fine-tune")
-    def prepare_for_training(self, adapter_type: AdapterType = "lora", **attrs: t.Any) -> tuple[peft.PeftModel, T]:
+    def prepare_for_training(
+        self,
+        adapter_type: AdapterType = "lora",
+        use_gradient_checkpointing: bool = True,
+        **attrs: t.Any,
+    ) -> tuple[peft.PeftModel, T]:
         if pkg.pkg_version_info("peft")[:2] >= (0, 4):
             from peft import prepare_model_for_kbit_training
         else:
             from peft import prepare_model_for_int8_training as prepare_model_for_kbit_training
 
         peft_config = (
             self.config["fine_tune_strategies"]
@@ -1083,15 +1088,21 @@
                     llm_config_class=self.config_class,
                 ),
             )
             .train()
             .with_config(**attrs)
             .to_peft_config()
         )
-        wrapped_peft = peft.get_peft_model(prepare_model_for_kbit_training(self.model), peft_config)
+        wrapped_peft = peft.get_peft_model(
+            prepare_model_for_kbit_training(
+                self.model,
+                use_gradient_checkpointing=use_gradient_checkpointing,
+            ),
+            peft_config,
+        )
         if DEBUG:
             wrapped_peft.print_trainable_parameters()
         return wrapped_peft, self.tokenizer
 
     @requires_dependencies("peft", extra="fine-tune")
     def apply_adapter(
         self,
```

### Comparing `openllm-0.2.1/src/openllm/_prompt.py` & `openllm-0.2.2/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/_quantisation.py` & `openllm-0.2.2/src/openllm/_quantisation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/_schema.py` & `openllm-0.2.2/src/openllm/_schema.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/_service.py` & `openllm-0.2.2/src/openllm/_service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/_strategies.py` & `openllm-0.2.2/src/openllm/_strategies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/_types.py` & `openllm-0.2.2/src/openllm/_types.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/cli.py` & `openllm-0.2.2/src/openllm/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,39 +69,35 @@
 from bentoml._internal.models.model import ModelStore
 
 from .__about__ import __version__
 from .exceptions import OpenLLMException
 from .utils import DEBUG
 from .utils import ENV_VARS_TRUE_VALUES
 from .utils import EnvVarMixin
-from .utils import LazyLoader
 from .utils import LazyType
 from .utils import analytics
 from .utils import bentoml_cattr
 from .utils import codegen
 from .utils import configure_logging
 from .utils import dantic
 from .utils import first_not_none
 from .utils import get_debug_mode
 from .utils import get_quiet_mode
 from .utils import gpu_count
 from .utils import is_jupyter_available
 from .utils import is_jupytext_available
 from .utils import is_notebook_available
 from .utils import is_peft_available
-from .utils import is_torch_available
 from .utils import is_transformers_supports_agent
 from .utils import resolve_user_filepath
 from .utils import set_debug_mode
 from .utils import set_quiet_mode
 
 
 if t.TYPE_CHECKING:
-    import torch
-
     from bentoml._internal.bento import BentoStore
     from bentoml._internal.container import DefaultBuilder
 
     from ._types import ClickFunctionWrapper
     from ._types import DictStrAny
     from ._types import ListStr
     from ._types import LiteralRuntime
@@ -109,15 +105,14 @@
 
     ServeCommand = t.Literal["serve", "serve-grpc"]
     OutputLiteral = t.Literal["json", "pretty", "porcelain"]
 
     TupleStr = tuple[str, ...]
 else:
     TupleStr = tuple
-    torch = LazyLoader("torch", globals(), "torch")
 
 
 # NOTE: We need to do this so that overload can register
 # correct overloads to typing registry
 if sys.version_info[:2] >= (3, 11):
     from typing import overload
 else:
@@ -1368,17 +1363,14 @@
             msg = f"'{model}' does not exists in local store. Saving..."
             if model_id is not None:
                 msg = f"'{model}' with 'model_id={model_id}' does not exists in local store. Saving..."
             _echo(msg, fg="yellow", nl=True)
 
         _ref = llm.import_model(trust_remote_code=llm.__llm_trust_remote_code__)
 
-        if impl == "pt" and is_torch_available() and torch.cuda.is_available():
-            torch.cuda.empty_cache()
-
     if machine:
         # NOTE: We will prefix the tag with __tag__ and we can use regex to correctly
         # get the tag from 'bentoml.bentos.build|build_bentofile'
         _echo(f"__tag__:{_ref.tag}", fg="white")
     elif output == "pretty":
         if _previously_saved:
             _echo(
@@ -2463,24 +2455,26 @@
 @utils_command.command()
 @click.argument(
     "model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()])
 )
 @click.argument("prompt", type=click.STRING)
 @output_option
 @click.option("--format", type=click.STRING, default=None)
-def get_prompt(model_name: str, prompt: str, format: str | None, output: OutputLiteral):
+def get_prompt(model_name: str, prompt: str, format: str | None, output: OutputLiteral) -> None:
     """Get the default prompt used by OpenLLM."""
     try:
         module = openllm.utils.EnvVarMixin(model_name).module
         template = module.DEFAULT_PROMPT_TEMPLATE
         if callable(template):
             if format is None:
+                if not hasattr(module, "PROMPT_MAPPING") or module.PROMPT_MAPPING is None:
+                    raise RuntimeError("Failed to find prompt mapping while DEFAULT_PROMPT_TEMPLATE is a function.")
                 raise click.BadOptionUsage(
                     "format",
-                    f"{model_name} prompt requires passing '--format' (available format: {module.PROMPT_MAPPING})",
+                    f"{model_name} prompt requires passing '--format' (available format: {list(module.PROMPT_MAPPING)})",
                 )
             _prompt = template(format)
         else:
             _prompt = template
 
         fully_formatted = _prompt.format(instruction=prompt)
```

### Comparing `openllm-0.2.1/src/openllm/client.py` & `openllm-0.2.2/src/openllm/client.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/exceptions.py` & `openllm-0.2.2/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/testing.py` & `openllm-0.2.2/src/openllm/testing.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/bundle/__init__.py` & `openllm-0.2.2/src/openllm/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/bundle/_package.py` & `openllm-0.2.2/src/openllm/bundle/_package.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/bundle/oci/Dockerfile-builder` & `openllm-0.2.2/src/openllm/bundle/oci/Dockerfile-builder`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/bundle/oci/__init__.py` & `openllm-0.2.2/src/openllm/bundle/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/__init__.py` & `openllm-0.2.2/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/auto/__init__.py` & `openllm-0.2.2/src/openllm/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/auto/configuration_auto.py` & `openllm-0.2.2/src/openllm/models/auto/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/auto/factory.py` & `openllm-0.2.2/src/openllm/models/auto/factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/auto/modeling_auto.py` & `openllm-0.2.2/src/openllm/models/auto/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.2.2/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.2.2/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/auto/modeling_vllm_auto.py` & `openllm-0.2.2/src/openllm/models/auto/modeling_vllm_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/baichuan/__init__.py` & `openllm-0.2.2/src/openllm/models/baichuan/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/baichuan/configuration_baichuan.py` & `openllm-0.2.2/src/openllm/models/baichuan/configuration_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/baichuan/modeling_baichuan.py` & `openllm-0.2.2/src/openllm/models/baichuan/modeling_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/chatglm/__init__.py` & `openllm-0.2.2/src/openllm/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.2.2/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.2.2/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.2.2/src/openllm/models/dolly_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.2.2/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.2.2/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/falcon/__init__.py` & `openllm-0.2.2/src/openllm/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.2.2/src/openllm/models/falcon/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.2.2/src/openllm/models/falcon/modeling_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/flan_t5/__init__.py` & `openllm-0.2.2/src/openllm/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.2.2/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.2.2/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.2.2/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.2.2/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.2.2/src/openllm/models/gpt_neox/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/gpt_neox/configuration_gpt_neox.py` & `openllm-0.2.2/src/openllm/models/gpt_neox/configuration_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/gpt_neox/modeling_gpt_neox.py` & `openllm-0.2.2/src/openllm/models/gpt_neox/modeling_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/llama/__init__.py` & `openllm-0.2.2/src/openllm/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/llama/configuration_llama.py` & `openllm-0.2.2/src/openllm/models/llama/configuration_llama.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,23 @@
             "openlm-research/open_llama_13b",
             "huggyllama/llama-65b",
             "huggyllama/llama-30b",
             "huggyllama/llama-13b",
             "huggyllama/llama-7b",
         ],
         "tokenizer_class": "LlamaTokenizerFast",
+        "fine_tune_strategies": (
+            {
+                "adapter_type": "lora",
+                "r": 64,
+                "lora_alpha": 16,
+                "lora_dropout": 0.1,
+                "bias": "none",
+            },
+        ),
     }
 
     class GenerationConfig:
         max_new_tokens: int = 256
         temperature: float = 0.45
         top_p: float = 0.95
         top_k: int = 12
```

### Comparing `openllm-0.2.1/src/openllm/models/llama/modeling_llama.py` & `openllm-0.2.2/src/openllm/models/llama/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/llama/modeling_vllm_llama.py` & `openllm-0.2.2/src/openllm/models/llama/modeling_vllm_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/mpt/__init__.py` & `openllm-0.2.2/src/openllm/models/mpt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/mpt/configuration_mpt.py` & `openllm-0.2.2/src/openllm/models/mpt/configuration_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/mpt/modeling_mpt.py` & `openllm-0.2.2/src/openllm/models/mpt/modeling_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/opt/__init__.py` & `openllm-0.2.2/src/openllm/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/opt/configuration_opt.py` & `openllm-0.2.2/src/openllm/models/opt/configuration_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/opt/modeling_flax_opt.py` & `openllm-0.2.2/src/openllm/models/opt/modeling_flax_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/opt/modeling_opt.py` & `openllm-0.2.2/src/openllm/models/opt/modeling_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/opt/modeling_tf_opt.py` & `openllm-0.2.2/src/openllm/models/opt/modeling_tf_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/stablelm/__init__.py` & `openllm-0.2.2/src/openllm/models/stablelm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.2.2/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.2.2/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/starcoder/__init__.py` & `openllm-0.2.2/src/openllm/models/starcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.2.2/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.2.2/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/playground/__init__.py` & `openllm-0.2.2/src/openllm/playground/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/playground/_meta.yml` & `openllm-0.2.2/src/openllm/playground/_meta.yml`

 * *Files 8% similar despite different names*

```diff
@@ -36,7 +36,15 @@
 
     This script demonstrate how one can fine tune Falcon using [QLoRa](https://arxiv.org/pdf/2305.14314.pdf),
     [trl](https://github.com/lvwerra/trl).
 
     It is trained using OpenAssistant's Guanaco [dataset](https://huggingface.co/datasets/timdettmers/openassistant-guanaco)
 
     It requires at least one GPU to be available, so make sure to have it.
+llama2_qlora:
+  description: |
+    ## Fine tuning LlaMA 2
+    This script demonstrate how one can fine tune Falcon using LoRA with [trl](https://github.com/lvwerra/trl)
+
+    It is trained using the [Dolly datasets](https://huggingface.co/datasets/databricks/databricks-dolly-15k)
+
+    It requires at least one GPU to be available.
```

### Comparing `openllm-0.2.1/src/openllm/playground/falcon_tuned.py` & `openllm-0.2.2/src/openllm/playground/falcon_tuned.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,28 +8,23 @@
 import torch
 
 # import openllm here for OPENLLMDEVDEBUG
 import openllm
 import transformers
 
 
+# Make sure to have at least one GPU to run this script
+
 openllm.utils.configure_logging()
 
 logger = logging.getLogger(__name__)
 
-if len(openllm.utils.gpu_count()) < 1:
-    raise RuntimeError("This script can only be run with system that GPU is available.")
-
-_deps = ["trl", '"openllm[fine-tune]"']
-
-if openllm.utils.DEBUG:
-    logger.info("Installing dependencies to run this script: %s", _deps)
+# On notebook, make sure to install the following
+# ! pip install -U openllm[fine-tune] @ git+https://github.com/bentoml/OpenLLM.git
 
-    if os.system(f"pip install -U {' '.join(_deps)}") != 0:
-        raise SystemExit(1)
 
 from datasets import load_dataset
 from trl import SFTTrainer
 
 
 DEFAULT_MODEL_ID = "ybelkada/falcon-7b-sharded-bf16"
 DATASET_NAME = "timdettmers/openassistant-guanaco"
@@ -109,8 +104,8 @@
 # upcast layernorm in float32 for more stable training
 for name, module in trainer.model.named_modules():
     if "norm" in name:
         module = module.to(torch.float32)
 
 trainer.train()
 
-model.save_pretrained(os.path.join(training_args.output_dir, "lora"))
+trainer.model.save_pretrained(os.path.join(training_args.output_dir, "lora"))
```

### Comparing `openllm-0.2.1/src/openllm/playground/features.py` & `openllm-0.2.2/src/openllm/playground/features.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/playground/opt_tuned.py` & `openllm-0.2.2/src/openllm/playground/opt_tuned.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,22 @@
 import sys
 import typing as t
 
 # import openllm here for OPENLLMDEVDEBUG
 import openllm
 import transformers
 
+# Make sure to have at least one GPU to run this script
 
 openllm.utils.configure_logging()
 
 logger = logging.getLogger(__name__)
 
-if len(openllm.utils.gpu_count()) < 1:
-    raise RuntimeError("This script can only be run with system that GPU is available.")
-
-_deps = ['"openllm[fine-tune]"']
-
-if openllm.utils.DEBUG:
-    logger.info("Installing dependencies to run this script: %s", _deps)
-
-    if os.system(f"pip install -U {' '.join(_deps)}") != 0:
-        raise SystemExit(1)
+# On notebook, make sure to install the following
+# ! pip install -U openllm[fine-tune] @ git+https://github.com/bentoml/OpenLLM.git
 
 from datasets import load_dataset
 
 
 if t.TYPE_CHECKING:
     from peft import PeftModel
 
@@ -98,8 +91,8 @@
 data = data.map(lambda samples: tokenizer(samples["quote"]), batched=True)
 
 trainer = load_trainer(model, tokenizer, data, training_args)
 model.config.use_cache = False  # silence just for warning, reenable for inference later
 
 trainer.train()
 
-model.save_pretrained(os.path.join(training_args.output_dir, "lora"))
+trainer.model.save_pretrained(os.path.join(training_args.output_dir, "lora"))
```

### Comparing `openllm-0.2.1/src/openllm/serialisation/__init__.py` & `openllm-0.2.2/src/openllm/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/serialisation/constants.py` & `openllm-0.2.2/src/openllm/serialisation/constants.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/serialisation/ggml.py` & `openllm-0.2.2/src/openllm/serialisation/ggml.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/serialisation/transformers.py` & `openllm-0.2.2/src/openllm/serialisation/transformers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/utils/__init__.py` & `openllm-0.2.2/src/openllm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/utils/analytics.py` & `openllm-0.2.2/src/openllm/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/utils/codegen.py` & `openllm-0.2.2/src/openllm/utils/codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
         lines,
         args=("_", "fields"),
         globs=globs,
         annotations={"_": "type[LLMConfig]", "fields": fields_ann, "return": fields_ann},
     )
 
 
-def gen_sdk(func: AnyCallable, name: str | None = None, **attrs: t.Any) -> AnyCallable:
+def gen_sdk(func: AnyCallable, name: str | None = None, **attrs: t.Any):
     """Enhance function with nicer Repr."""
     from .representation import ReprMixin
 
     if name is None:
         name = func.__name__.strip("_")
 
     _signatures = inspect.signature(func).parameters
```

### Comparing `openllm-0.2.1/src/openllm/utils/dantic.py` & `openllm-0.2.2/src/openllm/utils/dantic.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.2.2/src/openllm/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.2.2/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.2.2/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/utils/dummy_pt_and_triton_objects.py` & `openllm-0.2.2/src/openllm/utils/dummy_pt_and_triton_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.2.2/src/openllm/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.2.2/src/openllm/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/utils/dummy_vllm_objects.py` & `openllm-0.2.2/src/openllm/utils/dummy_vllm_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/utils/import_utils.py` & `openllm-0.2.2/src/openllm/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/utils/lazy.py` & `openllm-0.2.2/src/openllm/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm/utils/representation.py` & `openllm-0.2.2/src/openllm/utils/representation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm_client/__init__.py` & `openllm-0.2.2/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm_client/_prompt.py` & `openllm-0.2.2/src/openllm_client/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm_client/runtimes/__init__.py` & `openllm-0.2.2/src/openllm_client/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm_client/runtimes/base.py` & `openllm-0.2.2/src/openllm_client/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm_client/runtimes/grpc.py` & `openllm-0.2.2/src/openllm_client/runtimes/grpc.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/src/openllm_client/runtimes/http.py` & `openllm-0.2.2/src/openllm_client/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/__init__.py` & `openllm-0.2.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/client_test.py` & `openllm-0.2.2/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/configuration_test.py` & `openllm-0.2.2/tests/configuration_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/conftest.py` & `openllm-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/llm_test.py` & `openllm-0.2.2/tests/llm_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/models_test.py` & `openllm-0.2.2/tests/models_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/package_test.py` & `openllm-0.2.2/tests/package_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/strategies_test.py` & `openllm-0.2.2/tests/strategies_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/_strategies/__init__.py` & `openllm-0.2.2/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/_strategies/_configuration.py` & `openllm-0.2.2/tests/_strategies/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/models/__init__.py` & `openllm-0.2.2/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/models/conftest.py` & `openllm-0.2.2/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/models/flan_t5_test.py` & `openllm-0.2.2/tests/models/flan_t5_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/models/opt_test.py` & `openllm-0.2.2/tests/models/opt_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json` & `openllm-0.2.2/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json` & `openllm-0.2.2/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/models/__snapshots__/opt_test/test_opt_125m[container].json` & `openllm-0.2.2/tests/models/__snapshots__/opt_test/test_opt_125m[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/tests/models/__snapshots__/opt_test/test_opt_125m[local].json` & `openllm-0.2.2/tests/models/__snapshots__/opt_test/test_opt_125m[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/.gitignore` & `openllm-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/LICENSE.md` & `openllm-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/README.md` & `openllm-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/hatch.toml` & `openllm-0.2.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.1/pyproject.toml` & `openllm-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 baichuan = ["cpm-kernels", "sentencepiece"]
 chatglm = ["cpm-kernels", "sentencepiece"]
 falcon = ["einops", "xformers"]
 fine-tune = ["peft", "bitsandbytes", "datasets", "accelerate", "deepspeed", "trl"]
 flan-t5 = ["flax", "jax", "jaxlib", "tensorflow", "keras"]
 ggml = ["ctransformers"]
 gptq = ["auto-gptq[triton]"]
-llama = ["openllm[vllm]", "fairscale", "sentencepiece"]
+llama = ["fairscale", "sentencepiece"]
 mpt = ["triton", "einops"]
 openai = ["openai", "tiktoken"]
 opt = ["flax", "jax", "jaxlib", "tensorflow", "keras"]
 playground = ["jupyter", "notebook", "ipython", "jupytext", "nbformat"]
 starcoder = ["bitsandbytes"]
 vllm = ["vllm", "ray"]
```

### Comparing `openllm-0.2.1/PKG-INFO` & `openllm-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.2.1
+Version: 0.2.2
 Summary: OpenLLM: Operating LLMs in production
 Project-URL: Blog, https://modelserving.com
 Project-URL: Discord, https://l.bentoml.com/join-openllm-discord
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: GitHub, https://github.com/bentoml/openllm
 Project-URL: History, https://github.com/bentoml/openllm/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
@@ -95,15 +95,14 @@
 Requires-Dist: tensorflow; extra == 'flan-t5'
 Provides-Extra: ggml
 Requires-Dist: ctransformers; extra == 'ggml'
 Provides-Extra: gptq
 Requires-Dist: auto-gptq[triton]; extra == 'gptq'
 Provides-Extra: llama
 Requires-Dist: fairscale; extra == 'llama'
-Requires-Dist: openllm[vllm]; extra == 'llama'
 Requires-Dist: sentencepiece; extra == 'llama'
 Provides-Extra: mpt
 Requires-Dist: einops; extra == 'mpt'
 Requires-Dist: triton; extra == 'mpt'
 Provides-Extra: openai
 Requires-Dist: openai; extra == 'openai'
 Requires-Dist: tiktoken; extra == 'openai'
```

