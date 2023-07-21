# Comparing `tmp/openllm-0.2.3.tar.gz` & `tmp/openllm-0.2.4.tar.gz`

## Comparing `openllm-0.2.3.tar` & `openllm-0.2.4.tar`

### file list

```diff
@@ -1,137 +1,137 @@
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.3/.gitattributes
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 openllm-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.3/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0    12268 2020-02-02 00:00:00.000000 openllm-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.3/CITATION.cff
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.3/DEVELOPMENT.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.3/nightly-requirements-gpu.txt
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.3/nightly-requirements.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.3/package.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.3/pyoxidizer.bzl
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.3/taplo.toml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/__about__.py
--rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/__main__.py
--rw-r--r--   0        0        0    90069 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_configuration.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_generation.py
--rw-r--r--   0        0        0    67405 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_llm.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_prompt.py
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_quantisation.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_schema.py
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_service.py
--rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_strategies.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/_types.py
--rw-r--r--   0        0        0   101542 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/cli.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/client.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/py.typed
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/testing.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/bundle/__init__.py
--rw-r--r--   0        0        0    15112 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/bundle/_package.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/bundle/oci/Dockerfile-builder
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/bundle/oci/Dockerfile-vllm
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/bundle/oci/__init__.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/auto/modeling_vllm_auto.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/baichuan/__init__.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/baichuan/configuration_baichuan.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/baichuan/modeling_baichuan.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/gpt_neox/configuration_gpt_neox.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/gpt_neox/modeling_gpt_neox.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/llama/configuration_llama.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/llama/modeling_llama.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/llama/modeling_vllm_llama.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/mpt/__init__.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/mpt/configuration_mpt.py
--rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/mpt/modeling_mpt.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/opt/__init__.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/opt/configuration_opt.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/opt/modeling_flax_opt.py
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/opt/modeling_opt.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/opt/modeling_tf_opt.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/__init__.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/_meta.yml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/falcon_tuned.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/features.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/llama2_qlora.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/playground/opt_tuned.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/serialisation/__init__.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/serialisation/constants.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/serialisation/ggml.py
--rw-r--r--   0        0        0    16729 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/serialisation/transformers.py
--rw-r--r--   0        0        0    16991 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    19990 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_pt_and_triton_objects.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/dummy_vllm_objects.py
--rw-r--r--   0        0        0    20528 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm/utils/representation.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.3/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/client_test.py
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/configuration_test.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/llm_test.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models_test.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/package_test.py
--rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/strategies_test.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/__init__.py
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/conftest.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/flan_t5_test.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/opt_test.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.3/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.3/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.3/LICENSE.md
--rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.3/README.md
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 openllm-0.2.3/hatch.toml
--rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 openllm-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    30090 2020-02-02 00:00:00.000000 openllm-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.4/.gitattributes
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 openllm-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.4/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0    12353 2020-02-02 00:00:00.000000 openllm-0.2.4/CHANGELOG.md
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.4/CITATION.cff
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.4/DEVELOPMENT.md
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.4/nightly-requirements-gpu.txt
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.4/nightly-requirements.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.4/package.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.4/pyoxidizer.bzl
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.4/taplo.toml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/__about__.py
+-rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/__main__.py
+-rw-r--r--   0        0        0    90069 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_configuration.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_generation.py
+-rw-r--r--   0        0        0    67205 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_llm.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_quantisation.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_schema.py
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_service.py
+-rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_strategies.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_types.py
+-rw-r--r--   0        0        0   100438 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/cli.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/client.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/py.typed
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/testing.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/bundle/__init__.py
+-rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/bundle/_package.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/bundle/oci/Dockerfile-builder
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/bundle/oci/Dockerfile-vllm
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/bundle/oci/__init__.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/modeling_vllm_auto.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/baichuan/__init__.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/baichuan/configuration_baichuan.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/baichuan/modeling_baichuan.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/gpt_neox/configuration_gpt_neox.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/gpt_neox/modeling_gpt_neox.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/llama/configuration_llama.py
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/llama/modeling_llama.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/llama/modeling_vllm_llama.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/mpt/__init__.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/mpt/configuration_mpt.py
+-rw-r--r--   0        0        0     8006 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/mpt/modeling_mpt.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/opt/__init__.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/opt/configuration_opt.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/opt/modeling_flax_opt.py
+-rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/opt/modeling_opt.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/opt/modeling_tf_opt.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/__init__.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/_meta.yml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/falcon_tuned.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/features.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/llama2_qlora.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/opt_tuned.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/serialisation/__init__.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/serialisation/constants.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/serialisation/ggml.py
+-rw-r--r--   0        0        0    17424 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/serialisation/transformers.py
+-rw-r--r--   0        0        0    17096 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    20006 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_pt_and_triton_objects.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_vllm_objects.py
+-rw-r--r--   0        0        0    20528 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/representation.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/client_test.py
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/configuration_test.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/llm_test.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models_test.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/package_test.py
+-rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/strategies_test.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/__init__.py
+-rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/conftest.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/flan_t5_test.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/opt_test.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.4/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.4/LICENSE.md
+-rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.4/README.md
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 openllm-0.2.4/hatch.toml
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 openllm-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    30097 2020-02-02 00:00:00.000000 openllm-0.2.4/PKG-INFO
```

### Comparing `openllm-0.2.3/.pre-commit-config.yaml` & `openllm-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/ADDING_NEW_MODEL.md` & `openllm-0.2.4/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/CHANGELOG.md` & `openllm-0.2.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.2.4](https://github.com/bentoml/openllm/tree/v0.2.4)
+No significant changes.
+
+
 ## [0.2.3](https://github.com/bentoml/openllm/tree/v0.2.3)
 No significant changes.
 
 
 ## [0.2.2](https://github.com/bentoml/openllm/tree/v0.2.2)
 No significant changes.
```

### Comparing `openllm-0.2.3/CITATION.cff` & `openllm-0.2.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/DEVELOPMENT.md` & `openllm-0.2.4/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/nightly-requirements.txt` & `openllm-0.2.4/nightly-requirements.txt`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/package.json` & `openllm-0.2.4/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.2.4'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.2.3",
+    "version": "0.2.4",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.2.3/pyoxidizer.bzl` & `openllm-0.2.4/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/__about__.py` & `openllm-0.2.4/src/openllm/__about__.py`

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
-__version__ = "0.2.3"
+__version__ = "0.2.4"
```

### Comparing `openllm-0.2.3/src/openllm/__init__.py` & `openllm-0.2.4/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/__main__.py` & `openllm-0.2.4/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/_configuration.py` & `openllm-0.2.4/src/openllm/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/_generation.py` & `openllm-0.2.4/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/_llm.py` & `openllm-0.2.4/src/openllm/_llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 from .utils import MYPY
 from .utils import EnvVarMixin
 from .utils import LazyLoader
 from .utils import ReprMixin
 from .utils import bentoml_cattr
 from .utils import codegen
 from .utils import first_not_none
