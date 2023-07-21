# Comparing `tmp/openllm-0.2.2.tar.gz` & `tmp/openllm-0.2.3.tar.gz`

## Comparing `openllm-0.2.2.tar` & `openllm-0.2.3.tar`

### file list

```diff
@@ -1,138 +1,137 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 openllm-0.2.2/.DS_Store
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.2/.gitattributes
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 openllm-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.2/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0    12183 2020-02-02 00:00:00.000000 openllm-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.2/CITATION.cff
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.2/DEVELOPMENT.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.2/nightly-requirements-gpu.txt
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.2/nightly-requirements.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.2/package.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.2/pyoxidizer.bzl
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.2/taplo.toml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/__about__.py
--rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/__main__.py
--rw-r--r--   0        0        0    90069 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_configuration.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_generation.py
--rw-r--r--   0        0        0    67405 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_llm.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_prompt.py
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_quantisation.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_schema.py
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_service.py
--rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_strategies.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/_types.py
--rw-r--r--   0        0        0   101267 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/cli.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/client.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/py.typed
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/testing.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/bundle/__init__.py
--rw-r--r--   0        0        0    14379 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/bundle/_package.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/bundle/oci/Dockerfile-builder
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/bundle/oci/Dockerfile-vllm
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/bundle/oci/__init__.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/auto/modeling_vllm_auto.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/baichuan/__init__.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/baichuan/configuration_baichuan.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/baichuan/modeling_baichuan.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/gpt_neox/configuration_gpt_neox.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/gpt_neox/modeling_gpt_neox.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/llama/configuration_llama.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/llama/modeling_llama.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/llama/modeling_vllm_llama.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/mpt/__init__.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/mpt/configuration_mpt.py
--rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/mpt/modeling_mpt.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/opt/__init__.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/opt/configuration_opt.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/opt/modeling_flax_opt.py
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/opt/modeling_opt.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/opt/modeling_tf_opt.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/__init__.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/_meta.yml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/falcon_tuned.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/features.py
--rw-r--r--   0        0        0     8507 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/llama2_qlora.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/playground/opt_tuned.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/serialisation/__init__.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/serialisation/constants.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/serialisation/ggml.py
--rw-r--r--   0        0        0    16729 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/serialisation/transformers.py
--rw-r--r--   0        0        0    16991 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    19990 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_pt_and_triton_objects.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/dummy_vllm_objects.py
--rw-r--r--   0        0        0    20528 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm/utils/representation.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.2/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/client_test.py
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/configuration_test.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/llm_test.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models_test.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/package_test.py
--rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/strategies_test.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/__init__.py
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/conftest.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/flan_t5_test.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/opt_test.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.2/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.2/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.2/LICENSE.md
--rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.2/README.md
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 openllm-0.2.2/hatch.toml
--rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 openllm-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    30090 2020-02-02 00:00:00.000000 openllm-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.3/.gitattributes
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 openllm-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.3/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0    12268 2020-02-02 00:00:00.000000 openllm-0.2.3/CHANGELOG.md
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.3/CITATION.cff
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.3/DEVELOPMENT.md
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.3/nightly-requirements-gpu.txt
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.3/nightly-requirements.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.3/package.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.3/pyoxidizer.bzl
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.3/taplo.toml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/__about__.py
+-rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/__main__.py
+-rw-r--r--   0        0        0    90069 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_configuration.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_generation.py
+-rw-r--r--   0        0        0    67405 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_llm.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_quantisation.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_schema.py
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_service.py
+-rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_strategies.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_types.py
+-rw-r--r--   0        0        0   101542 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/cli.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/client.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/py.typed
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/testing.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/bundle/__init__.py
+-rw-r--r--   0        0        0    15112 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/bundle/_package.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/bundle/oci/Dockerfile-builder
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/bundle/oci/Dockerfile-vllm
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/bundle/oci/__init__.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/modeling_vllm_auto.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/baichuan/__init__.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/baichuan/configuration_baichuan.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/baichuan/modeling_baichuan.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/gpt_neox/configuration_gpt_neox.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/gpt_neox/modeling_gpt_neox.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/llama/configuration_llama.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/llama/modeling_llama.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/llama/modeling_vllm_llama.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/mpt/__init__.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/mpt/configuration_mpt.py
+-rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/mpt/modeling_mpt.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/opt/__init__.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/opt/configuration_opt.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/opt/modeling_flax_opt.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/opt/modeling_opt.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/opt/modeling_tf_opt.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/__init__.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/_meta.yml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/falcon_tuned.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/features.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/llama2_qlora.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/opt_tuned.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/serialisation/__init__.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/serialisation/constants.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/serialisation/ggml.py
+-rw-r--r--   0        0        0    16729 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/serialisation/transformers.py
+-rw-r--r--   0        0        0    16991 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    19990 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_pt_and_triton_objects.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_vllm_objects.py
+-rw-r--r--   0        0        0    20528 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/representation.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/client_test.py
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/configuration_test.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/llm_test.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models_test.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/package_test.py
+-rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/strategies_test.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/__init__.py
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/conftest.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/flan_t5_test.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/opt_test.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.3/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.3/LICENSE.md
+-rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.3/README.md
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 openllm-0.2.3/hatch.toml
+-rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 openllm-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    30090 2020-02-02 00:00:00.000000 openllm-0.2.3/PKG-INFO
```

