# Comparing `tmp/openllm-0.2.4.tar.gz` & `tmp/openllm-0.2.5.tar.gz`

## Comparing `openllm-0.2.4.tar` & `openllm-0.2.5.tar`

### file list

```diff
@@ -1,137 +1,137 @@
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.4/.gitattributes
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 openllm-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.4/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0    12353 2020-02-02 00:00:00.000000 openllm-0.2.4/CHANGELOG.md
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.4/CITATION.cff
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.4/DEVELOPMENT.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.4/nightly-requirements-gpu.txt
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.4/nightly-requirements.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.4/package.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.4/pyoxidizer.bzl
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.4/taplo.toml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/__about__.py
--rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/__main__.py
--rw-r--r--   0        0        0    90069 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_configuration.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_generation.py
--rw-r--r--   0        0        0    67205 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_llm.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_prompt.py
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_quantisation.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_schema.py
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_service.py
--rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_strategies.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/_types.py
--rw-r--r--   0        0        0   100438 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/cli.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/client.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/py.typed
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/testing.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/bundle/__init__.py
--rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/bundle/_package.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/bundle/oci/Dockerfile-builder
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/bundle/oci/Dockerfile-vllm
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/bundle/oci/__init__.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/auto/modeling_vllm_auto.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/baichuan/__init__.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/baichuan/configuration_baichuan.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/baichuan/modeling_baichuan.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/gpt_neox/configuration_gpt_neox.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/gpt_neox/modeling_gpt_neox.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/llama/configuration_llama.py
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/llama/modeling_llama.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/llama/modeling_vllm_llama.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/mpt/__init__.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/mpt/configuration_mpt.py
--rw-r--r--   0        0        0     8006 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/mpt/modeling_mpt.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/opt/__init__.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/opt/configuration_opt.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/opt/modeling_flax_opt.py
--rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/opt/modeling_opt.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/opt/modeling_tf_opt.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/__init__.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/_meta.yml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/falcon_tuned.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/features.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/llama2_qlora.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/playground/opt_tuned.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/serialisation/__init__.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/serialisation/constants.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/serialisation/ggml.py
--rw-r--r--   0        0        0    17424 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/serialisation/transformers.py
--rw-r--r--   0        0        0    17096 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    20006 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_pt_and_triton_objects.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/dummy_vllm_objects.py
--rw-r--r--   0        0        0    20528 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm/utils/representation.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.4/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/client_test.py
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/configuration_test.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/conftest.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/llm_test.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models_test.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/package_test.py
--rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/strategies_test.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/__init__.py
--rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/conftest.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/flan_t5_test.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/opt_test.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.4/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.4/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.4/LICENSE.md
--rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.4/README.md
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 openllm-0.2.4/hatch.toml
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 openllm-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    30097 2020-02-02 00:00:00.000000 openllm-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.5/.gitattributes
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 openllm-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.5/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0    12745 2020-02-02 00:00:00.000000 openllm-0.2.5/CHANGELOG.md
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.5/CITATION.cff
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.5/DEVELOPMENT.md
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.5/nightly-requirements-gpu.txt
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.5/nightly-requirements.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.5/package.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.5/pyoxidizer.bzl
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.5/taplo.toml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/__about__.py
+-rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/__main__.py
+-rw-r--r--   0        0        0    90069 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_configuration.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_generation.py
+-rw-r--r--   0        0        0    67205 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_llm.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_quantisation.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_schema.py
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_service.py
+-rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_strategies.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_types.py
+-rw-r--r--   0        0        0   101935 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/cli.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/client.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/py.typed
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/testing.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/bundle/__init__.py
+-rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/bundle/_package.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/bundle/oci/Dockerfile-builder
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/bundle/oci/Dockerfile-vllm
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/bundle/oci/__init__.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/modeling_vllm_auto.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/baichuan/__init__.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/baichuan/configuration_baichuan.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/baichuan/modeling_baichuan.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/gpt_neox/configuration_gpt_neox.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/gpt_neox/modeling_gpt_neox.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/llama/configuration_llama.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/llama/modeling_llama.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/llama/modeling_vllm_llama.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/mpt/__init__.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/mpt/configuration_mpt.py
+-rw-r--r--   0        0        0     8006 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/mpt/modeling_mpt.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/opt/__init__.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/opt/configuration_opt.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/opt/modeling_flax_opt.py
+-rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/opt/modeling_opt.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/opt/modeling_tf_opt.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/__init__.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/_meta.yml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/falcon_tuned.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/features.py
+-rw-r--r--   0        0        0     8520 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/llama2_qlora.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/opt_tuned.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/serialisation/__init__.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/serialisation/constants.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/serialisation/ggml.py
+-rw-r--r--   0        0        0    17424 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/serialisation/transformers.py
+-rw-r--r--   0        0        0    17096 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    20013 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_pt_and_triton_objects.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_vllm_objects.py
+-rw-r--r--   0        0        0    20528 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/representation.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/client_test.py
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/configuration_test.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/conftest.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/llm_test.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models_test.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/package_test.py
+-rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/strategies_test.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/__init__.py
+-rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/conftest.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/flan_t5_test.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/opt_test.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.5/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.5/LICENSE.md
+-rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.5/README.md
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 openllm-0.2.5/hatch.toml
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 openllm-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    30097 2020-02-02 00:00:00.000000 openllm-0.2.5/PKG-INFO
```