-from .utils import get_debug_mode
 from .utils import in_docker
 from .utils import is_peft_available
 from .utils import is_torch_available
 from .utils import non_intrusive_setattr
 from .utils import normalize_attrs_to_model_tokenizer_pair
 from .utils import pkg
 from .utils import requires_dependencies
@@ -970,39 +969,35 @@
         """This utility function will download the model if it doesn't exist yet.
 
         Make sure to call this function if 'ensure_available' is not set during
         Auto LLM initialisation.
 
         The equivalent for ``openllm.Runner`` is ``openllm.Runner.download_model``.
         """
-        additional_args: list[str] = []
-        if not get_debug_mode():
-            additional_args.append("--quiet")
         return openllm.import_model(
             self.config["start_name"],
             model_id=self.model_id,
             model_version=self._model_version,
             runtime=self.runtime,
             implementation=self.__llm_implementation__,
             quantize=self._quantize_method,
             serialisation_format=self._serialisation_format,
-            additional_args=additional_args,
         )
 
     @property
     def _bentomodel(self) -> bentoml.Model:
         if self.__llm_bentomodel__ is None:
             self.__llm_bentomodel__ = openllm.serialisation.get(self)
         return self.__llm_bentomodel__
 
     @property
     def model(self) -> M:
         """The model to use for this LLM. This shouldn't be set at runtime, rather let OpenLLM handle it."""
         # Run check for GPU
-        if self.config["requires_gpu"] and len(openllm.utils.gpu_count()) < 1:
+        if self.config["requires_gpu"] and openllm.utils.device_count() < 1:
             raise GpuNotAvailableError(f"{self} only supports running with GPU (None available).") from None
 
         if self.__llm_model__ is None:
             self.__llm_model__ = t.cast(
                 M, openllm.serialisation.load_model(self, *self._model_decls, **self._model_attrs)
             )
         return t.cast(M, self.__llm_model__)
```

### Comparing `openllm-0.2.3/src/openllm/_prompt.py` & `openllm-0.2.4/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/_quantisation.py` & `openllm-0.2.4/src/openllm/_quantisation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/_schema.py` & `openllm-0.2.4/src/openllm/_schema.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/_service.py` & `openllm-0.2.4/src/openllm/_service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/_strategies.py` & `openllm-0.2.4/src/openllm/_strategies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/_types.py` & `openllm-0.2.4/src/openllm/_types.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/cli.py` & `openllm-0.2.4/src/openllm/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 import attr
 import click
 import click_option_group as cog
 import fs
 import fs.errors
 import inflection
 import orjson
-import psutil
 import yaml
 from bentoml_cli.utils import BentoMLCommandGroup
 from bentoml_cli.utils import opt_callback
 from simple_di import Provide
 from simple_di import inject
 
 import bentoml
@@ -69,35 +68,42 @@
 from bentoml._internal.models.model import ModelStore
 
 from .__about__ import __version__
 from .exceptions import OpenLLMException
 from .utils import DEBUG
 from .utils import ENV_VARS_TRUE_VALUES
 from .utils import EnvVarMixin
+from .utils import LazyLoader
 from .utils import LazyType
 from .utils import analytics
+from .utils import available_devices
 from .utils import bentoml_cattr
 from .utils import codegen
 from .utils import configure_logging
 from .utils import dantic
+from .utils import device_count
 from .utils import first_not_none
 from .utils import get_debug_mode
 from .utils import get_quiet_mode
-from .utils import gpu_count
 from .utils import is_jupyter_available
 from .utils import is_jupytext_available
 from .utils import is_notebook_available
 from .utils import is_peft_available
+from .utils import is_torch_available
 from .utils import is_transformers_supports_agent
 from .utils import resolve_user_filepath
 from .utils import set_debug_mode
 from .utils import set_quiet_mode
 
 
 if t.TYPE_CHECKING:
+    import jupytext
+    import nbformat
+    import torch
+
     from bentoml._internal.bento import BentoStore
     from bentoml._internal.container import DefaultBuilder
 
     from ._types import ClickFunctionWrapper
     from ._types import DictStrAny
     from ._types import ListStr
     from ._types import LiteralRuntime
@@ -105,14 +111,17 @@
 
     ServeCommand = t.Literal["serve", "serve-grpc"]
     OutputLiteral = t.Literal["json", "pretty", "porcelain"]
 
     TupleStr = tuple[str, ...]
 else:
     TupleStr = tuple
+    torch = LazyLoader("torch", globals(), "torch")
+    jupytext = LazyLoader("jupytext", globals(), "jupytext")
+    nbformat = LazyLoader("nbformat", globals(), "nbformat")
 
 
 # NOTE: We need to do this so that overload can register
 # correct overloads to typing registry
 if sys.version_info[:2] >= (3, 11):
     from typing import overload
 else:
@@ -153,15 +162,15 @@
     if not LazyType(TupleStr).isinstance(value):
         ctx.fail(f"{param} only accept multiple values, not {type(value)} (value: {value})")
 
     el: TupleStr = tuple(i for k in value for i in k)
 
     # NOTE: --device all is a special case
     if len(el) == 1 and el[0] == "all":
-        return tuple(map(str, gpu_count()))
+        return tuple(map(str, available_devices()))
 
     return el
 
 
 def _echo(text: t.Any, fg: str = "green", _with_style: bool = True, **attrs: t.Any) -> None:
     call = click.echo
     if _with_style:
@@ -847,24 +856,21 @@
 
     return noop
 
 
 def prerequisite_check(
     ctx: click.Context,
     llm_config: openllm.LLMConfig,
-    gpu_available: tuple[str, ...],
     quantize: t.LiteralString | None,
     adapter_map: dict[str, str | None] | None,
     num_workers: int,
 ) -> None:
-    if get_debug_mode():
-        _echo("Running prerequisite check.", fg="magenta")
     if quantize:
-        if len(gpu_available) < 1:
-            _echo(f"Quantization requires at least 1 GPU (got {len(gpu_available)})", fg="red")
+        if device_count() < 1:
+            _echo("Quantization requires at least 1 GPU (got None)", fg="red")
             ctx.exit(1)
 
     if adapter_map and not is_peft_available():
         _echo(
             "Using adapter requires 'peft' to be available. Make sure to install with 'pip install \"openllm[fine-tune]\"'",
             fg="red",
         )
@@ -875,35 +881,34 @@
         missing_requirements = [i for i in requirements if importlib.util.find_spec(i) is None]
         if len(missing_requirements) > 0:
             _echo(
                 f"Make sure to have the following dependencies available: {missing_requirements}",
                 fg="yellow",
             )
 