### Comparing `openllm-0.2.2/.pre-commit-config.yaml` & `openllm-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/ADDING_NEW_MODEL.md` & `openllm-0.2.3/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/CHANGELOG.md` & `openllm-0.2.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.2.3](https://github.com/bentoml/openllm/tree/v0.2.3)
+No significant changes.
+
+
 ## [0.2.2](https://github.com/bentoml/openllm/tree/v0.2.2)
 No significant changes.
 
 
 ## [0.2.1](https://github.com/bentoml/openllm/tree/v0.2.1)
 No significant changes.
```

### Comparing `openllm-0.2.2/CITATION.cff` & `openllm-0.2.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/DEVELOPMENT.md` & `openllm-0.2.3/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/nightly-requirements.txt` & `openllm-0.2.3/nightly-requirements.txt`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/package.json` & `openllm-0.2.3/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.2.3'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.2.2",
+    "version": "0.2.3",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.2.2/pyoxidizer.bzl` & `openllm-0.2.3/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/__about__.py` & `openllm-0.2.3/src/openllm/__about__.py`

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
-__version__ = "0.2.2"
+__version__ = "0.2.3"
```

### Comparing `openllm-0.2.2/src/openllm/__init__.py` & `openllm-0.2.3/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/__main__.py` & `openllm-0.2.3/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/_configuration.py` & `openllm-0.2.3/src/openllm/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/_generation.py` & `openllm-0.2.3/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/_llm.py` & `openllm-0.2.3/src/openllm/_llm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/_prompt.py` & `openllm-0.2.3/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/_quantisation.py` & `openllm-0.2.3/src/openllm/_quantisation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/_schema.py` & `openllm-0.2.3/src/openllm/_schema.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/_service.py` & `openllm-0.2.3/src/openllm/_service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/_strategies.py` & `openllm-0.2.3/src/openllm/_strategies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/_types.py` & `openllm-0.2.3/src/openllm/_types.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/cli.py` & `openllm-0.2.3/src/openllm/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -2468,22 +2468,27 @@
             if format is None:
                 if not hasattr(module, "PROMPT_MAPPING") or module.PROMPT_MAPPING is None:
                     raise RuntimeError("Failed to find prompt mapping while DEFAULT_PROMPT_TEMPLATE is a function.")
                 raise click.BadOptionUsage(
                     "format",
                     f"{model_name} prompt requires passing '--format' (available format: {list(module.PROMPT_MAPPING)})",
                 )
+            if format not in module.PROMPT_MAPPING:
+                raise click.BadOptionUsage(
+                    "format",
+                    f"Given format {format} is not valid for {model_name} (available format: {list(module.PROMPT_MAPPING)})",
+                )
             _prompt = template(format)
         else:
             _prompt = template
 
         fully_formatted = _prompt.format(instruction=prompt)
 
         if output == "porcelain":