### Comparing `openllm-0.2.4/.pre-commit-config.yaml` & `openllm-0.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/ADDING_NEW_MODEL.md` & `openllm-0.2.5/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/CHANGELOG.md` & `openllm-0.2.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,28 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.2.5](https://github.com/bentoml/openllm/tree/v0.2.5)
+
+### Features
+
+- Added support for sending arguments via CLI.
+
+  ```python
+  openllm query --endpoint localhost:3000 "What is the difference between noun and pronoun?" --sampling-params temperature 0.84
+  ```
+
+  Fixed llama2 qlora training script to save unquantized weights
+  [#130](https://github.com/bentoml/openllm/issues/130)
+
+
 ## [0.2.4](https://github.com/bentoml/openllm/tree/v0.2.4)
 No significant changes.
 
 
 ## [0.2.3](https://github.com/bentoml/openllm/tree/v0.2.3)
 No significant changes.
```

### Comparing `openllm-0.2.4/CITATION.cff` & `openllm-0.2.5/CITATION.cff`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/DEVELOPMENT.md` & `openllm-0.2.5/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/nightly-requirements.txt` & `openllm-0.2.5/nightly-requirements.txt`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/package.json` & `openllm-0.2.5/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.2.5'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.2.4",
+    "version": "0.2.5",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.2.4/pyoxidizer.bzl` & `openllm-0.2.5/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/__about__.py` & `openllm-0.2.5/src/openllm/bundle/oci/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,8 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.2.4"
+"""OCI-related utilities for OpenLLM.
+
+## TODO
+- generate compatible Sagemaker container
+- build custom kernels and CUDA 11.8
+- compose vLLM for PagedAttention
+"""
```

### Comparing `openllm-0.2.4/src/openllm/__init__.py` & `openllm-0.2.5/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/__main__.py` & `openllm-0.2.5/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/_configuration.py` & `openllm-0.2.5/src/openllm/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/_generation.py` & `openllm-0.2.5/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/_llm.py` & `openllm-0.2.5/src/openllm/_llm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/_prompt.py` & `openllm-0.2.5/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/_quantisation.py` & `openllm-0.2.5/src/openllm/_quantisation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/_schema.py` & `openllm-0.2.5/src/openllm/_schema.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/_service.py` & `openllm-0.2.5/src/openllm/_service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/_strategies.py` & `openllm-0.2.5/src/openllm/_strategies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/_types.py` & `openllm-0.2.5/src/openllm/_types.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/cli.py` & `openllm-0.2.5/src/openllm/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 from .utils import DEBUG
 from .utils import ENV_VARS_TRUE_VALUES
 from .utils import EnvVarMixin
 from .utils import LazyLoader
 from .utils import LazyType
 from .utils import analytics
 from .utils import available_devices
-from .utils import bentoml_cattr
 from .utils import codegen
 from .utils import configure_logging
 from .utils import dantic
 from .utils import device_count
 from .utils import first_not_none
 from .utils import get_debug_mode
 from .utils import get_quiet_mode
@@ -175,24 +174,30 @@
     call = click.echo
     if _with_style:
         attrs["fg"] = fg if not get_debug_mode() else None
         call = click.secho
     call(text, **attrs)
 
 
-output_option: t.Callable[[_AnyCallable], _AnyCallable] = click.option(
-    "-o",
-    "--output",
-    type=click.Choice(["json", "pretty", "porcelain"]),
-    default="pretty",
-    help="Showing output type.",
-    show_default=True,
-    envvar="OPENLLM_OUTPUT",
-    show_envvar=True,
-)
+def output_option(f: t.Callable[[FC], FC], *, factory: t.Any = click) -> t.Callable[[FC], FC]:
+    return factory.option(
+        "-o",
+        "--output",
+        "output",
+        type=click.Choice(["json", "pretty", "porcelain"]),
+        default="pretty",
+        help="Showing output type.",
+        show_default=True,
+        envvar="OPENLLM_OUTPUT",
+        show_envvar=True,
+    )(f)
+
+
+def machine_option(factory: t.Any) -> t.Callable[[FC], FC]:
+    return factory.option("--machine", is_flag=True, default=False, hidden=True)
 
 
 def model_id_option(factory: t.Any, model_env: EnvVarMixin | None = None) -> t.Callable[[FC], FC]:
     envvar = None
     if model_env is not None:
         envvar = model_env.model_id
     return factory.option(
@@ -1233,15 +1238,15 @@
     "--runtime",
     type=click.Choice(["ggml", "transformers"]),
     default="transformers",
     help="The runtime to use for the given model. Default is transformers.",
 )
 @output_option
 @quantize_option(click)
-@click.option("--machine", is_flag=True, default=False, hidden=True)
+@machine_option(click)
 @click.option("--implementation", type=click.Choice(["pt", "tf", "flax", "vllm"]), default=None, hidden=True)
 @serialisation_option(click)
 def download_models_command(
     model: str,
     model_id: str | None,
     converter: str | None,
     model_version: str | None,
@@ -1739,15 +1744,15 @@
 
 @cli.command(context_settings={"token_normalize_func": inflection.underscore})
 @click.argument(
     "model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()])
 )
 @model_id_option(click)
 @output_option
-@click.option("--machine", is_flag=True, default=False, hidden=True)
+@machine_option(click)
 @click.option("--overwrite", is_flag=True, help="Overwrite existing Bento for given LLM if it already exists.")
 @workers_per_resource_option(click, build=True)
 @cog.optgroup.group(cls=cog.MutuallyExclusiveOptionGroup, name="Optimisation options")
 @quantize_option(cog.optgroup, build=True)
 @bettertransformer_option(cog.optgroup)
 @click.option(
     "--runtime",
@@ -2013,15 +2018,15 @@
 @output_option
 @click.option(
     "--show-available",
     is_flag=True,
     default=False,
     help="Show available models in local store (mutually exclusive with '-o porcelain').",
 )
-@click.option("--machine", is_flag=True, default=False, hidden=True)
+@machine_option(click)
 @click.pass_context
 def models_command(
     ctx: click.Context, output: OutputLiteral, show_available: bool, machine: bool
 ) -> DictStrAny | None:
     """List all supported models.
 
     \b
@@ -2077,32 +2082,35 @@
             if DEBUG:
                 try:
                     openllm.AutoLLM.for_model(m, llm_config=config)
                 except Exception as e:
                     failed_initialized.append((m, e))
 
         ids_in_local_store: DictStrAny | None = None
+        local_models: DictStrAny | None = None
         if show_available:
             ids_in_local_store = {
                 k: [
                     i
                     for i in bentoml.models.list()
                     if "framework" in i.info.labels
                     and i.info.labels["framework"] == "openllm"
                     and "model_name" in i.info.labels
                     and i.info.labels["model_name"] == k
                 ]
                 for k in json_data.keys()
             }
             ids_in_local_store = {k: v for k, v in ids_in_local_store.items() if v}
+            local_models = {k: [str(i.tag) for i in val] for k, val in ids_in_local_store.items()}
 
         if machine:
             if show_available:
                 assert ids_in_local_store
-                json_data["local"] = [bentoml_cattr.unstructure(i.tag) for m in ids_in_local_store.values() for i in m]
+                assert local_models
+                json_data["local"] = local_models
             return json_data
         elif output == "pretty":
             import tabulate
 
             tabulate.PRESERVE_WHITESPACE = True
 
             # llm, architecture, url, model_id, installation, cpu, gpu, runtime_impl
@@ -2170,30 +2178,32 @@
                 _echo("\nThe following models are supported but failed to initialize:\n")
                 for m, err in failed_initialized:
                     _echo(f"- {m}: ", fg="blue", nl=False)
                     _echo(err, fg="red")
 
             if show_available:
                 assert ids_in_local_store is not None
+                assert local_models
                 if len(ids_in_local_store) == 0:
                     _echo("No models available locally.")
                     ctx.exit(0)
 
                 _echo("The following are available in local store:", fg="magenta")
                 _echo(
                     orjson.dumps(
-                        {k: [str(i.tag) for i in val] for k, val in ids_in_local_store.items()},
+                        local_models,
                         option=orjson.OPT_INDENT_2,
                     ).decode(),
                     fg="white",
                 )
         else:
             if show_available:
                 assert ids_in_local_store
-                json_data["local"] = [bentoml_cattr.unstructure(i.tag) for m in ids_in_local_store.values() for i in m]
+                assert local_models
+                json_data["local"] = local_models
             _echo(
                 orjson.dumps(
                     json_data,
                     option=orjson.OPT_INDENT_2,
                 ).decode(),
                 fg="white",
             )
@@ -2261,15 +2271,15 @@
         return key, True
     elif len(values) == 1:
         return key, values[0]
     else:
         raise click.BadParameter(f"Invalid option format: {value}")
 
 
-def shared_client_options(f: FC) -> FC:
+def shared_client_options(f: t.Callable[[FC], FC]) -> t.Callable[[FC], FC]:
     options = [
         click.option(
             "--endpoint",
             type=click.STRING,
             help="OpenLLM Server endpoint, i.e: http://localhost:3000",
             envvar="OPENLLM_ENDPOINT",
             default="http://localhost:3000",
@@ -2354,46 +2364,57 @@
 
 @cli.command()
 @shared_client_options
 @click.option(
     "--server-type", type=click.Choice(["grpc", "http"]), help="Server type", default="http", show_default=True
 )
 @click.argument("prompt", type=click.STRING)
+@click.option(
+    "--sampling-params",
+    help="Define query options. (format: ``--opt temperature=0.8 --opt=top_k:12)",
+    required=False,
+    multiple=True,
+    callback=opt_callback,
+    metavar="ARG=VALUE[,ARG=VALUE]",
+)
 @click.pass_context
 def query(
     ctx: click.Context,
     prompt: str,
     endpoint: str,
     timeout: int,
     server_type: t.Literal["http", "grpc"],
     output: OutputLiteral,
+    _memoized: DictStrAny,
+    **attrs: t.Any,
 ) -> None:
     """Ask a LLM interactively, from a terminal.
 
     \b
     ```bash
     $ openllm query --endpoint http://12.323.2.1:3000 "What is the meaning of life?"
     ```
     """
+    _memoized = {k: orjson.loads(v[0]) for k, v in _memoized.items() if v}
     if server_type == "grpc":
         endpoint = re.sub(r"http://", "", endpoint)
     client = (
         openllm.client.HTTPClient(endpoint, timeout=timeout)
         if server_type == "http"
         else openllm.client.GrpcClient(endpoint, timeout=timeout)
     )
 
     input_fg = "magenta"
     generated_fg = "cyan"
 
     if output != "porcelain":
-        _echo("Input prompt: ", nl=False, fg="white")
-        _echo(f"{prompt}", fg=input_fg, nl=False)
+        _echo("==Input==\n", fg="white")
+        _echo(f"{prompt}", fg=input_fg)
 
-    res = client.query(prompt, return_raw_response=True)
+    res = client.query(prompt, return_raw_response=True, **_memoized)
 
     if output == "pretty":
         full_formatted = client.llm.postprocess_generate(prompt, res["responses"])
         response = full_formatted[len(prompt) + 1 :]
         _echo("\n\n==Responses==\n", fg="white")
         _echo(f"{prompt} ", fg=input_fg, nl=False)
         _echo(response, fg=generated_fg)
@@ -2420,54 +2441,80 @@
         for k in tuple(inflection.dasherize(key) for key in openllm.CONFIG_MAPPING.keys())
     }
     mapping = {k: v for k, v in mapping.items() if v}
     _echo(orjson.dumps(mapping, option=orjson.OPT_INDENT_2).decode(), fg="white")
     ctx.exit(0)
 
 
+@overload
+def get_prompt(
+    model_name: str, prompt: str, format: str | None, output: OutputLiteral, machine: t.Literal[True] = True
+) -> str:
+    ...
+
+
+@overload
+def get_prompt(
+    model_name: str, prompt: str, format: str | None, output: OutputLiteral, machine: t.Literal[False] = ...
+) -> None:
+    ...
+
+
 @utils_command.command()
 @click.argument(
     "model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()])
 )
 @click.argument("prompt", type=click.STRING)
 @output_option
 @click.option("--format", type=click.STRING, default=None)
-def get_prompt(model_name: str, prompt: str, format: str | None, output: OutputLiteral) -> None:
+@machine_option(click)
+def get_prompt(model_name: str, prompt: str, format: str | None, output: OutputLiteral, machine: bool) -> str | None:
     """Get the default prompt used by OpenLLM."""
+    module = openllm.utils.EnvVarMixin(model_name).module
     try:
-        module = openllm.utils.EnvVarMixin(model_name).module
-        template = module.DEFAULT_PROMPT_TEMPLATE
+        template = getattr(module, "DEFAULT_PROMPT_TEMPLATE", None)
+        prompt_mapping = getattr(module, "PROMPT_MAPPING", None)
+        if template is None:
+            raise click.BadArgumentUsage(f"model {model_name} does not have a default prompt template") from None
         if callable(template):
             if format is None:
                 if not hasattr(module, "PROMPT_MAPPING") or module.PROMPT_MAPPING is None:
                     raise RuntimeError("Failed to find prompt mapping while DEFAULT_PROMPT_TEMPLATE is a function.")
                 raise click.BadOptionUsage(
                     "format",
                     f"{model_name} prompt requires passing '--format' (available format: {list(module.PROMPT_MAPPING)})",
                 )
-            if format not in module.PROMPT_MAPPING:
+            if prompt_mapping is None:
+                raise click.BadArgumentUsage(
+                    f"Failed to fine prompt mapping while the default prompt for {model_name} is a callable."
+                ) from None
+            if format not in prompt_mapping:
                 raise click.BadOptionUsage(
                     "format",
-                    f"Given format {format} is not valid for {model_name} (available format: {list(module.PROMPT_MAPPING)})",
+                    f"Given format {format} is not valid for {model_name} (available format: {list(prompt_mapping)})",
                 )
             _prompt = template(format)
         else:
             _prompt = template
 
+        # XXX: FIX ME, currently doesn't work with all different context variable
+        # will need a --opt parser for this
         fully_formatted = _prompt.format(instruction=prompt)
 
-        if output == "porcelain":
+        if machine:
+            return repr(fully_formatted)
+        elif output == "porcelain":
             _echo(repr(fully_formatted), fg="white")
         elif output == "json":
             _echo(orjson.dumps({"prompt": fully_formatted}, option=orjson.OPT_INDENT_2).decode(), fg="white")
         else:
             _echo(f"== Prompt for {model_name} ==\n", fg="magenta")
             _echo(fully_formatted, fg="white")
     except AttributeError:
-        raise click.ClickException(f"{model_name} does not have default prompt template.") from None
+        raise click.ClickException(f"Failed to determine a default prompt template for {model_name}.") from None
 
 
 def load_notebook_metadata() -> DictStrAny:
     with open(os.path.join(os.path.dirname(openllm.playground.__file__), "_meta.yml"), "r") as f:
         content = yaml.safe_load(f)
     if not all("description" in k for k in content.values()):
         raise ValueError("Invalid metadata file. All entries must have a 'description' key.")
```

### Comparing `openllm-0.2.4/src/openllm/client.py` & `openllm-0.2.5/src/openllm/client.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/exceptions.py` & `openllm-0.2.5/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/testing.py` & `openllm-0.2.5/src/openllm/testing.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/bundle/__init__.py` & `openllm-0.2.5/src/openllm/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/bundle/_package.py` & `openllm-0.2.5/src/openllm/bundle/_package.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/bundle/oci/Dockerfile-builder` & `openllm-0.2.5/src/openllm/bundle/oci/Dockerfile-builder`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/bundle/oci/__init__.py` & `openllm-0.2.5/src/openllm/utils/dummy_pt_and_triton_objects.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""OCI-related utilities for OpenLLM.
 
-## TODO
-- generate compatible Sagemaker container
-- build custom kernels and CUDA 11.8
-- compose vLLM for PagedAttention
-"""
+from __future__ import annotations
+import typing as t
+
+from ..utils import DummyMetaclass
+from ..utils import require_backends
+
+
+class MPT(metaclass=DummyMetaclass):
+    _backends = ["torch", "triton"]
+
+    def __init__(self, *args: t.Any, **attrs: t.Any):
+        require_backends(self, ["torch"])
```

### Comparing `openllm-0.2.4/src/openllm/models/__init__.py` & `openllm-0.2.5/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/auto/__init__.py` & `openllm-0.2.5/src/openllm/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/auto/configuration_auto.py` & `openllm-0.2.5/src/openllm/models/auto/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/auto/factory.py` & `openllm-0.2.5/src/openllm/models/auto/factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/auto/modeling_auto.py` & `openllm-0.2.5/src/openllm/models/auto/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.2.5/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.2.5/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/auto/modeling_vllm_auto.py` & `openllm-0.2.5/src/openllm/models/auto/modeling_vllm_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/baichuan/__init__.py` & `openllm-0.2.5/src/openllm/models/baichuan/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/baichuan/configuration_baichuan.py` & `openllm-0.2.5/src/openllm/models/baichuan/configuration_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/baichuan/modeling_baichuan.py` & `openllm-0.2.5/src/openllm/models/baichuan/modeling_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/chatglm/__init__.py` & `openllm-0.2.5/src/openllm/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.2.5/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.2.5/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.2.5/src/openllm/models/dolly_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.2.5/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.2.5/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/falcon/__init__.py` & `openllm-0.2.5/src/openllm/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.2.5/src/openllm/models/falcon/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.2.5/src/openllm/models/falcon/modeling_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/flan_t5/__init__.py` & `openllm-0.2.5/src/openllm/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.2.5/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.2.5/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.2.5/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.2.5/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.2.5/src/openllm/models/gpt_neox/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/gpt_neox/configuration_gpt_neox.py` & `openllm-0.2.5/src/openllm/models/gpt_neox/configuration_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/gpt_neox/modeling_gpt_neox.py` & `openllm-0.2.5/src/openllm/models/gpt_neox/modeling_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/llama/__init__.py` & `openllm-0.2.5/src/openllm/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/llama/configuration_llama.py` & `openllm-0.2.5/src/openllm/models/llama/configuration_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/llama/modeling_llama.py` & `openllm-0.2.5/src/openllm/models/llama/modeling_llama.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,20 +39,14 @@
 
 class LlaMA(openllm.LLM["transformers.LlamaForCausalLM", "transformers.LlamaTokenizerFast"]):
     __openllm_internal__ = True
 
     def llm_post_init(self):
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
-    @property
-    def import_kwargs(self):
-        model_kwds = {"device_map": "auto" if torch.cuda.device_count() > 1 else None}
-        tokenizer_kwds: dict[str, t.Any] = {}
-        return model_kwds, tokenizer_kwds
-
     def sanitize_parameters(
         self,
         prompt: str,
         top_k: int | None = None,
         top_p: float | None = None,
         temperature: float | None = None,
         max_new_tokens: int | None = None,
```

### Comparing `openllm-0.2.4/src/openllm/models/llama/modeling_vllm_llama.py` & `openllm-0.2.5/src/openllm/models/llama/modeling_vllm_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/mpt/__init__.py` & `openllm-0.2.5/src/openllm/models/mpt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/mpt/configuration_mpt.py` & `openllm-0.2.5/src/openllm/models/mpt/configuration_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/mpt/modeling_mpt.py` & `openllm-0.2.5/src/openllm/models/mpt/modeling_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/opt/__init__.py` & `openllm-0.2.5/src/openllm/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/opt/configuration_opt.py` & `openllm-0.2.5/src/openllm/models/opt/configuration_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/opt/modeling_flax_opt.py` & `openllm-0.2.5/src/openllm/models/opt/modeling_flax_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/opt/modeling_opt.py` & `openllm-0.2.5/src/openllm/models/opt/modeling_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/opt/modeling_tf_opt.py` & `openllm-0.2.5/src/openllm/models/opt/modeling_tf_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/stablelm/__init__.py` & `openllm-0.2.5/src/openllm/models/stablelm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.2.5/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.2.5/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/starcoder/__init__.py` & `openllm-0.2.5/src/openllm/models/starcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.2.5/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.2.5/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/playground/__init__.py` & `openllm-0.2.5/src/openllm/playground/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/playground/_meta.yml` & `openllm-0.2.5/src/openllm/playground/_meta.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/playground/falcon_tuned.py` & `openllm-0.2.5/src/openllm/playground/falcon_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/playground/features.py` & `openllm-0.2.5/src/openllm/playground/features.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/playground/llama2_qlora.py` & `openllm-0.2.5/src/openllm/playground/llama2_qlora.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,18 +44,14 @@
 
 
 # Change this to the local converted path if you don't have access to the meta-llama model
 DEFAULT_MODEL_ID = "meta-llama/Llama-2-7b-hf"
 DATASET_NAME = "databricks/databricks-dolly-15k"
 
 
-# import the model first hand
-openllm.import_model("llama", model_id=DEFAULT_MODEL_ID)
-
-
 def format_dolly(sample):
     instruction = f"### Instruction\n{sample['instruction']}"
     context = f"### Context\n{sample['context']}" if len(sample["context"]) > 0 else None
     response = f"### Answer\n{sample['response']}"
     # join all the parts together
     prompt = "\n\n".join([i for i in [instruction, context, response] if i is not None])
     return prompt
@@ -185,14 +181,18 @@
     model_args, training_args = parser.parse_json_file(json_file=os.path.abspath(sys.argv[1]))
 else:
     model_args, training_args = t.cast(
         t.Tuple[ModelArguments, TrainingArguments], parser.parse_args_into_dataclasses()
     )
 
 
+# import the model first hand
+openllm.import_model("llama", model_id=model_args.model_id)
+
+
 def train_loop(model_args: ModelArguments, training_args: TrainingArguments):
     import peft
 
     transformers.set_seed(model_args.seed)
 
     model, tokenizer = prepare_for_int4_training(
         model_args.model_id,
```

### Comparing `openllm-0.2.4/src/openllm/playground/opt_tuned.py` & `openllm-0.2.5/src/openllm/playground/opt_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/serialisation/__init__.py` & `openllm-0.2.5/src/openllm/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/serialisation/constants.py` & `openllm-0.2.5/src/openllm/serialisation/constants.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/serialisation/ggml.py` & `openllm-0.2.5/src/openllm/serialisation/ggml.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/serialisation/transformers.py` & `openllm-0.2.5/src/openllm/serialisation/transformers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/utils/__init__.py` & `openllm-0.2.5/src/openllm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/utils/analytics.py` & `openllm-0.2.5/src/openllm/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/utils/codegen.py` & `openllm-0.2.5/src/openllm/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/utils/dantic.py` & `openllm-0.2.5/src/openllm/utils/dantic.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
         if not all(isinstance(v, item_type) for v in values):
             raise ValueError(f"Field {value} contains items of different types.")
         self.internal_type = item_type
         self.mapping = {str(v): v for v in values}
         super(EnumChoice, self).__init__(list(self.mapping.keys()), case_sensitive)
 
 
-def allows_multiple(field_type: type) -> bool:
+def allows_multiple(field_type: type[t.Any]) -> bool:
     """Checks whether the current type allows for multiple arguments to be provided as input or not.
 
     For containers, it exploits click's support for lists and such to use the same option multiple times
     to create a complex object: `python run.py --subsets train --subsets test`
     # becomes `subsets: ["train", "test"]`.
 
     Args:
```

### Comparing `openllm-0.2.4/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.2.5/src/openllm/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.2.5/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.2.5/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/utils/dummy_pt_and_triton_objects.py` & `openllm-0.2.5/src/openllm/utils/dummy_vllm_objects.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,12 +15,22 @@
 from __future__ import annotations
 import typing as t
 
 from ..utils import DummyMetaclass
 from ..utils import require_backends
 
 
-class MPT(metaclass=DummyMetaclass):
-    _backends = ["torch", "triton"]
+class VLLMLlaMA(metaclass=DummyMetaclass):
+    _backends = ["vllm"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
-        require_backends(self, ["torch"])
+        require_backends(self, ["vllm"])
+
+
+class AutoVLLM(metaclass=DummyMetaclass):
+    _backends = ["vllm"]
+
+    def __init__(self, *args: t.Any, **attrs: t.Any):
+        require_backends(self, ["vllm"])
+
+
+MODEL_VLLM_MAPPING = None
```

### Comparing `openllm-0.2.4/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.2.5/src/openllm/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.2.5/src/openllm/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/utils/import_utils.py` & `openllm-0.2.5/src/openllm/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/utils/lazy.py` & `openllm-0.2.5/src/openllm/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm/utils/representation.py` & `openllm-0.2.5/src/openllm/utils/representation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm_client/__init__.py` & `openllm-0.2.5/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm_client/_prompt.py` & `openllm-0.2.5/src/openllm_client/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm_client/runtimes/__init__.py` & `openllm-0.2.5/src/openllm_client/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm_client/runtimes/base.py` & `openllm-0.2.5/src/openllm_client/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm_client/runtimes/grpc.py` & `openllm-0.2.5/src/openllm_client/runtimes/grpc.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/src/openllm_client/runtimes/http.py` & `openllm-0.2.5/src/openllm_client/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/__init__.py` & `openllm-0.2.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/client_test.py` & `openllm-0.2.5/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/configuration_test.py` & `openllm-0.2.5/tests/configuration_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/conftest.py` & `openllm-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/llm_test.py` & `openllm-0.2.5/tests/llm_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/models_test.py` & `openllm-0.2.5/tests/models_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/package_test.py` & `openllm-0.2.5/tests/package_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/strategies_test.py` & `openllm-0.2.5/tests/strategies_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/_strategies/__init__.py` & `openllm-0.2.5/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/_strategies/_configuration.py` & `openllm-0.2.5/tests/_strategies/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/models/__init__.py` & `openllm-0.2.5/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/models/conftest.py` & `openllm-0.2.5/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/models/flan_t5_test.py` & `openllm-0.2.5/tests/models/flan_t5_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/models/opt_test.py` & `openllm-0.2.5/tests/models/opt_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json` & `openllm-0.2.5/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json` & `openllm-0.2.5/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/models/__snapshots__/opt_test/test_opt_125m[container].json` & `openllm-0.2.5/tests/models/__snapshots__/opt_test/test_opt_125m[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/tests/models/__snapshots__/opt_test/test_opt_125m[local].json` & `openllm-0.2.5/tests/models/__snapshots__/opt_test/test_opt_125m[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/.gitignore` & `openllm-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/LICENSE.md` & `openllm-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/README.md` & `openllm-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/hatch.toml` & `openllm-0.2.5/hatch.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/pyproject.toml` & `openllm-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.4/PKG-INFO` & `openllm-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.2.4
+Version: 0.2.5
 Summary: OpenLLM: Operating LLMs in production
 Project-URL: Blog, https://modelserving.com
 Project-URL: Discord, https://l.bentoml.com/join-openllm-discord
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: GitHub, https://github.com/bentoml/openllm
 Project-URL: History, https://github.com/bentoml/openllm/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
```