-    if num_workers > 1 and len(gpu_available) < num_workers:
+    if num_workers > 1 and device_count() < num_workers:
         raise click.BadOptionUsage(
             "workers_per_resource",
             f"# of workers is infered to {num_workers} GPUs per runner worker, while there are only"
-            f"'{gpu_available}' for inference. (Tip: Try again using '--workers-per-resource={1/len(gpu_available)}')",
+            f"'{device_count()}' for inference. (Tip: Try again using '--workers-per-resource={1/device_count()}')",
             ctx=ctx,
         )
 
 
 _wpr_strategies = {"round_robin", "conserved"}
 
 
 def start_bento(
     group: click.Group,
     bento: bentoml.Bento,
     llm_config: openllm.LLMConfig,
     serve_grpc: bool,
     **command_attrs: t.Any,
 ) -> click.Command:
-    gpu_available = gpu_count()
-    if llm_config["requires_gpu"] and len(gpu_available) < 1:
+    if llm_config["requires_gpu"] and device_count() < 1:
         return noop_command(
             group, llm_config, f"No GPU available, while {bento!r} requires GPU to run.", **command_attrs
         )
 
     command_attrs["help"] = start_bento_docstring(bento, llm_config, serve_grpc)
 
     # Now we have to format the model_id accordingly based on the model_fs
@@ -956,22 +961,16 @@
 
         workers_per_resource = first_not_none(workers_per_resource, default=config["workers_per_resource"])
 
         if isinstance(workers_per_resource, str):
             if workers_per_resource == "round_robin":
                 workers_per_resource = 1.0
             elif workers_per_resource == "conserved":
-                if device:
-                    available_gpu = device
-                else:
-                    available_gpu = gpu_count()
-                if len(available_gpu) != 0:
-                    workers_per_resource = float(1 / len(available_gpu))
-                else:
-                    workers_per_resource = 1.0
+                available_gpu = device if device else available_devices()
+                workers_per_resource = 1.0 if len(available_gpu) == 0 else float(1 / len(available_gpu))
             else:
                 try:
                     workers_per_resource = float(workers_per_resource)
                 except ValueError:
                     ctx.fail(f"'workers_per_resource' only accept '{_wpr_strategies}' as possible strategies.")
 
         num_workers = int(1 / workers_per_resource)
@@ -981,29 +980,29 @@
             config["model_name"],
             config["default_implementation"],
             bettertransformer=bettertransformer,
             quantize=quantize,
             runtime=runtime,
         )
 
-        prerequisite_check(ctx, config, gpu_available, quantize, adapter_map, num_workers)
+        prerequisite_check(ctx, config, quantize, adapter_map, num_workers)
 
         # NOTE: This is to set current configuration
         start_env = os.environ.copy()
         start_env = parse_config_options(config, server_timeout, workers_per_resource, device, start_env)
 
         if fast:
             _echo(f"Fast mode has no effects when 'start' {bento.tag!s}", fg="yellow")
 
         start_env.update(
             {
                 env.framework: env.framework_value,
                 env.config: config.model_dump_json().decode(),
                 env.runtime: env.runtime_value,
-                "BENTOML_DEBUG": str(get_debug_mode()),
+                "BENTOML_DEBUG": str(not get_quiet_mode()),
                 "BENTOML_HOME": os.environ.get("BENTOML_HOME", BentoMLContainer.bentoml_home.get()),
                 "OPENLLM_MODEL_ID": model.path,
                 "OPENLLM_SERIALIZATION": serialisation_format,
             }
         )
 
         if adapter_map:
@@ -1017,31 +1016,20 @@
 
         if serve_grpc:
             server = bentoml.GrpcServer(bento, **server_attrs)
         else:
             server = bentoml.HTTPServer(bento, **server_attrs)
         analytics.track_start_init(config)
 
-        if not get_debug_mode():
+        if return_process:
             server.start(env=start_env, text=True)
             process = server.process
             if process is None:
                 raise click.ClickException("Failed to start the server.")
-
-            if return_process:
-                return process
-
-            try:
-                assert process.stdout
-                with process:
-                    for line in iter(process.stdout.readline, b""):
-                        _echo(line.strip(), fg="white")
-            except Exception as err:
-                _echo(f"Error caught while running LLM Server: \n{err}", fg="red")
-                raise
+            return process
         else:
             try:
                 server.start(env=start_env, text=True, blocking=True)
             except Exception as err:
                 _echo(f"Error caught while running LLM Server:\n{err}", fg="red")
 
         # NOTE: Return the configuration for telemetry purposes.
@@ -1053,16 +1041,15 @@
 def start_model(
     group: click.Group,
     model_name: str,
     llm_config: openllm.LLMConfig,
     serve_grpc: bool,
     **command_attrs: t.Any,
 ) -> click.Command:
-    gpu_available = gpu_count()
-    if llm_config["requires_gpu"] and len(gpu_available) < 1:
+    if llm_config["requires_gpu"] and device_count() < 1:
         # NOTE: The model requires GPU, therefore we will return a dummy command
         command_attrs.update(
             {
                 "short_help": "(Disabled because there is no GPU available)",
                 "help": f"""{model_name} is currently not available to run on your
                 local machine because it requires GPU for inference.""",
             }
@@ -1108,22 +1095,16 @@
 
         workers_per_resource = first_not_none(workers_per_resource, default=config["workers_per_resource"])
 
         if isinstance(workers_per_resource, str):
             if workers_per_resource == "round_robin":
                 workers_per_resource = 1.0
             elif workers_per_resource == "conserved":
-                if device:
-                    available_gpu = device
-                else:
-                    available_gpu = gpu_count()
-                if len(available_gpu) != 0:
-                    workers_per_resource = float(1 / len(available_gpu))
-                else:
-                    workers_per_resource = 1.0
+                available_gpu = device if device else available_devices()
+                workers_per_resource = 1.0 if len(available_gpu) == 0 else float(1 / len(available_gpu))
             else:
                 try:
                     workers_per_resource = float(workers_per_resource)
                 except ValueError:
                     ctx.fail(f"'workers_per_resource' only accept '{_wpr_strategies}' as possible strategies.")
 
         num_workers = int(1 / workers_per_resource)
@@ -1133,30 +1114,30 @@
             config["model_name"],
             config["default_implementation"],
             bettertransformer=bettertransformer,
             quantize=quantize,
             runtime=runtime,
         )
 
-        prerequisite_check(ctx, config, gpu_available, quantize, adapter_map, num_workers)
+        prerequisite_check(ctx, config, quantize, adapter_map, num_workers)
 
         # NOTE: This is to set current configuration
         start_env = os.environ.copy()
         start_env = parse_config_options(config, server_timeout, workers_per_resource, device, start_env)
 
         if fast and not get_quiet_mode():
             _echo(
                 f"Fast mode is enabled. Make sure the model is available in local store before 'start': 'openllm import {model_name}{'--model-id ' + model_id if model_id else ''}'",
                 fg="yellow",
             )
 
         start_env.update(
             {
                 env.framework: env.framework_value,
-                "BENTOML_DEBUG": str(get_debug_mode()),
+                "BENTOML_DEBUG": str(not get_quiet_mode()),
                 "BENTOML_HOME": os.environ.get("BENTOML_HOME", BentoMLContainer.bentoml_home.get()),
                 "OPENLLM_SERIALIZATION": serialisation_format,
             }
         )
 
         if adapter_map:
             _echo(f"OpenLLM will convert '{model_name}' to use provided adapters layers: {list(adapter_map)}")