-            _echo(f'__prompt__:"{fully_formatted}"', fg="white")
+            _echo(repr(fully_formatted), fg="white")
         elif output == "json":
             _echo(orjson.dumps({"prompt": fully_formatted}, option=orjson.OPT_INDENT_2).decode(), fg="white")
         else:
             _echo(f"== Prompt for {model_name} ==\n", fg="magenta")
             _echo(fully_formatted, fg="white")
     except AttributeError:
         raise click.ClickException(f"{model_name} does not have default prompt template.") from None
@@ -2494,15 +2499,15 @@
         content = yaml.safe_load(f)
     if not all("description" in k for k in content.values()):
         raise ValueError("Invalid metadata file. All entries must have a 'description' key.")
     return content
 
 
 @cli.command()
-@click.argument("output-dir", default=".")
+@click.argument("output-dir", default=None, required=False)
 @click.option(
     "--port",
     envvar="JUPYTER_PORT",
     show_envvar=True,
     show_default=True,
     default=8888,
     help="Default port for Jupyter server",
```

### Comparing `openllm-0.2.2/src/openllm/client.py` & `openllm-0.2.3/src/openllm/client.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/exceptions.py` & `openllm-0.2.3/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/testing.py` & `openllm-0.2.3/src/openllm/testing.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/bundle/__init__.py` & `openllm-0.2.3/src/openllm/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/bundle/_package.py` & `openllm-0.2.3/src/openllm/bundle/_package.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from bentoml._internal.configuration.containers import BentoMLContainer
 from bentoml._internal.models.model import ModelStore
 
 from ..exceptions import OpenLLMException
 from ..utils import DEBUG
 from ..utils import EnvVarMixin
 from ..utils import codegen
+from ..utils import gpu_count
 from ..utils import is_flax_available
 from ..utils import is_tf_available
 from ..utils import is_torch_available
 from ..utils import pkg
 from ..utils import resolve_user_filepath
 
 
@@ -232,15 +233,15 @@
 
 
 @inject
 def create_bento(
     bento_tag: bentoml.Tag,
     llm_fs: FS,
     llm: openllm.LLM[t.Any, t.Any],
-    workers_per_resource: int | float,
+    workers_per_resource: str | int | float,
     quantize: t.LiteralString | None,
     bettertransformer: bool | None,
     dockerfile_template: str | None,
     adapter_map: dict[str, str | None] | None = None,
     extra_dependencies: tuple[str, ...] | None = None,
     build_ctx: str | None = None,
     runtime: t.Literal["ggml", "transformers"] = "transformers",
@@ -251,14 +252,31 @@
     framework_envvar = llm.config["env"]["framework_value"]
     labels = dict(llm.identifying_params)
     labels.update({"_type": llm.llm_type, "_framework": framework_envvar, "start_name": llm.config["start_name"]})
 
     if adapter_map:
         labels.update(adapter_map)
 
+    if isinstance(workers_per_resource, str):
+        if workers_per_resource == "round_robin":
+            workers_per_resource = 1.0
+        elif workers_per_resource == "conserved":
+            available_gpu = gpu_count()
+            if len(available_gpu) != 0:
+                workers_per_resource = float(1 / len(available_gpu))
+            else:
+                workers_per_resource = 1.0
+        else:
+            try:
+                workers_per_resource = float(workers_per_resource)
+            except ValueError:
+                raise ValueError(
+                    "'workers_per_resource' only accept ['round_robin', 'conserved'] as possible strategies."
+                ) from None
+
     logger.info("Building Bento for '%s'", llm.config["start_name"])
 
     if adapter_map is not None:
         if build_ctx is None:
             raise ValueError("build_ctx is required when 'adapter_map' is not None")
         updated_mapping: dict[str, str | None] = {}
         for adapter_id, name in adapter_map.items():
```

### Comparing `openllm-0.2.2/src/openllm/bundle/oci/Dockerfile-builder` & `openllm-0.2.3/src/openllm/bundle/oci/Dockerfile-builder`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/bundle/oci/__init__.py` & `openllm-0.2.3/src/openllm/bundle/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/__init__.py` & `openllm-0.2.3/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/auto/__init__.py` & `openllm-0.2.3/src/openllm/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/auto/configuration_auto.py` & `openllm-0.2.3/src/openllm/models/auto/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/auto/factory.py` & `openllm-0.2.3/src/openllm/models/auto/factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/auto/modeling_auto.py` & `openllm-0.2.3/src/openllm/models/auto/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.2.3/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.2.3/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/auto/modeling_vllm_auto.py` & `openllm-0.2.3/src/openllm/models/auto/modeling_vllm_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/baichuan/__init__.py` & `openllm-0.2.3/src/openllm/models/baichuan/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/baichuan/configuration_baichuan.py` & `openllm-0.2.3/src/openllm/models/baichuan/configuration_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/baichuan/modeling_baichuan.py` & `openllm-0.2.3/src/openllm/models/baichuan/modeling_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/chatglm/__init__.py` & `openllm-0.2.3/src/openllm/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.2.3/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.2.3/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.2.3/src/openllm/models/dolly_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.2.3/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.2.3/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/falcon/__init__.py` & `openllm-0.2.3/src/openllm/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.2.3/src/openllm/models/falcon/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.2.3/src/openllm/models/falcon/modeling_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/flan_t5/__init__.py` & `openllm-0.2.3/src/openllm/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.2.3/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.2.3/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.2.3/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.2.3/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.2.3/src/openllm/models/gpt_neox/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/gpt_neox/configuration_gpt_neox.py` & `openllm-0.2.3/src/openllm/models/gpt_neox/configuration_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/gpt_neox/modeling_gpt_neox.py` & `openllm-0.2.3/src/openllm/models/gpt_neox/modeling_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/llama/__init__.py` & `openllm-0.2.3/src/openllm/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/llama/configuration_llama.py` & `openllm-0.2.3/src/openllm/models/llama/configuration_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/llama/modeling_llama.py` & `openllm-0.2.3/src/openllm/models/llama/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/llama/modeling_vllm_llama.py` & `openllm-0.2.3/src/openllm/models/llama/modeling_vllm_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/mpt/__init__.py` & `openllm-0.2.3/src/openllm/models/mpt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/mpt/configuration_mpt.py` & `openllm-0.2.3/src/openllm/models/mpt/configuration_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/mpt/modeling_mpt.py` & `openllm-0.2.3/src/openllm/models/mpt/modeling_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/opt/__init__.py` & `openllm-0.2.3/src/openllm/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/opt/configuration_opt.py` & `openllm-0.2.3/src/openllm/models/opt/configuration_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/opt/modeling_flax_opt.py` & `openllm-0.2.3/src/openllm/models/opt/modeling_flax_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/opt/modeling_opt.py` & `openllm-0.2.3/src/openllm/models/opt/modeling_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/opt/modeling_tf_opt.py` & `openllm-0.2.3/src/openllm/models/opt/modeling_tf_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/stablelm/__init__.py` & `openllm-0.2.3/src/openllm/models/stablelm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.2.3/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.2.3/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/starcoder/__init__.py` & `openllm-0.2.3/src/openllm/models/starcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.2.3/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.2.3/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/playground/__init__.py` & `openllm-0.2.3/src/openllm/playground/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/playground/_meta.yml` & `openllm-0.2.3/src/openllm/playground/_meta.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/playground/falcon_tuned.py` & `openllm-0.2.3/src/openllm/playground/falcon_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/playground/features.py` & `openllm-0.2.3/src/openllm/playground/features.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/playground/llama2_qlora.py` & `openllm-0.2.3/src/openllm/playground/llama2_qlora.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
 @dataclasses.dataclass
 class TrainingArguments:
     per_device_train_batch_size: int = dataclasses.field(default=1)
     gradient_checkpointing: bool = dataclasses.field(default=True)
     bf16: bool = dataclasses.field(default=torch.cuda.get_device_capability()[0] == 8)
     learning_rate: float = dataclasses.field(default=5e-5)
-    epochs: int = dataclasses.field(default=3)
+    num_train_epochs: int = dataclasses.field(default=3)
     logging_steps: int = dataclasses.field(default=1)
     logging_strategy: str = dataclasses.field(default="steps")
     output_dir: str = dataclasses.field(default=os.path.join(os.getcwd(), "outputs", "llama"))
     save_strategy: str = dataclasses.field(default="no")
 
 
 @dataclasses.dataclass
```

### Comparing `openllm-0.2.2/src/openllm/playground/opt_tuned.py` & `openllm-0.2.3/src/openllm/playground/opt_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/serialisation/__init__.py` & `openllm-0.2.3/src/openllm/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/serialisation/constants.py` & `openllm-0.2.3/src/openllm/serialisation/constants.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/serialisation/ggml.py` & `openllm-0.2.3/src/openllm/serialisation/ggml.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/serialisation/transformers.py` & `openllm-0.2.3/src/openllm/serialisation/transformers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/__init__.py` & `openllm-0.2.3/src/openllm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/analytics.py` & `openllm-0.2.3/src/openllm/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/codegen.py` & `openllm-0.2.3/src/openllm/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/dantic.py` & `openllm-0.2.3/src/openllm/utils/dantic.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.2.3/src/openllm/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.2.3/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.2.3/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/dummy_pt_and_triton_objects.py` & `openllm-0.2.3/src/openllm/utils/dummy_pt_and_triton_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.2.3/src/openllm/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.2.3/src/openllm/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/dummy_vllm_objects.py` & `openllm-0.2.3/src/openllm/utils/dummy_vllm_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/import_utils.py` & `openllm-0.2.3/src/openllm/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/lazy.py` & `openllm-0.2.3/src/openllm/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm/utils/representation.py` & `openllm-0.2.3/src/openllm/utils/representation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm_client/__init__.py` & `openllm-0.2.3/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm_client/_prompt.py` & `openllm-0.2.3/src/openllm_client/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm_client/runtimes/__init__.py` & `openllm-0.2.3/src/openllm_client/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm_client/runtimes/base.py` & `openllm-0.2.3/src/openllm_client/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm_client/runtimes/grpc.py` & `openllm-0.2.3/src/openllm_client/runtimes/grpc.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/src/openllm_client/runtimes/http.py` & `openllm-0.2.3/src/openllm_client/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/__init__.py` & `openllm-0.2.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/client_test.py` & `openllm-0.2.3/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/configuration_test.py` & `openllm-0.2.3/tests/configuration_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/conftest.py` & `openllm-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/llm_test.py` & `openllm-0.2.3/tests/llm_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/models_test.py` & `openllm-0.2.3/tests/models_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/package_test.py` & `openllm-0.2.3/tests/package_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/strategies_test.py` & `openllm-0.2.3/tests/strategies_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/_strategies/__init__.py` & `openllm-0.2.3/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/_strategies/_configuration.py` & `openllm-0.2.3/tests/_strategies/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/models/__init__.py` & `openllm-0.2.3/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/models/conftest.py` & `openllm-0.2.3/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/models/flan_t5_test.py` & `openllm-0.2.3/tests/models/flan_t5_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/models/opt_test.py` & `openllm-0.2.3/tests/models/opt_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json` & `openllm-0.2.3/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json` & `openllm-0.2.3/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/models/__snapshots__/opt_test/test_opt_125m[container].json` & `openllm-0.2.3/tests/models/__snapshots__/opt_test/test_opt_125m[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/tests/models/__snapshots__/opt_test/test_opt_125m[local].json` & `openllm-0.2.3/tests/models/__snapshots__/opt_test/test_opt_125m[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/.gitignore` & `openllm-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/LICENSE.md` & `openllm-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/README.md` & `openllm-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/hatch.toml` & `openllm-0.2.3/hatch.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/pyproject.toml` & `openllm-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.2/PKG-INFO` & `openllm-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.2.2
+Version: 0.2.3
 Summary: OpenLLM: Operating LLMs in production
 Project-URL: Blog, https://modelserving.com
 Project-URL: Discord, https://l.bentoml.com/join-openllm-discord
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: GitHub, https://github.com/bentoml/openllm
 Project-URL: History, https://github.com/bentoml/openllm/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
```