@@ -1208,35 +1189,20 @@
                     ]
                 )
             _echo(
                 f"\n🚀 Next step: run '{cmd_name}' to create a Bento for {model_name}",
                 fg="blue",
             )
 
-        if not get_debug_mode():
+        if return_process:
             server.start(env=start_env, text=True)
             process = server.process
             if process is None:
                 raise click.ClickException("Failed to start the server.")
-
-            if return_process:
-                return process
-
-            try:
-                assert process.stdout
-                with process:
-                    for line in iter(process.stdout.readline, b""):
-                        _echo(line.strip(), fg="white")
-            except Exception as err:
-                _echo(f"Error caught while running LLM Server: \n{err}", fg="red")
-                raise
-            except KeyboardInterrupt:
-                next_step(model_name, adapter_map)
-            else:
-                next_step(model_name, adapter_map)
+            return process
         else:
             try:
                 server.start(env=start_env, text=True, blocking=True)
             except KeyboardInterrupt:
                 next_step(model_name, adapter_map)
             except Exception as err:
                 _echo(f"Error caught while running LLM Server:\n{err}", fg="red")
@@ -1363,14 +1329,17 @@
             msg = f"'{model}' does not exists in local store. Saving..."
             if model_id is not None:
                 msg = f"'{model}' with 'model_id={model_id}' does not exists in local store. Saving..."
             _echo(msg, fg="yellow", nl=True)
 
         _ref = llm.import_model(trust_remote_code=llm.__llm_trust_remote_code__)
 
+        if impl == "pt" and is_torch_available() and torch.cuda.is_available():
+            torch.cuda.empty_cache()
+
     if machine:
         # NOTE: We will prefix the tag with __tag__ and we can use regex to correctly
         # get the tag from 'bentoml.bentos.build|build_bentofile'
         _echo(f"__tag__:{_ref.tag}", fg="white")
     elif output == "pretty":
         if _previously_saved:
             _echo(
@@ -1994,18 +1963,15 @@
             _echo(
                 "📖 Next steps:\n\n"
                 + "* Serving BentoLLM locally with 'openllm start':\n"
                 + f"    $ openllm start {bento.tag}\n\n"
                 + "* Push to BentoCloud with 'bentoml push':\n"
                 + f"    $ bentoml push {bento.tag}\n\n"
                 + "* Containerize your Bento with 'bentoml containerize':\n"
-                + f"    $ bentoml containerize {bento.tag}"
-                + " --opt progress=plain"
-                if get_debug_mode()
-                else ""
+                + f"    $ bentoml containerize {bento.tag} --opt progress=plain"
                 + "\n\n"
                 + "    Tip: To enable additional BentoML features for 'containerize', "
                 + "use '--enable-features=FEATURE[,FEATURE]' "
                 + "[see 'bentoml containerize -h' for more advanced usage]\n",
                 fg="blue",
             )
     elif output == "json":
@@ -2208,30 +2174,22 @@
 
             if show_available:
                 assert ids_in_local_store is not None
                 if len(ids_in_local_store) == 0:
                     _echo("No models available locally.")
                     ctx.exit(0)
 
-                _available = [[k + "\n\n" * len(v), [str(i.tag) for i in v]] for k, v in ids_in_local_store.items()]
-                column_widths = [int(COLUMNS / 2), int(COLUMNS / 2)]
-                table = tabulate.tabulate(
-                    _available,
-                    tablefmt="fancy_grid",
-                    headers=["Model Id", "Models"],
-                    maxcolwidths=column_widths,
+                _echo("The following are available in local store:", fg="magenta")
+                _echo(
+                    orjson.dumps(
+                        {k: [str(i.tag) for i in val] for k, val in ids_in_local_store.items()},
+                        option=orjson.OPT_INDENT_2,
+                    ).decode(),
+                    fg="white",
                 )
-                _echo("The following models are available in local store:\n", fg="magenta")
-
-                formatted_table = ""
-                for line in table.split("\n"):
-                    formatted_table += (
-                        "".join(f"{cell:{width}}" for cell, width in zip(line.split("\t"), column_widths)) + "\n"
-                    )
-                _echo(formatted_table, fg="white")
         else:
             if show_available:
                 assert ids_in_local_store
                 json_data["local"] = [bentoml_cattr.unstructure(i.tag) for m in ids_in_local_store.values() for i in m]
             _echo(
                 orjson.dumps(
                     json_data,
@@ -2449,14 +2407,28 @@
 
 @cli.group(name="utils")
 def utils_command() -> None:
     """Utilities Subcommand group."""
 
 
 @utils_command.command()
+@click.pass_context
+def list_bentos(ctx: click.Context):
+    """List available bentos built by OpenLLM."""
+    _local_bentos = {str(i.tag): i.info.labels["start_name"] for i in bentoml.list() if "start_name" in i.info.labels}
+    mapping = {
+        k: [tag for tag, name in _local_bentos.items() if name == k]
+        for k in tuple(inflection.dasherize(key) for key in openllm.CONFIG_MAPPING.keys())
+    }
+    mapping = {k: v for k, v in mapping.items() if v}
+    _echo(orjson.dumps(mapping, option=orjson.OPT_INDENT_2).decode(), fg="white")
+    ctx.exit(0)
+
+
+@utils_command.command()
 @click.argument(
     "model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()])
 )
 @click.argument("prompt", type=click.STRING)
 @output_option
 @click.option("--format", type=click.STRING, default=None)
 def get_prompt(model_name: str, prompt: str, format: str | None, output: OutputLiteral) -> None:
@@ -2530,18 +2502,14 @@
     \b
     > Note: This command requires Jupyter to be installed. Install it with 'pip install "openllm[playground]"'
     """
     if not is_jupyter_available() or not is_jupytext_available() or not is_notebook_available():
         raise RuntimeError(
             "Playground requires 'jupyter', 'jupytext', and 'notebook'. Install it with 'pip install \"openllm[playground]\"'"
         )
-
-    import jupytext
-    import nbformat
-
     metadata = load_notebook_metadata()
     _temp_dir = False
     if output_dir is None:
         _temp_dir = True
         output_dir = tempfile.mkdtemp(prefix="openllm-playground-")
     else:
         os.makedirs(os.path.abspath(os.path.expandvars(os.path.expanduser(output_dir))), exist_ok=True)
@@ -2583,13 +2551,9 @@
     except KeyboardInterrupt:
         _echo("\nShutting down Jupyter server...", fg="yellow")
         if _temp_dir:
             _echo("Note: You can access the generated notebooks in: " + output_dir, fg="blue")
     ctx.exit(0)
 
 
-if psutil.WINDOWS:
-    sys.stdout.reconfigure(encoding="utf-8")  # type: ignore
-
-
 if __name__ == "__main__":
     cli()
```

### Comparing `openllm-0.2.3/src/openllm/client.py` & `openllm-0.2.4/src/openllm/client.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/exceptions.py` & `openllm-0.2.4/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/testing.py` & `openllm-0.2.4/src/openllm/testing.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/bundle/__init__.py` & `openllm-0.2.4/src/openllm/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/bundle/_package.py` & `openllm-0.2.4/src/openllm/bundle/_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from bentoml._internal.configuration.containers import BentoMLContainer
 from bentoml._internal.models.model import ModelStore
 
 from ..exceptions import OpenLLMException
 from ..utils import DEBUG
 from ..utils import EnvVarMixin
 from ..utils import codegen
-from ..utils import gpu_count
+from ..utils import device_count
 from ..utils import is_flax_available
 from ..utils import is_tf_available
 from ..utils import is_torch_available
 from ..utils import pkg
 from ..utils import resolve_user_filepath
 
 
@@ -256,19 +256,15 @@
     if adapter_map:
         labels.update(adapter_map)
 
     if isinstance(workers_per_resource, str):
         if workers_per_resource == "round_robin":
             workers_per_resource = 1.0
         elif workers_per_resource == "conserved":
-            available_gpu = gpu_count()
-            if len(available_gpu) != 0:
-                workers_per_resource = float(1 / len(available_gpu))
-            else:
-                workers_per_resource = 1.0
+            workers_per_resource = 1.0 if device_count() == 0 else float(1 / device_count())
         else:
             try:
                 workers_per_resource = float(workers_per_resource)
             except ValueError:
                 raise ValueError(
                     "'workers_per_resource' only accept ['round_robin', 'conserved'] as possible strategies."
                 ) from None
```

### Comparing `openllm-0.2.3/src/openllm/bundle/oci/Dockerfile-builder` & `openllm-0.2.4/src/openllm/bundle/oci/Dockerfile-builder`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/bundle/oci/__init__.py` & `openllm-0.2.4/src/openllm/bundle/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/__init__.py` & `openllm-0.2.4/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/auto/__init__.py` & `openllm-0.2.4/src/openllm/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/auto/configuration_auto.py` & `openllm-0.2.4/src/openllm/models/auto/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/auto/factory.py` & `openllm-0.2.4/src/openllm/models/auto/factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/auto/modeling_auto.py` & `openllm-0.2.4/src/openllm/models/auto/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.2.4/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.2.4/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/auto/modeling_vllm_auto.py` & `openllm-0.2.4/src/openllm/models/auto/modeling_vllm_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/baichuan/__init__.py` & `openllm-0.2.4/src/openllm/models/baichuan/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/baichuan/configuration_baichuan.py` & `openllm-0.2.4/src/openllm/models/baichuan/configuration_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/baichuan/modeling_baichuan.py` & `openllm-0.2.4/src/openllm/models/baichuan/modeling_baichuan.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,20 +18,18 @@
 
 from .configuration_baichuan import DEFAULT_PROMPT_TEMPLATE
 from ..._prompt import default_formatter
 
 
 if t.TYPE_CHECKING:
     import torch
-    import torch.amp
 
     import transformers
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-    torch.amp = openllm.utils.LazyLoader("torch.amp", globals(), "torch.amp")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 
 
 class Baichuan(openllm.LLM["transformers.PreTrainedModel", "transformers.PreTrainedTokenizerBase"]):
     __openllm_internal__ = True
 
     def llm_post_init(self):
@@ -74,13 +72,13 @@
         return prompt_text, generate_kwargs, {}
 
     def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str:
         return generation_result[0]
 
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
         inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-        with torch.inference_mode(), torch.amp.autocast("cuda", dtype=torch.float16):
+        with torch.inference_mode(), torch.autocast("cuda", dtype=torch.float16):
             outputs = self.model.generate(
                 **inputs,
                 generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
             )
             return self.tokenizer.batch_decode(outputs, skip_special_tokens=True)
```

### Comparing `openllm-0.2.3/src/openllm/models/chatglm/__init__.py` & `openllm-0.2.4/src/openllm/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.2.4/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.2.4/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,19 +95,15 @@
             assert chat_history is not None, "'retain_history' is True while there is no history provided."
             chat_history.extend(history)
         return generated
 
     def generate(self, prompt: str, **attrs: t.Any) -> tuple[str, list[tuple[str, str]]]:
         with torch.inference_mode():
             self.model.eval()
-
             # Only use half precision if the model is not yet quantized
             if self.config.use_half_precision:
                 self.model.half()
-
-            self.model.cuda()
-
             return self.model.chat(
                 self.tokenizer,
                 prompt,
                 generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
             )
```

### Comparing `openllm-0.2.3/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.2.4/src/openllm/models/dolly_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.2.4/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.2.4/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/falcon/__init__.py` & `openllm-0.2.4/src/openllm/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.2.4/src/openllm/models/falcon/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.2.4/src/openllm/models/falcon/modeling_falcon.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,21 +19,19 @@
 
 from .configuration_falcon import DEFAULT_PROMPT_TEMPLATE
 from ..._prompt import default_formatter
 
 
 if t.TYPE_CHECKING:
     import torch
-    import torch.amp
 
     import bentoml
     import transformers
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-    torch.amp = openllm.utils.LazyLoader("torch.amp", globals(), "torch.amp")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 
 
 class Falcon(openllm.LLM["transformers.PreTrainedModel", "transformers.PreTrainedTokenizerBase"]):
     __openllm_internal__ = True
 
     @property
@@ -97,15 +95,15 @@
 
     def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str:
         return generation_result[0]
 
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
         eos_token_id = attrs.pop("eos_token_id", self.tokenizer.eos_token_id)
         inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-        with torch.inference_mode(), torch.amp.autocast("cuda", dtype=torch.float16):
+        with torch.inference_mode(), torch.autocast("cuda", dtype=torch.float16):
             outputs = self.model.generate(
                 input_ids=inputs["input_ids"],
                 attention_mask=inputs["attention_mask"],
                 generation_config=self.config.model_construct_env(
                     eos_token_id=eos_token_id, **attrs
                 ).to_generation_config(),
             )
```

### Comparing `openllm-0.2.3/src/openllm/models/flan_t5/__init__.py` & `openllm-0.2.4/src/openllm/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.2.4/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.2.4/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,16 +73,14 @@
         return prompt_text, generation_config, {}
 
     def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str:
         return generation_result[0]
 
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
         with torch.inference_mode():
-            if torch.cuda.is_available():
-                self.model.cuda()
-            input_ids = t.cast("torch.Tensor", self.tokenizer(prompt, return_tensors="pt").input_ids).to(self.device)
+            input_ids = self.tokenizer(prompt, return_tensors="pt").input_ids.to(self.device)
             result_tensor = self.model.generate(
                 input_ids,
                 do_sample=True,
                 generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
             )
             return self.tokenizer.batch_decode(result_tensor, skip_special_tokens=True)
```

### Comparing `openllm-0.2.3/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.2.4/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.2.4/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.2.4/src/openllm/models/gpt_neox/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/gpt_neox/configuration_gpt_neox.py` & `openllm-0.2.4/src/openllm/models/gpt_neox/configuration_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/gpt_neox/modeling_gpt_neox.py` & `openllm-0.2.4/src/openllm/models/gpt_neox/modeling_gpt_neox.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,22 +20,20 @@
 
 from .configuration_gpt_neox import DEFAULT_PROMPT_TEMPLATE
 from ..._prompt import default_formatter
 
 
 if t.TYPE_CHECKING:
     import torch
-    import torch.amp
 
     import bentoml
     import transformers
 else:
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-    torch.amp = openllm.utils.LazyLoader("torch.amp", globals(), "torch.amp")
 
 
 logger = logging.getLogger(__name__)
 
 
 class GPTNeoX(openllm.LLM["transformers.GPTNeoXForCausalLM", "transformers.GPTNeoXTokenizerFast"]):
     __openllm_internal__ = True
```

### Comparing `openllm-0.2.3/src/openllm/models/llama/__init__.py` & `openllm-0.2.4/src/openllm/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/llama/configuration_llama.py` & `openllm-0.2.4/src/openllm/models/llama/configuration_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/llama/modeling_llama.py` & `openllm-0.2.4/src/openllm/models/llama/modeling_llama.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,20 @@
 
 class LlaMA(openllm.LLM["transformers.LlamaForCausalLM", "transformers.LlamaTokenizerFast"]):
     __openllm_internal__ = True
 
     def llm_post_init(self):
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
+    @property
+    def import_kwargs(self):
+        model_kwds = {"device_map": "auto" if torch.cuda.device_count() > 1 else None}
+        tokenizer_kwds: dict[str, t.Any] = {}
+        return model_kwds, tokenizer_kwds
+
     def sanitize_parameters(
         self,
         prompt: str,
         top_k: int | None = None,
         top_p: float | None = None,
         temperature: float | None = None,
         max_new_tokens: int | None = None,
```

### Comparing `openllm-0.2.3/src/openllm/models/llama/modeling_vllm_llama.py` & `openllm-0.2.4/src/openllm/models/llama/modeling_vllm_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/mpt/__init__.py` & `openllm-0.2.4/src/openllm/models/mpt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/mpt/configuration_mpt.py` & `openllm-0.2.4/src/openllm/models/mpt/configuration_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/mpt/modeling_mpt.py` & `openllm-0.2.4/src/openllm/models/mpt/modeling_mpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,22 +23,20 @@
 from ..._prompt import default_formatter
 from ...utils import generate_labels
 from ...utils import is_triton_available
 
 
 if t.TYPE_CHECKING:
     import torch
-    import torch.amp
 
     import transformers
 
     from .configuration_mpt import MPTPromptType
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-    torch.amp = openllm.utils.LazyLoader("torch.amp", globals(), "torch.amp")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 
 logger = logging.getLogger(__name__)
 
 
 def get_mpt_config(
     model_id_or_path: str,
@@ -185,25 +183,22 @@
         return generation_result[0]
 
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
         llm_config = self.config.model_construct_env(**attrs)
 
         inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
 
-        if torch.cuda.is_available():
-            self.model.cuda()
-
         attrs = {
             "do_sample": False if llm_config["temperature"] == 0 else True,
             "eos_token_id": self.tokenizer.eos_token_id,
             "pad_token_id": self.tokenizer.pad_token_id,
             "generation_config": llm_config.to_generation_config(),
         }
 
         with torch.inference_mode():
             if torch.cuda.is_available():
-                with torch.amp.autocast("cuda", torch.float16):
+                with torch.autocast("cuda", torch.float16):
                     generated_tensors = self.model.generate(**inputs, **attrs)
             else:
                 generated_tensors = self.model.generate(**inputs, **attrs)
 
         return self.tokenizer.batch_decode(generated_tensors, skip_special_tokens=True)
```

### Comparing `openllm-0.2.3/src/openllm/models/opt/__init__.py` & `openllm-0.2.4/src/openllm/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/opt/configuration_opt.py` & `openllm-0.2.4/src/openllm/models/opt/configuration_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/opt/modeling_flax_opt.py` & `openllm-0.2.4/src/openllm/models/opt/modeling_flax_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/opt/modeling_opt.py` & `openllm-0.2.4/src/openllm/models/opt/modeling_opt.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,18 +130,14 @@
         if self.config.format_outputs:
             return "Generated result:\n" + "\n -".join(generation_result)
         else:
             return "\n".join(generation_result)
 
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
         with torch.inference_mode():
-            if torch.cuda.is_available() and torch.cuda.device_count() == 1:
-                self.model.cuda()
-
             inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-
             generated_tensors = self.model.generate(
                 **inputs,
                 do_sample=True,
                 generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
             )
             return self.tokenizer.batch_decode(generated_tensors, skip_special_tokens=True)
```

### Comparing `openllm-0.2.3/src/openllm/models/opt/modeling_tf_opt.py` & `openllm-0.2.4/src/openllm/models/opt/modeling_tf_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/stablelm/__init__.py` & `openllm-0.2.4/src/openllm/models/stablelm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.2.4/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.2.4/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,19 +21,17 @@
 from .configuration_stablelm import SYSTEM_PROMPT
 from ..._prompt import default_formatter
 
 
 if t.TYPE_CHECKING:
     import transformers  # noqa
     import torch
-    import torch.amp
 else:
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-    torch.amp = openllm.utils.LazyLoader("torch.amp", globals(), "torch.amp")
 
 
 logger = logging.getLogger(__name__)
 
 
 class StableLM(openllm.LLM["transformers.GPTNeoXForCausalLM", "transformers.GPTNeoXTokenizerFast"]):
     __openllm_internal__ = True
@@ -92,19 +90,16 @@
         generation_kwargs = {
             "do_sample": True,
             "generation_config": self.config.model_construct_env(**attrs).to_generation_config(),
             "pad_token_id": self.tokenizer.eos_token_id,
             "stopping_criteria": transformers.StoppingCriteriaList([StopOnTokens()]),
         }
 
-        if torch.cuda.is_available():
-            self.model.cuda()
-
-        inputs = t.cast("torch.Tensor", self.tokenizer(prompt, return_tensors="pt")).to(self.device)
+        inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
 
         with torch.inference_mode():
             if torch.cuda.is_available():
-                with torch.amp.autocast("cuda", torch.float16):
+                with torch.autocast("cuda", torch.float16):
                     tokens = self.model.generate(**inputs, **generation_kwargs)
             else:
                 tokens = self.model.generate(**inputs, **generation_kwargs)
         return [self.tokenizer.decode(tokens[0], skip_special_tokens=True)]
```

### Comparing `openllm-0.2.3/src/openllm/models/starcoder/__init__.py` & `openllm-0.2.4/src/openllm/models/starcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.2.4/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.2.4/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/playground/__init__.py` & `openllm-0.2.4/src/openllm/playground/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/playground/_meta.yml` & `openllm-0.2.4/src/openllm/playground/_meta.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/playground/falcon_tuned.py` & `openllm-0.2.4/src/openllm/playground/falcon_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/playground/features.py` & `openllm-0.2.4/src/openllm/playground/features.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/playground/llama2_qlora.py` & `openllm-0.2.4/src/openllm/playground/llama2_qlora.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/playground/opt_tuned.py` & `openllm-0.2.4/src/openllm/playground/opt_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/serialisation/__init__.py` & `openllm-0.2.4/src/openllm/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/serialisation/constants.py` & `openllm-0.2.4/src/openllm/serialisation/constants.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/serialisation/ggml.py` & `openllm-0.2.4/src/openllm/serialisation/ggml.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/serialisation/transformers.py` & `openllm-0.2.4/src/openllm/serialisation/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,16 +142,21 @@
     # NOTE: get the base args and attrs, then
     # allow override via import_model
     (model_decls, model_attrs), tokenizer_attrs = llm.llm_parameters
     decls = (*model_decls, *decls)
     attrs = {**model_attrs, **attrs}
 
     safe_serialisation = llm._serialisation_format == "safetensors"
-    metadata: DictStrAny = {"safe_serialisation": safe_serialisation}
     quantize_method = llm._quantize_method
+
+    metadata: DictStrAny = {
+        "safe_serialisation": safe_serialisation,
+        "_quantize": quantize_method if quantize_method is not None else False,
+    }
+
     signatures: DictStrAny = {}
     if quantize_method == "gptq":
         if not is_autogptq_available():
             raise OpenLLMException(
                 "GPTQ quantisation requires 'auto-gptq' (Not found in local environment). Install it with 'pip install \"openllm[gptq]\"'"
             )
         if llm.config["model_type"] != "causal_lm":
@@ -179,40 +184,38 @@
                 **hub_attrs,
                 **attrs,
             ),
         )
         metadata["_pretrained_class"] = model.__class__.__name__
         metadata["_framework"] = model.framework
 
-    if llm._quantize_method is not None:
-        metadata["_quantize"] = llm._quantize_method
-
     _tokenizer = infer_tokenizers_class_for_llm(llm).from_pretrained(
         llm.model_id,
         trust_remote_code=trust_remote_code,
         **hub_attrs,
         **tokenizer_attrs,
     )
     if _tokenizer.pad_token is None:
         _tokenizer.pad_token = _tokenizer.eos_token
 
-    external_modules = None
-    if trust_remote_code:
-        external_modules = [importlib.import_module(model.__module__), importlib.import_module(_tokenizer.__module__)]
-
     try:
         with bentoml.models.create(
             llm.tag,
             module="openllm.serialisation.transformers",
             api_version="v1",
             context=generate_context(framework_name="openllm"),
             labels=generate_labels(llm),
             signatures=signatures if signatures else make_default_signatures(model),
             options=ModelOptions(),
-            external_modules=external_modules,
+            external_modules=[
+                importlib.import_module(model.__module__),
+                importlib.import_module(_tokenizer.__module__),
+            ]
+            if trust_remote_code
+            else None,
             metadata=metadata,
         ) as bentomodel:
             _tokenizer.save_pretrained(bentomodel.path)
 
             if quantize_method == "gptq":
                 model.save_quantized(bentomodel.path, use_safetensors=safe_serialisation)
             else:
@@ -260,21 +263,19 @@
 def load_model(llm: openllm.LLM[M, t.Any], *decls: t.Any, **attrs: t.Any) -> ModelProtocol[M]:
     """Load the model from BentoML store.
 
     By default, it will try to find check the model in the local store.
     If model is not found, it will raises a ``bentoml.exceptions.NotFound``.
     """
     config, hub_attrs, attrs = process_transformers_config(llm.model_id, llm.__llm_trust_remote_code__, **attrs)
-
     # NOTE: get the base args and attrs, then
     # allow override via import_model
     (model_decls, model_attrs), _ = llm.llm_parameters
     decls = (*model_decls, *decls)
     attrs = {**model_attrs, **attrs}
-
     metadata = llm._bentomodel.info.metadata
     safe_serialization = first_not_none(
         t.cast(t.Optional[bool], metadata.get("safe_serialisation", None)),
         attrs.pop("safe_serialization", None),
         default=llm._serialisation_format == "safetensors",
     )
     if "_quantize" in metadata and metadata["_quantize"] == "gptq":
@@ -292,23 +293,35 @@
                 quantize_config=t.cast("autogptq.BaseQuantizeConfig", llm.quantization_config),
                 trust_remote_code=llm.__llm_trust_remote_code__,
                 use_safetensors=safe_serialization,
                 **hub_attrs,
                 **attrs,
             ),
         )
-
     model = infer_autoclass_from_llm_config(llm, config).from_pretrained(
         llm._bentomodel.path,
         *decls,
         config=config,
         trust_remote_code=llm.__llm_trust_remote_code__,
         **hub_attrs,
         **attrs,
     )
+    # NOTE: we only cast and load the model if it is not already quantized and setup correctly
+    loaded_in_kbit = (
+        getattr(model, "is_loaded_in_8bit", False)
+        or getattr(model, "is_loaded_in_4bit", False)
+        or getattr(model, "is_quantized", False)
+    )
+    if torch.cuda.is_available() and torch.cuda.device_count() == 1 and not loaded_in_kbit:
+        try:
+            model = model.to("cuda")
+        except torch.cuda.OutOfMemoryError as err:
+            raise RuntimeError(
+                f"Failed to fit {llm.config['model_name']} with model_id '{llm.model_id}' to CUDA.\nNote: You can try out '--quantize int8' for dynamic quantization."
+            ) from err
     if llm.bettertransformer and llm.__llm_implementation__ == "pt" and not isinstance(model, _transformers.Pipeline):
         # BetterTransformer is currently only supported on PyTorch.
         from optimum.bettertransformer import BetterTransformer
 
         model = BetterTransformer.transform(model)  # type: ignore
     return t.cast("ModelProtocol[M]", model)
```

### Comparing `openllm-0.2.3/src/openllm/utils/__init__.py` & `openllm-0.2.4/src/openllm/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,21 +95,26 @@
         return isinstance(cls, type) and issubclass(cls, class_or_tuple)  # type: ignore[arg-type]
     except TypeError:
         if isinstance(cls, _WithArgsTypes):
             return False
         raise
 
 
-def gpu_count() -> tuple[str, ...]:
+def available_devices() -> tuple[str, ...]:
     """Return available GPU under system. Currently only supports NVIDIA GPUs."""
     from .._strategies import NvidiaGpuResource
 
     return tuple(NvidiaGpuResource.from_system())
 
 
+@functools.lru_cache(maxsize=1)
+def device_count() -> int:
+    return len(available_devices())
+
+
 # equivocal setattr to save one lookup per assignment
 _object_setattr = object.__setattr__
 
 
 def non_intrusive_setattr(obj: t.Any, name: str, value: t.Any) -> None:
     """This makes sure that we don't overwrite any existing attributes on the object."""
     _setattr = functools.partial(setattr, obj) if isinstance(obj, type) else _object_setattr.__get__(obj)
```

### Comparing `openllm-0.2.3/src/openllm/utils/analytics.py` & `openllm-0.2.4/src/openllm/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/utils/codegen.py` & `openllm-0.2.4/src/openllm/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/utils/dantic.py` & `openllm-0.2.4/src/openllm/utils/dantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,17 +522,17 @@
         Most types do not provide completions, but some do, and this allows custom types to provide custom completions as well.
 
         Args:
             ctx: Invocation context for this command.
             param: The parameter that is requesting completion.
             incomplete: Value being completed. May be empty.
         """
-        from ..utils import gpu_count
+        from ..utils import available_devices
 
-        mapping = incomplete.split(self.envvar_list_splitter) if incomplete else gpu_count()
+        mapping = incomplete.split(self.envvar_list_splitter) if incomplete else available_devices()
 
         return [sc.CompletionItem(str(i), help=f"CUDA device index {i}") for i in mapping]
 
     def convert(self, value: t.Any, param: click.Parameter | None, ctx: click.Context | None) -> t.Any:
         if isinstance(value, bytes):
             enc = _get_argv_encoding()
             try:
```

### Comparing `openllm-0.2.3/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.2.4/src/openllm/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.2.4/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.2.4/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/utils/dummy_pt_and_triton_objects.py` & `openllm-0.2.4/src/openllm/utils/dummy_pt_and_triton_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.2.4/src/openllm/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.2.4/src/openllm/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/utils/dummy_vllm_objects.py` & `openllm-0.2.4/src/openllm/utils/dummy_vllm_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/utils/import_utils.py` & `openllm-0.2.4/src/openllm/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/utils/lazy.py` & `openllm-0.2.4/src/openllm/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm/utils/representation.py` & `openllm-0.2.4/src/openllm/utils/representation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm_client/__init__.py` & `openllm-0.2.4/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm_client/_prompt.py` & `openllm-0.2.4/src/openllm_client/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm_client/runtimes/__init__.py` & `openllm-0.2.4/src/openllm_client/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm_client/runtimes/base.py` & `openllm-0.2.4/src/openllm_client/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm_client/runtimes/grpc.py` & `openllm-0.2.4/src/openllm_client/runtimes/grpc.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/src/openllm_client/runtimes/http.py` & `openllm-0.2.4/src/openllm_client/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/__init__.py` & `openllm-0.2.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/client_test.py` & `openllm-0.2.4/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/configuration_test.py` & `openllm-0.2.4/tests/configuration_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/conftest.py` & `openllm-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/llm_test.py` & `openllm-0.2.4/tests/llm_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/models_test.py` & `openllm-0.2.4/tests/models_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/package_test.py` & `openllm-0.2.4/tests/package_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/strategies_test.py` & `openllm-0.2.4/tests/strategies_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/_strategies/__init__.py` & `openllm-0.2.4/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/_strategies/_configuration.py` & `openllm-0.2.4/tests/_strategies/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/models/__init__.py` & `openllm-0.2.4/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/models/conftest.py` & `openllm-0.2.4/tests/models/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,16 +253,15 @@
     args = ["serve" if not _serve_grpc else "serve-grpc"]
 
     env: DictStrAny = {}
 
     if quantize is not None:
         env[envvar.quantize] = quantize
 
-    available = openllm.utils.gpu_count()
-    gpus = len(available) if len(available) > 0 else -1
+    gpus = openllm.utils.device_count() or -1
     devs = [docker.types.DeviceRequest(count=gpus, capabilities=[["gpu"]])] if gpus > 0 else None
 
     container = client.containers.run(
         image_tag,
         command=args,
         name=container_name,
         environment=env,
```

### Comparing `openllm-0.2.3/tests/models/flan_t5_test.py` & `openllm-0.2.4/tests/models/flan_t5_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/models/opt_test.py` & `openllm-0.2.4/tests/models/opt_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json` & `openllm-0.2.4/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json` & `openllm-0.2.4/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/models/__snapshots__/opt_test/test_opt_125m[container].json` & `openllm-0.2.4/tests/models/__snapshots__/opt_test/test_opt_125m[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/tests/models/__snapshots__/opt_test/test_opt_125m[local].json` & `openllm-0.2.4/tests/models/__snapshots__/opt_test/test_opt_125m[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/.gitignore` & `openllm-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/LICENSE.md` & `openllm-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/README.md` & `openllm-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/hatch.toml` & `openllm-0.2.4/hatch.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.3/pyproject.toml` & `openllm-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     "openllm[playground]",
     "openllm[starcoder]",
     "openllm[vllm]",
 ]
 baichuan = ["cpm-kernels", "sentencepiece"]
 chatglm = ["cpm-kernels", "sentencepiece"]
 falcon = ["einops", "xformers"]
-fine-tune = ["peft", "bitsandbytes", "datasets", "accelerate", "deepspeed", "trl"]
+fine-tune = ["peft>=0.4.0", "bitsandbytes", "datasets", "accelerate", "deepspeed", "trl"]
 flan-t5 = ["flax", "jax", "jaxlib", "tensorflow", "keras"]
 ggml = ["ctransformers"]
 gptq = ["auto-gptq[triton]"]
 llama = ["fairscale", "sentencepiece"]
 mpt = ["triton", "einops"]
 openai = ["openai", "tiktoken"]
 opt = ["flax", "jax", "jaxlib", "tensorflow", "keras"]
```

### Comparing `openllm-0.2.3/PKG-INFO` & `openllm-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.2.3
+Version: 0.2.4
 Summary: OpenLLM: Operating LLMs in production
 Project-URL: Blog, https://modelserving.com
 Project-URL: Discord, https://l.bentoml.com/join-openllm-discord
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: GitHub, https://github.com/bentoml/openllm
 Project-URL: History, https://github.com/bentoml/openllm/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
@@ -81,15 +81,15 @@
 Requires-Dist: einops; extra == 'falcon'
 Requires-Dist: xformers; extra == 'falcon'
 Provides-Extra: fine-tune
 Requires-Dist: accelerate; extra == 'fine-tune'
 Requires-Dist: bitsandbytes; extra == 'fine-tune'
 Requires-Dist: datasets; extra == 'fine-tune'
 Requires-Dist: deepspeed; extra == 'fine-tune'
-Requires-Dist: peft; extra == 'fine-tune'
+Requires-Dist: peft>=0.4.0; extra == 'fine-tune'
 Requires-Dist: trl; extra == 'fine-tune'
 Provides-Extra: flan-t5
 Requires-Dist: flax; extra == 'flan-t5'
 Requires-Dist: jax; extra == 'flan-t5'
 Requires-Dist: jaxlib; extra == 'flan-t5'
 Requires-Dist: keras; extra == 'flan-t5'
 Requires-Dist: tensorflow; extra == 'flan-t5'
```

