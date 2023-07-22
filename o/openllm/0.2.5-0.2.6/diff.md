# Comparing `tmp/openllm-0.2.5.tar.gz` & `tmp/openllm-0.2.6.tar.gz`

## Comparing `openllm-0.2.5.tar` & `openllm-0.2.6.tar`

### file list

```diff
@@ -1,137 +1,137 @@
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.5/.gitattributes
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 openllm-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.5/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0    12745 2020-02-02 00:00:00.000000 openllm-0.2.5/CHANGELOG.md
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.5/CITATION.cff
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.5/DEVELOPMENT.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.5/nightly-requirements-gpu.txt
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.5/nightly-requirements.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.5/package.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.5/pyoxidizer.bzl
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.5/taplo.toml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/__about__.py
--rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/__main__.py
--rw-r--r--   0        0        0    90069 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_configuration.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_generation.py
--rw-r--r--   0        0        0    67205 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_llm.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_prompt.py
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_quantisation.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_schema.py
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_service.py
--rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_strategies.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/_types.py
--rw-r--r--   0        0        0   101935 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/cli.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/client.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/py.typed
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/testing.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/bundle/__init__.py
--rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/bundle/_package.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/bundle/oci/Dockerfile-builder
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/bundle/oci/Dockerfile-vllm
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/bundle/oci/__init__.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/auto/modeling_vllm_auto.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/baichuan/__init__.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/baichuan/configuration_baichuan.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/baichuan/modeling_baichuan.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/gpt_neox/configuration_gpt_neox.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/gpt_neox/modeling_gpt_neox.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/llama/configuration_llama.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/llama/modeling_llama.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/llama/modeling_vllm_llama.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/mpt/__init__.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/mpt/configuration_mpt.py
--rw-r--r--   0        0        0     8006 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/mpt/modeling_mpt.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/opt/__init__.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/opt/configuration_opt.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/opt/modeling_flax_opt.py
--rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/opt/modeling_opt.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/opt/modeling_tf_opt.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/__init__.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/_meta.yml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/falcon_tuned.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/features.py
--rw-r--r--   0        0        0     8520 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/llama2_qlora.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/playground/opt_tuned.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/serialisation/__init__.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/serialisation/constants.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/serialisation/ggml.py
--rw-r--r--   0        0        0    17424 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/serialisation/transformers.py
--rw-r--r--   0        0        0    17096 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    20013 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_pt_and_triton_objects.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/dummy_vllm_objects.py
--rw-r--r--   0        0        0    20528 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm/utils/representation.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.5/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/client_test.py
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/configuration_test.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/llm_test.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models_test.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/package_test.py
--rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/strategies_test.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/__init__.py
--rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/conftest.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/flan_t5_test.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/opt_test.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.5/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.5/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.5/LICENSE.md
--rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.5/README.md
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 openllm-0.2.5/hatch.toml
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 openllm-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    30097 2020-02-02 00:00:00.000000 openllm-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.6/.gitattributes
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 openllm-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.6/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0    13197 2020-02-02 00:00:00.000000 openllm-0.2.6/CHANGELOG.md
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.6/CITATION.cff
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.6/DEVELOPMENT.md
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.6/nightly-requirements-gpu.txt
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.6/nightly-requirements.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.6/package.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.6/pyoxidizer.bzl
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.6/taplo.toml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/__about__.py
+-rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/__main__.py
+-rw-r--r--   0        0        0    90013 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/_configuration.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/_generation.py
+-rw-r--r--   0        0        0    70703 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/_llm.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/_quantisation.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/_schema.py
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/_service.py
+-rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/_strategies.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/_types.py
+-rw-r--r--   0        0        0   101935 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/cli.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/client.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/py.typed
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/testing.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/bundle/__init__.py
+-rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/bundle/_package.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/bundle/oci/Dockerfile-builder
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/bundle/oci/Dockerfile-vllm
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/bundle/oci/__init__.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/auto/modeling_vllm_auto.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/baichuan/__init__.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/baichuan/configuration_baichuan.py
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/baichuan/modeling_baichuan.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0    12726 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/gpt_neox/configuration_gpt_neox.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/gpt_neox/modeling_gpt_neox.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/llama/configuration_llama.py
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/llama/modeling_llama.py
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/llama/modeling_vllm_llama.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/mpt/__init__.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/mpt/configuration_mpt.py
+-rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/mpt/modeling_mpt.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/opt/__init__.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/opt/configuration_opt.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/opt/modeling_flax_opt.py
+-rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/opt/modeling_opt.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/opt/modeling_tf_opt.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/playground/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/playground/__init__.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/playground/_meta.yml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/playground/falcon_tuned.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/playground/features.py
+-rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/playground/llama2_qlora.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/playground/opt_tuned.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/serialisation/__init__.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/serialisation/constants.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/serialisation/ggml.py
+-rw-r--r--   0        0        0    15544 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/serialisation/transformers.py
+-rw-r--r--   0        0        0    17096 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    20013 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/dummy_pt_and_triton_objects.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/dummy_vllm_objects.py
+-rw-r--r--   0        0        0    20528 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm/utils/representation.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.6/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/client_test.py
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/configuration_test.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/conftest.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/llm_test.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/models_test.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/package_test.py
+-rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/strategies_test.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/models/__init__.py
+-rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/models/conftest.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/models/flan_t5_test.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/models/opt_test.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.6/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.6/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.6/LICENSE.md
+-rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.6/README.md
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 openllm-0.2.6/hatch.toml
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 openllm-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    30097 2020-02-02 00:00:00.000000 openllm-0.2.6/PKG-INFO
```

### Comparing `openllm-0.2.5/.pre-commit-config.yaml` & `openllm-0.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/ADDING_NEW_MODEL.md` & `openllm-0.2.6/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/CHANGELOG.md` & `openllm-0.2.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,25 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.2.6](https://github.com/bentoml/openllm/tree/v0.2.6)
+
+### Backwards-incompatible Changes
+
+- Updated signature for `load_model` and `load_tokenizer` not to allow tag.
+  Tag can be accessed via `llm.tag`, or if using `openllm.serialisation` or `bentoml.transformers` then you can use `self._bentomodel`
+
+  Updated serialisation shared logics to reduce callstack for saving three calltrace.
+  [#132](https://github.com/bentoml/openllm/issues/132)
+
+
 ## [0.2.5](https://github.com/bentoml/openllm/tree/v0.2.5)
 
 ### Features
 
 - Added support for sending arguments via CLI.
 
   ```python
```

### Comparing `openllm-0.2.5/CITATION.cff` & `openllm-0.2.6/CITATION.cff`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/DEVELOPMENT.md` & `openllm-0.2.6/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/nightly-requirements.txt` & `openllm-0.2.6/nightly-requirements.txt`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/package.json` & `openllm-0.2.6/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.2.6'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.2.5",
+    "version": "0.2.6",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.2.5/pyoxidizer.bzl` & `openllm-0.2.6/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/__about__.py` & `openllm-0.2.6/src/openllm/playground/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.2.5"
```

### Comparing `openllm-0.2.5/src/openllm/__init__.py` & `openllm-0.2.6/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/__main__.py` & `openllm-0.2.6/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/_configuration.py` & `openllm-0.2.6/src/openllm/_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1009,15 +1009,15 @@
     globs: DictStrAny = {
         "cls": cls,
         "_cached_attribute": attributes,
         "_cached_getattribute_get": _object_getattribute.__get__,
     }
     annotations: DictStrAny = {"return": None}
 
-    lines: ListStr = ["_getattr = _cached_getattribute_get(_cached_attribute)"]
+    lines: ListStr = []
     for attr_name, field in attr.fields_dict(attributes.__class__).items():
         arg_name = field.metadata.get("target", f"__{_prefix}_{inflection.underscore(attr_name)}__")
         args.append(f"{attr_name}=getattr(_cached_attribute, '{attr_name}')")
         lines.append(_setattr_class(arg_name, attr_name))
         annotations[attr_name] = field.type
 
     return codegen.generate_function(
```

### Comparing `openllm-0.2.5/src/openllm/_generation.py` & `openllm-0.2.6/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/_llm.py` & `openllm-0.2.6/src/openllm/_llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,20 +34,23 @@
 import bentoml
 import openllm
 from bentoml._internal.models import ModelStore
 from bentoml._internal.models.model import ModelSignature
 
 from ._configuration import AdapterType
 from ._configuration import FineTuneConfig
+from ._configuration import _object_getattribute
+from ._configuration import _setattr_class
 from ._quantisation import infer_quantisation_config
 from .exceptions import ForbiddenAttributeError
 from .exceptions import GpuNotAvailableError
 from .utils import DEBUG
 from .utils import ENV_VARS_TRUE_VALUES
 from .utils import MYPY
+from .utils import SHOW_CODEGEN
 from .utils import EnvVarMixin
 from .utils import LazyLoader
 from .utils import ReprMixin
 from .utils import bentoml_cattr
 from .utils import codegen
 from .utils import first_not_none
 from .utils import in_docker
@@ -73,20 +76,20 @@
 if t.TYPE_CHECKING:
     import auto_gptq as autogptq
     import peft
     import torch
     import vllm
 
     import transformers
-    from bentoml._internal.runner.strategy import Strategy
 
     from ._configuration import PeftType
     from ._types import AdaptersMapping
     from ._types import AdaptersTuple
     from ._types import DictStrAny
+    from ._types import ListStr
     from ._types import LiteralRuntime
     from ._types import LLMEmbeddings
     from ._types import LLMRunnable
     from ._types import LLMRunner
     from ._types import ModelSignatureDict as _ModelSignatureDict
     from ._types import PeftAdapterOutput
     from ._types import TupleAny
@@ -240,15 +243,15 @@
     return resolved
 
 
 _reserved_namespace = {"config_class", "model", "tokenizer", "import_kwargs"}
 
 M = t.TypeVar(
     "M",
-    bound="t.Union[transformers.PreTrainedModel, transformers.Pipeline, transformers.TFPreTrainedModel, transformers.FlaxPreTrainedModel, vllm.LLM]",
+    bound="t.Union[transformers.PreTrainedModel, transformers.Pipeline, transformers.TFPreTrainedModel, transformers.FlaxPreTrainedModel, vllm.LLM, peft.PeftModel, autogptq.modeling.BaseGPTQForCausalLM]",
 )
 T = t.TypeVar(
     "T",
     bound="t.Union[transformers.PreTrainedTokenizerFast, transformers.PreTrainedTokenizer, transformers.PreTrainedTokenizerBase]",
 )
 
 
@@ -344,18 +347,18 @@
         _, tokenizer_attrs = llm.llm_parameters
         ```
 
         By default, `model_decls` and `model_attrs` is already sanitised and concatenated into `args` and `attrs`
         """
         raise NotImplementedError
 
-    def load_model(self, tag: bentoml.Tag, *args: t.Any, **attrs: t.Any) -> M:
+    def load_model(self, *args: t.Any, **attrs: t.Any) -> M:
         """This function can be implemented to override the default load_model behaviour.
 
-        See falcon for example implementation.
+        See falcon for example implementation. Tag can be accessed via ``self.tag``
         """
         raise NotImplementedError
 
     def load_tokenizer(self, tag: bentoml.Tag, **attrs: t.Any) -> T:
         """This function can be implemented to override how to load the tokenizer.
 
         See falcon for example implementation.
@@ -390,31 +393,26 @@
     """This is used to determine which implementation that this LLM has.
 
     Usually, this will inferred from class name, that follows the HuggingFace's naming convention:
 
     - `OPTForConditionalGeneration` -> `pt`
     - `TFOPTForConditionalGeneration` -> `tf`
     - `FlaxOPTForConditionalGeneration` -> `flax`
+
+    An additional naming for all VLLM backend: VLLMLlaMA -> `vllm`
     """
-    __llm_model__: M | peft.PeftModel | None
+    __llm_model__: M | None
     """A reference to the actual model. Instead of access this directly, you should use `model` property instead."""
     __llm_tokenizer__: T | None
     """A reference to the actual tokenizer. Instead of access this directly, you should use `tokenizer` property instead."""
     __llm_bentomodel__: bentoml.Model | None
     """A reference to the bentomodel used for this LLM. Instead of access this directly, you should use `_bentomodel` property instead."""
     __llm_adapter_map__: dict[AdapterType, dict[str | t.Literal["default"], tuple[peft.PeftConfig, str]]] | None
     """A reference to the the cached LoRA adapter mapping."""
 
-    __llm_custom_import__: bool
-    """Whether this LLM has a custom import_model"""
-    __llm_custom_load__: bool
-    """A boolean to determine whether a custom 'load_model' is implemented"""
-    __llm_custom_tokenizer__: bool
-    """A boolean to determine whether a custom 'load_tokenizer' is implemented"""
-
     if t.TYPE_CHECKING and not MYPY:
 
         def __attrs_init__(
             self,
             config: openllm.LLMConfig,
             quantization_config: transformers.BitsAndBytesConfig | autogptq.BaseQuantizeConfig | None,
             model_id: str,
@@ -428,14 +426,129 @@
             quantize_method: t.Literal["int8", "int4", "gptq"] | None,
             serialisation_format: t.Literal["safetensors", "legacy"],
             **attrs: t.Any,
         ) -> None:
             """Generated __attrs_init__ for openllm.LLM."""
 
 
+if t.TYPE_CHECKING:
+    _R = t.TypeVar("_R")
+
+    class _import_model_wrapper(t.Generic[_R, M, T]):
+        def __call__(self, llm: LLM[M, T], *decls: t.Any, trust_remote_code: bool, **attrs: t.Any) -> _R:
+            ...
+
+    class _load_model_wrapper(t.Generic[M, T]):
+        def __call__(self, llm: LLM[M, T], *decls: t.Any, **attrs: t.Any) -> M:
+            ...
+
+    class _load_tokenizer_wrapper(t.Generic[M, T]):
+        def __call__(self, llm: LLM[M, T], **attrs: t.Any) -> T:
+            ...
+
+    class _llm_post_init_wrapper(t.Generic[M, T]):
+        def __call__(self, llm: LLM[M, T]) -> T:
+            ...
+
+
+def _wrapped_import_model(f: _import_model_wrapper[bentoml.Model, M, T]):
+    @functools.wraps(f)
+    def wrapper(
+        self: LLM[M, T], *decls: t.Any, trust_remote_code: bool | None = None, **attrs: t.Any
+    ) -> bentoml.Model:
+        trust_remote_code = first_not_none(trust_remote_code, default=self.__llm_trust_remote_code__)
+        # wrapped around custom init to provide some meta compression
+        # for all decls and attrs
+        (model_decls, model_attrs), _ = self.llm_parameters
+        decls = (*model_decls, *decls)
+        attrs = {**model_attrs, **attrs}
+        return f(self, *decls, trust_remote_code=trust_remote_code, **attrs)
+
+    return wrapper
+
+
+def _wrapped_load_model(f: _load_model_wrapper[M, T]):
+    @functools.wraps(f)
+    def wrapper(self: LLM[M, T], *decls: t.Any, **attrs: t.Any) -> M:
+        # wrapped around custom init to provide some meta compression
+        # for all decls and attrs
+        (model_decls, model_attrs), _ = self.llm_parameters
+        decls = (*model_decls, *decls)
+        attrs = {**model_attrs, **attrs}
+        return f(self, *decls, **attrs)
+
+    return wrapper
+
+
+def _wrapped_load_tokenizer(f: _load_tokenizer_wrapper[M, T]):
+    @functools.wraps(f)
+    def wrapper(self: LLM[M, T], **tokenizer_attrs: t.Any) -> T:
+        _, model_tokenizer_attrs = self.llm_parameters
+        tokenizer_attrs = {**model_tokenizer_attrs, **tokenizer_attrs}
+        return f(self, **tokenizer_attrs)
+
+    return wrapper
+
+
+def _wrapped_llm_post_init(f: _llm_post_init_wrapper[M, T]) -> t.Callable[[LLM[M, T]], None]:
+    @functools.wraps(f)
+    def wrapper(self: LLM[M, T]):
+        _default_post_init(self)
+        f(self)
+
+    return wrapper
+
+
+def _make_assignment_script(cls: type[LLM[M, T]]) -> t.Callable[[type[LLM[M, T]]], None]:
+    attributes = {
+        "import_model": _wrapped_import_model,
+        "load_model": _wrapped_load_model,
+        "load_tokenizer": _wrapped_load_tokenizer,
+        "llm_post_init": _wrapped_llm_post_init,
+    }
+    args: ListStr = []
+    anns: DictStrAny = {}
+    lines: ListStr = []
+    globs: DictStrAny = {
+        "cls": cls,
+        "_cached_attribute": attributes,
+        "_cached_getattribute_get": _object_getattribute.__get__,
+        "LLMInterface": LLMInterface,
+        "openllm": openllm,
+    }
+    # function initialisation
+    for func, impl in attributes.items():
+        globs[f"__wrapped_{func}"] = impl
+        impl_name = f"__wrapped_{func}"
+        cached_func_name = f"_cached_{cls.__name__}_func"
+        if func == "llm_post_init":
+            func_call = f"_impl_{cls.__name__}_{func}={impl_name}"
+        else:
+            func_call = f"_impl_{cls.__name__}_{func}={cached_func_name} if {cached_func_name} is not _cached_LLMInterface_getattr('{func}') else openllm.serialisation.{func}"
+        lines.extend(
+            [
+                "_cached_LLMInterface_getattr=_cached_getattribute_get(LLMInterface)",
+                f"{cached_func_name}=cls.{func}",
+                func_call,
+                _setattr_class(func, f"{impl_name}(_impl_{cls.__name__}_{func})"),
+            ]
+        )
+
+    # cached attribute initialisation
+    interface_anns = codegen.get_annotations(LLMInterface)
+    for v in {"bentomodel", "model", "tokenizer", "adapter_map"}:
+        lines.append(_setattr_class(f"__llm_{v}__", None))
+        anns[f"__llm_{v}__"] = interface_anns.get("__llm_{v}__")
+
+    if SHOW_CODEGEN:
+        logger.info("Generated script for %s:\n\n%s", cls.__name__, "\n".join(lines))
+
+    return codegen.generate_function(cls, "__assign_attr", lines, args=("cls", *args), globs=globs, annotations=anns)
+
+
 _AdaptersTuple: type[AdaptersTuple] = codegen.make_attr_tuple_class("AdaptersTuple", ["adapter_id", "name", "config"])
 
 
 @attr.define(slots=True, repr=False, init=False)
 class LLM(LLMInterface[M, T], ReprMixin):
     config: openllm.LLMConfig
     """The config instance to use for this LLM. This will be created based on config_class and available
@@ -476,54 +589,15 @@
 
         if "__openllm_internal__" in cd:
             if "config_class" not in cd:
                 cls.config_class = config_class
         elif "config_class" not in cd:
             raise RuntimeError("Missing required key 'config_class'. Make sure to define it within the LLM subclass.")
 
-        _custom_import = True
-        if cls.import_model is LLMInterface[M, T].import_model:
-            # using the default import model if no custom import is set
-            _custom_import = False
-            setattr(cls, "import_model", openllm.serialisation.import_model)
-        else:
-            import_func = getattr(cls, "import_model")
-
-            def _wrapped_import_model(
-                self: LLM[M, T], *decls: t.Any, trust_remote_code: bool, **attrs: t.Any
-            ) -> bentoml.Model:
-                # wrapped around custom init to provide some meta compression
-                # for all decls and attrs
-                (model_decls, model_attrs), _ = self.llm_parameters
-
-                decls = (*model_decls, *decls)
-                attrs = {**model_attrs, **attrs}
-
-                return import_func(self, *decls, trust_remote_code=trust_remote_code, **attrs)
-
-            setattr(cls, "import_model", functools.update_wrapper(_wrapped_import_model, cls.import_model))
-
-        if cls.llm_post_init is LLMInterface[M, T].llm_post_init:
-            # using the default post init if no custom post init is set
-            wrapped_post_init = _default_post_init
-        else:
-            original_post_init = getattr(cls, "llm_post_init")
-
-            def wrapped_post_init(self: LLM[M, T]) -> None:
-                _default_post_init(self)
-                original_post_init(self)
-
-        setattr(cls, "llm_post_init", wrapped_post_init)
-
-        cls.__llm_custom_import__ = _custom_import
-        cls.__llm_custom_load__ = False if cls.load_model is LLMInterface[M, T].load_model else True
-        cls.__llm_custom_tokenizer__ = False if cls.load_tokenizer is LLMInterface[M, T].load_tokenizer else True
-
-        for at in {"bentomodel", "model", "tokenizer", "adapter_map"}:
-            setattr(cls, f"__llm_{at}__", None)
+        _make_assignment_script(cls)(cls)
 
         # update docstring for given entrypoint
         for fn in {"generate", "generate_one", "generate_iterator"}:
             original_fn = getattr(cls, fn, getattr(LLMInterface, fn))
             original_fn.__doc__ = (
                 original_fn.__doc__
                 or f"""\
@@ -542,15 +616,14 @@
         if self.__llm_model__ is not None and self.bettertransformer and self.__llm_implementation__ == "pt":
             from optimum.bettertransformer import BetterTransformer
 
             self.__llm_model__ = t.cast(
                 M,
                 BetterTransformer.reverse(t.cast("transformers.PreTrainedModel", self.__llm_model__)),
             )
-
         openllm.serialisation.save_pretrained(self, save_directory, **attrs)
 
     @classmethod
     @overload
     def from_pretrained(
         cls,
         model_id: str | None = ...,
@@ -993,24 +1066,24 @@
     def model(self) -> M:
         """The model to use for this LLM. This shouldn't be set at runtime, rather let OpenLLM handle it."""
         # Run check for GPU
         if self.config["requires_gpu"] and openllm.utils.device_count() < 1:
             raise GpuNotAvailableError(f"{self} only supports running with GPU (None available).") from None
 
         if self.__llm_model__ is None:
-            self.__llm_model__ = t.cast(
-                M, openllm.serialisation.load_model(self, *self._model_decls, **self._model_attrs)
-            )
-        return t.cast(M, self.__llm_model__)
+            # NOTE: the signature of load_model here is the wrapper under _wrapped_load_model
+            self.__llm_model__ = self.load_model(*self._model_decls, **self._model_attrs)
+        return self.__llm_model__
 
     @property
     def tokenizer(self) -> T:
         """The tokenizer to use for this LLM. This shouldn't be set at runtime, rather let OpenLLM handle it."""
         if self.__llm_tokenizer__ is None:
-            self.__llm_tokenizer__ = t.cast(T, openllm.serialisation.load_tokenizer(self))
+            # NOTE: the signature of load_tokenizer here is the wrapper under _wrapped_load_tokenizer
+            self.__llm_tokenizer__ = self.load_tokenizer(**self._tokenizer_attrs)
         return self.__llm_tokenizer__
 
     def _default_ft_config(self, _adapter_type: AdapterType, inference_mode: bool) -> FineTuneConfig:
         strategy = first_not_none(
             self.config["fine_tune_strategies"].get(_adapter_type),
             default=FineTuneConfig(adapter_type=t.cast("PeftType", _adapter_type), llm_config_class=self.config_class),
         )
@@ -1200,15 +1273,15 @@
     # order of these fields matter here, make sure to sync it with
     # openllm.models.auto.factory.BaseAutoLLMClass.for_model
     def to_runner(
         self,
         models: list[bentoml.Model] | None = None,
         max_batch_size: int | None = None,
         max_latency_ms: int | None = None,
-        scheduling_strategy: type[Strategy] | None = None,
+        scheduling_strategy: type[bentoml.Strategy] | None = None,
     ) -> LLMRunner:
         """Convert this LLM into a Runner.
 
         Args:
             models: Any additional ``bentoml.Model`` to be included in this given models.
                     By default, this will be determined from the model_name.
             max_batch_size: The maximum batch size for the runner.
@@ -1288,31 +1361,66 @@
 
 
 @overload
 def Runner(
     model_name: str,
     *,
     model_id: str | None = None,
+    model_version: str | None = ...,
     init_local: t.Literal[False, True] = ...,
     **attrs: t.Any,
 ) -> LLMRunner:
     ...
 
 
 @overload
 def Runner(
     model_name: str,
     *,
     model_id: str = ...,
+    model_version: str | None = ...,
     models: list[bentoml.Model] | None = ...,
     max_batch_size: int | None = ...,
     max_latency_ms: int | None = ...,
     method_configs: dict[str, ModelSignatureDict | ModelSignature] | None = ...,
     embedded: t.Literal[True, False] = ...,
-    scheduling_strategy: type[Strategy] | None = ...,
+    scheduling_strategy: type[bentoml.Strategy] | None = ...,
+    **attrs: t.Any,
+) -> LLMRunner:
+    ...
+
+
+@overload
+def Runner(
+    model_name: str,
+    *,
+    ensure_available: bool | None = None,
+    init_local: bool = ...,
+    implementation: LiteralRuntime | None = None,
+    llm_config: openllm.LLMConfig | None = None,
+    **attrs: t.Any,
+) -> LLMRunner:
+    ...
+
+
+@overload
+def Runner(
+    model_name: str,
+    *args: t.Any,
+    model_id: str | None = ...,
+    model_version: str | None = ...,
+    llm_config: openllm.LLMConfig | None = ...,
+    runtime: t.Literal["ggml", "transformers"] | None = ...,
+    quantize: t.Literal["int8", "int4", "gptq"] | None = ...,
+    bettertransformer: str | bool | None = ...,
+    adapter_id: str | None = ...,
+    adapter_name: str | None = ...,
+    adapter_map: dict[str, str | None] | None = ...,
+    quantization_config: transformers.BitsAndBytesConfig | autogptq.BaseQuantizeConfig | None = None,
+    serialisation: t.Literal["safetensors", "legacy"] = ...,
     **attrs: t.Any,
 ) -> LLMRunner:
     ...
 
 
 def Runner(
     model_name: str,
```

### Comparing `openllm-0.2.5/src/openllm/_prompt.py` & `openllm-0.2.6/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/_quantisation.py` & `openllm-0.2.6/src/openllm/_quantisation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/_schema.py` & `openllm-0.2.6/src/openllm/_schema.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/_service.py` & `openllm-0.2.6/src/openllm/_service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/_strategies.py` & `openllm-0.2.6/src/openllm/_strategies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/_types.py` & `openllm-0.2.6/src/openllm/_types.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/cli.py` & `openllm-0.2.6/src/openllm/cli.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/client.py` & `openllm-0.2.6/src/openllm/client.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/exceptions.py` & `openllm-0.2.6/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/testing.py` & `openllm-0.2.6/src/openllm/testing.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/bundle/__init__.py` & `openllm-0.2.6/src/openllm/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/bundle/_package.py` & `openllm-0.2.6/src/openllm/bundle/_package.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/bundle/oci/Dockerfile-builder` & `openllm-0.2.6/src/openllm/bundle/oci/Dockerfile-builder`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/bundle/oci/__init__.py` & `openllm-0.2.6/src/openllm/bundle/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/__init__.py` & `openllm-0.2.6/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/auto/__init__.py` & `openllm-0.2.6/src/openllm/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/auto/configuration_auto.py` & `openllm-0.2.6/src/openllm/models/auto/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/auto/factory.py` & `openllm-0.2.6/src/openllm/models/auto/factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/auto/modeling_auto.py` & `openllm-0.2.6/src/openllm/models/auto/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.2.6/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.2.6/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/auto/modeling_vllm_auto.py` & `openllm-0.2.6/src/openllm/models/auto/modeling_vllm_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/baichuan/__init__.py` & `openllm-0.2.6/src/openllm/models/baichuan/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/baichuan/configuration_baichuan.py` & `openllm-0.2.6/src/openllm/models/baichuan/configuration_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/baichuan/modeling_baichuan.py` & `openllm-0.2.6/src/openllm/models/baichuan/modeling_baichuan.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,14 @@
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 
 
 class Baichuan(openllm.LLM["transformers.PreTrainedModel", "transformers.PreTrainedTokenizerBase"]):
     __openllm_internal__ = True
 
-    def llm_post_init(self):
-        self.device = torch.device("cuda")
-
     def sanitize_parameters(
         self,
         prompt: str,
         max_new_tokens: int | None = None,
         top_p: float | None = None,
         temperature: float | None = None,
         use_default_prompt_template: bool = False,
```

### Comparing `openllm-0.2.5/src/openllm/models/chatglm/__init__.py` & `openllm-0.2.6/src/openllm/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.2.6/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.2.6/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,14 @@
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 
 
 class ChatGLM(openllm.LLM["transformers.PreTrainedModel", "transformers.PreTrainedTokenizerFast"]):
     __openllm_internal__ = True
 
-    def llm_post_init(self):
-        self.device = torch.device("cuda")
-
     def import_model(self, *args: t.Any, trust_remote_code: bool = True, **attrs: t.Any) -> bentoml.Model:
         _, tokenizer_attrs = self.llm_parameters
 
         return bentoml.transformers.save_model(
             self.tag,
             transformers.AutoModel.from_pretrained(self.model_id, trust_remote_code=trust_remote_code),
             labels=generate_labels(self),
```

### Comparing `openllm-0.2.5/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.2.6/src/openllm/models/dolly_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.2.6/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.2.6/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,22 +18,20 @@
 
 import openllm
 
 from .configuration_dolly_v2 import DEFAULT_PROMPT_TEMPLATE
 from .configuration_dolly_v2 import END_KEY
 from .configuration_dolly_v2 import RESPONSE_KEY
 from .configuration_dolly_v2 import get_special_token_id
-from ...utils import normalize_attrs_to_model_tokenizer_pair
 
 
 if t.TYPE_CHECKING:
     import tensorflow as tf
     import torch
 
-    import bentoml
     import transformers
 else:
     tf = openllm.utils.LazyLoader("tf", globals(), "tensorflow")
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 
 logger = logging.getLogger(__name__)
@@ -257,26 +255,18 @@
         model_kwds = {
             "device_map": "auto" if torch.cuda.is_available() else None,
             "torch_dtype": torch.bfloat16,
         }
         tokenizer_kwds = {"padding_side": "left"}
         return model_kwds, tokenizer_kwds
 
-    def llm_post_init(self):
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-
-    def load_model(self, tag: bentoml.Tag, *args: t.Any, **attrs: t.Any) -> transformers.Pipeline:
-        (_, model_attrs), tokenizer_attrs = self.llm_parameters
-        normalized_model_attrs, normalized_tokenizer_attrs = normalize_attrs_to_model_tokenizer_pair(**attrs)
-        attrs = {**model_attrs, **normalized_model_attrs}
-        tokenizer_attrs = {**tokenizer_attrs, **normalized_tokenizer_attrs}
-        _ref = openllm.serialisation.get(self)
+    def load_model(self, *args: t.Any, **attrs: t.Any) -> transformers.Pipeline:
         return get_pipeline(
-            model=transformers.AutoModelForCausalLM.from_pretrained(_ref.path, **attrs),
-            tokenizer=transformers.AutoTokenizer.from_pretrained(_ref.path, **tokenizer_attrs),
+            model=transformers.AutoModelForCausalLM.from_pretrained(self._bentomodel.path, *args, **attrs),
+            tokenizer=self.tokenizer,
             _init=True,
             return_full_text=self.config.return_full_text,
         )
 
     def sanitize_parameters(
         self,
         prompt: str,
```

### Comparing `openllm-0.2.5/src/openllm/models/falcon/__init__.py` & `openllm-0.2.6/src/openllm/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.2.6/src/openllm/models/falcon/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.2.6/src/openllm/models/opt/modeling_opt.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,123 +9,131 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
+import logging
 import typing as t
 
+import bentoml
 import openllm
 
-from .configuration_falcon import DEFAULT_PROMPT_TEMPLATE
+from .configuration_opt import DEFAULT_PROMPT_TEMPLATE
 from ..._prompt import default_formatter
+from ...utils import generate_labels
 
 
 if t.TYPE_CHECKING:
     import torch
 
-    import bentoml
     import transformers
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 
+logger = logging.getLogger(__name__)
 
-class Falcon(openllm.LLM["transformers.PreTrainedModel", "transformers.PreTrainedTokenizerBase"]):
+
+class OPT(openllm.LLM["transformers.OPTForCausalLM", "transformers.GPT2Tokenizer"]):
     __openllm_internal__ = True
 
+    def llm_post_init(self):
+        self.dtype = torch.float16 if torch.cuda.is_available() else torch.float32
+
     @property
-    def import_kwargs(self):
-        model_kwds = {"torch_dtype": torch.bfloat16, "device_map": "auto" if torch.cuda.is_available() else None}
-        tokenizer_kwds: dict[str, t.Any] = {}
+    def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]] | None:
+        model_kwds = {
+            "device_map": "auto" if torch.cuda.is_available() and torch.cuda.device_count() > 1 else None,
+            "torch_dtype": torch.float16 if torch.cuda.is_available() else torch.float32,
+        }
+        tokenizer_kwds = {
+            "padding_side": "left",
+            "truncation_side": "left",
+        }
         return model_kwds, tokenizer_kwds
 
-    def llm_post_init(self):
-        self.device = torch.device("cuda")
+    def import_model(self, *args: t.Any, trust_remote_code: bool = False, **attrs: t.Any) -> bentoml.Model:
+        _, tokenizer_attrs = self.llm_parameters
+
+        torch_dtype = attrs.pop("torch_dtype", self.dtype)
 
-    def load_model(self, tag: bentoml.Tag, *args: t.Any, **attrs: t.Any) -> t.Any:
-        trust_remote_code = attrs.pop("trust_remote_code", True)
-        return transformers.AutoModelForCausalLM.from_pretrained(
-            openllm.serialisation.get(self).path, trust_remote_code=trust_remote_code, **attrs
+        config = transformers.AutoConfig.from_pretrained(self.model_id)
+        tokenizer = transformers.AutoTokenizer.from_pretrained(self.model_id, **tokenizer_attrs)
+        tokenizer.pad_token_id = config.pad_token_id
+        model = t.cast(
+            "transformers.OPTForCausalLM",
+            transformers.AutoModelForCausalLM.from_pretrained(
+                self.model_id, torch_dtype=torch_dtype, trust_remote_code=trust_remote_code, **attrs
+            ),
+        )
+        return bentoml.transformers.save_model(
+            self.tag,
+            model,
+            custom_objects={"tokenizer": tokenizer},
+            labels=generate_labels(self),
         )
 
-    def load_tokenizer(self, tag: bentoml.Tag, **attrs: t.Any) -> t.Any:
-        trust_remote_code = attrs.pop("trust_remote_code", True)
-        return transformers.AutoTokenizer.from_pretrained(
-            openllm.serialisation.get(self).path, trust_remote_code=trust_remote_code, **attrs
+    def load_model(self, *args: t.Any, **attrs: t.Any) -> transformers.OPTForCausalLM:
+        torch_dtype = attrs.pop("torch_dtype", self.dtype)
+        model: transformers.OPTForCausalLM = transformers.AutoModelForCausalLM.from_pretrained(
+            bentoml.transformers.get(self.tag).path, *args, torch_dtype=torch_dtype, **attrs
         )
+        return model
 
     def sanitize_parameters(
         self,
         prompt: str,
         max_new_tokens: int | None = None,
+        temperature: float | None = None,
         top_k: int | None = None,
         num_return_sequences: int | None = None,
-        eos_token_id: int | None = None,
         use_default_prompt_template: bool = False,
         **attrs: t.Any,
     ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
         if use_default_prompt_template:
             template_variables = default_formatter.extract_template_variables(DEFAULT_PROMPT_TEMPLATE)
             prompt_variables = {k: v for k, v in attrs.items() if k in template_variables}
             if "instruction" in prompt_variables:
                 raise RuntimeError(
-                    "'instruction' should be passed as the first argument instead of "
-                    "kwargs when 'use_default_prompt_template=True'"
+                    "'instruction' should be passed as the first argument "
+                    "instead of kwargs when 'use_default_prompt_template=True'"
                 )
             try:
                 prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
             except KeyError as e:
                 raise RuntimeError(
                     f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. "
                     "Use 'use_default_prompt_template=False' to disable the default prompt template."
                 ) from None
         else:
             prompt_text = prompt
 
         generation_config = {
             "max_new_tokens": max_new_tokens,
+            "temperature": temperature,
             "top_k": top_k,
             "num_return_sequences": num_return_sequences,
-            "eos_token_id": eos_token_id,
-            **attrs,
         }
-
         return prompt_text, generation_config, {}
 
-    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str:
-        return generation_result[0]
+    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **attrs: t.Any) -> str:
+        if len(generation_result) == 1:
+            if self.config.format_outputs:
+                logger.warning("'format_outputs' doesn't have any effect when 'num_return_sequences=1'")
+            return generation_result[0]
+
+        if self.config.format_outputs:
+            return "Generated result:\n" + "\n -".join(generation_result)
+        else:
+            return "\n".join(generation_result)
 
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
-        eos_token_id = attrs.pop("eos_token_id", self.tokenizer.eos_token_id)
-        inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-        with torch.inference_mode(), torch.autocast("cuda", dtype=torch.float16):
-            outputs = self.model.generate(
-                input_ids=inputs["input_ids"],
-                attention_mask=inputs["attention_mask"],
-                generation_config=self.config.model_construct_env(
-                    eos_token_id=eos_token_id, **attrs
-                ).to_generation_config(),
+        with torch.inference_mode():
+            inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
+            generated_tensors = self.model.generate(
+                **inputs,
+                do_sample=True,
+                generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
             )
-            return self.tokenizer.batch_decode(outputs, skip_special_tokens=True)
-
-    def generate_one(
-        self, prompt: str, stop: list[str], **preprocess_generate_kwds: t.Any
-    ) -> list[dict[t.Literal["generated_text"], str]]:
-        from ..._generation import StopSequenceCriteria
-
-        max_new_tokens = preprocess_generate_kwds.pop("max_new_tokens", 200)
-        encoded_inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-        src_len = encoded_inputs["input_ids"].shape[1]
-        stopping_criteria = preprocess_generate_kwds.pop("stopping_criteria", transformers.StoppingCriteriaList([]))
-        stopping_criteria.append(StopSequenceCriteria(stop, self.tokenizer))
-        outputs = self.model.generate(
-            encoded_inputs["input_ids"], max_new_tokens=max_new_tokens, stopping_criteria=stopping_criteria
-        )
-
-        result = self.tokenizer.decode(outputs[0].tolist()[src_len:])
-        # Inference API returns the stop sequence
-        for stop_seq in stop:
-            if result.endswith(stop_seq):
-                result = result[: -len(stop_seq)]
-        return [{"generated_text": result}]
+            return self.tokenizer.batch_decode(generated_tensors, skip_special_tokens=True)
```

### Comparing `openllm-0.2.5/src/openllm/models/flan_t5/__init__.py` & `openllm-0.2.6/src/openllm/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.2.6/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.2.6/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,17 +27,14 @@
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
 
 
 class FlanT5(openllm.LLM["transformers.T5ForConditionalGeneration", "transformers.T5TokenizerFast"]):
     __openllm_internal__ = True
 
-    def llm_post_init(self):
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-
     def sanitize_parameters(
         self,
         prompt: str,
         max_new_tokens: int | None = None,
         temperature: float | None = None,
         top_k: int | None = None,
         top_p: float | None = None,
```

### Comparing `openllm-0.2.5/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.2.6/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.2.6/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.2.6/src/openllm/models/gpt_neox/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/gpt_neox/configuration_gpt_neox.py` & `openllm-0.2.6/src/openllm/models/gpt_neox/configuration_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/gpt_neox/modeling_gpt_neox.py` & `openllm-0.2.6/src/openllm/models/gpt_neox/modeling_gpt_neox.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from .configuration_gpt_neox import DEFAULT_PROMPT_TEMPLATE
 from ..._prompt import default_formatter
 
 
 if t.TYPE_CHECKING:
     import torch
 
-    import bentoml
     import transformers
 else:
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
 
 
 logger = logging.getLogger(__name__)
@@ -73,16 +72,16 @@
         model_kwds = {"device_map": "auto" if torch.cuda.device_count() > 1 else None}
         tokenizer_kwds: dict[str, t.Any] = {}
         return model_kwds, tokenizer_kwds
 
     def postprocess_generate(self, prompt: str, generation_result: list[str], **_: t.Any) -> str:
         return generation_result[0]
 
-    def load_model(self, tag: bentoml.Tag, *args: t.Any, **attrs: t.Any) -> t.Any:
-        model = transformers.AutoModelForCausalLM.from_pretrained(self._bentomodel.path, **attrs)
+    def load_model(self, *args: t.Any, **attrs: t.Any) -> transformers.GPTNeoXForCausalLM:
+        model = transformers.AutoModelForCausalLM.from_pretrained(self._bentomodel.path, *args, **attrs)
         if self.config.use_half_precision:
             model.half()
         return model
 
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
         from ..._generation import StopOnTokens
```

### Comparing `openllm-0.2.5/src/openllm/models/llama/__init__.py` & `openllm-0.2.6/src/openllm/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/llama/configuration_llama.py` & `openllm-0.2.6/src/openllm/models/llama/configuration_llama.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/llama/modeling_llama.py` & `openllm-0.2.6/src/openllm/models/llama/modeling_llama.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,17 +36,14 @@
 
 logger = logging.getLogger(__name__)
 
 
 class LlaMA(openllm.LLM["transformers.LlamaForCausalLM", "transformers.LlamaTokenizerFast"]):
     __openllm_internal__ = True
 
-    def llm_post_init(self):
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-
     def sanitize_parameters(
         self,
         prompt: str,
         top_k: int | None = None,
         top_p: float | None = None,
         temperature: float | None = None,
         max_new_tokens: int | None = None,
```

### Comparing `openllm-0.2.5/src/openllm/models/llama/modeling_vllm_llama.py` & `openllm-0.2.6/src/openllm/models/llama/modeling_vllm_llama.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from ..._prompt import default_formatter
 
 
 if t.TYPE_CHECKING:
     import torch
     import vllm
 
-    import bentoml
     import transformers
 else:
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     vllm = openllm.utils.LazyLoader("vllm", globals(), "vllm")
 
 
@@ -75,16 +74,16 @@
         model_kwds = {"device_map": "auto" if torch.cuda.device_count() > 1 else None}
         tokenizer_kwds: dict[str, t.Any] = {}
         return model_kwds, tokenizer_kwds
 
     def postprocess_generate(self, prompt: str, generation_result: list[str], **_: t.Any) -> str:
         return generation_result[0]
 
-    def load_model(self, tag: bentoml.Tag, *args: t.Any, **attrs: t.Any) -> t.Any:
-        model = transformers.AutoModelForCausalLM.from_pretrained(self._bentomodel.path, **attrs)
+    def load_model(self, *args: t.Any, **attrs: t.Any) -> t.Any:
+        model = transformers.AutoModelForCausalLM.from_pretrained(self._bentomodel.path, *args, **attrs)
         if self.config.use_half_precision:
             model.half()
         return model
 
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
         from ..._generation import StopOnTokens
```

### Comparing `openllm-0.2.5/src/openllm/models/mpt/__init__.py` & `openllm-0.2.6/src/openllm/models/mpt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/mpt/configuration_mpt.py` & `openllm-0.2.6/src/openllm/models/mpt/configuration_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/mpt/modeling_mpt.py` & `openllm-0.2.6/src/openllm/models/mpt/modeling_mpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     return config
 
 
 class MPT(openllm.LLM["transformers.PreTrainedModel", "transformers.GPTNeoXTokenizerFast"]):
     __openllm_internal__ = True
 
     def llm_post_init(self):
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.dtype = torch.bfloat16 if torch.cuda.is_available() else torch.float32
 
     @property
     def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]] | None:
         model_kwds = {"torch_dtype": torch.bfloat16 if torch.cuda.is_available() else torch.float32}
         tokenizer_kwds = {"padding_side": "left"}
         return model_kwds, tokenizer_kwds
@@ -106,20 +105,20 @@
                 model,
                 custom_objects={"tokenizer": tokenizer},
                 labels=generate_labels(self),
             )
         finally:
             torch.cuda.empty_cache()
 
-    def load_model(self, tag: bentoml.Tag, *args: t.Any, **attrs: t.Any) -> transformers.PreTrainedModel:
+    def load_model(self, *args: t.Any, **attrs: t.Any) -> transformers.PreTrainedModel:
         torch_dtype = attrs.pop("torch_dtype", self.dtype)
         device_map = attrs.pop("device_map", None)
         trust_remote_code = attrs.pop("trust_remote_code", True)
 
-        _ref = bentoml.transformers.get(tag)
+        _ref = bentoml.transformers.get(self.tag)
         config = get_mpt_config(
             _ref.path,
             self.config.max_sequence_length,
             self.device,
             device_map=device_map,
             trust_remote_code=trust_remote_code,
         )
```

### Comparing `openllm-0.2.5/src/openllm/models/opt/__init__.py` & `openllm-0.2.6/src/openllm/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/opt/configuration_opt.py` & `openllm-0.2.6/src/openllm/models/opt/configuration_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/opt/modeling_flax_opt.py` & `openllm-0.2.6/src/openllm/models/opt/modeling_flax_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/opt/modeling_opt.py` & `openllm-0.2.6/src/openllm/models/opt/modeling_tf_opt.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,74 +21,49 @@
 
 from .configuration_opt import DEFAULT_PROMPT_TEMPLATE
 from ..._prompt import default_formatter
 from ...utils import generate_labels
 
 
 if t.TYPE_CHECKING:
-    import torch
-
     import transformers
 else:
-    torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 
+
 logger = logging.getLogger(__name__)
 
 
-class OPT(openllm.LLM["transformers.OPTForCausalLM", "transformers.GPT2Tokenizer"]):
+class TFOPT(openllm.LLM["transformers.TFOPTForCausalLM", "transformers.GPT2Tokenizer"]):
     __openllm_internal__ = True
 
-    def llm_post_init(self):
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        self.dtype = torch.float16 if torch.cuda.is_available() else torch.float32
-
     @property
     def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]] | None:
-        model_kwds = {
-            "device_map": "auto" if torch.cuda.is_available() and torch.cuda.device_count() > 1 else None,
-            "torch_dtype": torch.float16 if torch.cuda.is_available() else torch.float32,
-        }
         tokenizer_kwds = {
             "padding_side": "left",
             "truncation_side": "left",
         }
-        return model_kwds, tokenizer_kwds
+        return {}, tokenizer_kwds
 
     def import_model(self, *args: t.Any, trust_remote_code: bool = False, **attrs: t.Any) -> bentoml.Model:
         _, tokenizer_attrs = self.llm_parameters
 
-        torch_dtype = attrs.pop("torch_dtype", self.dtype)
-
         config = transformers.AutoConfig.from_pretrained(self.model_id)
         tokenizer = transformers.AutoTokenizer.from_pretrained(self.model_id, **tokenizer_attrs)
         tokenizer.pad_token_id = config.pad_token_id
-        model = t.cast(
-            "transformers.OPTForCausalLM",
-            transformers.AutoModelForCausalLM.from_pretrained(
-                self.model_id, torch_dtype=torch_dtype, trust_remote_code=trust_remote_code, **attrs
-            ),
+        model: transformers.TFOPTForCausalLM = transformers.TFOPTForCausalLM.from_pretrained(
+            self.model_id, trust_remote_code=trust_remote_code, **attrs
         )
         return bentoml.transformers.save_model(
             self.tag,
             model,
             custom_objects={"tokenizer": tokenizer},
             labels=generate_labels(self),
         )
 
-    def load_model(self, tag: bentoml.Tag, *args: t.Any, **attrs: t.Any) -> transformers.OPTForCausalLM:
-        torch_dtype = attrs.pop("torch_dtype", self.dtype)
-        trust_remote_code = attrs.pop("trust_remote_code", False)
-
-        _ref = bentoml.transformers.get(tag)
-        model: transformers.OPTForCausalLM = transformers.AutoModelForCausalLM.from_pretrained(
-            _ref.path, trust_remote_code=trust_remote_code, torch_dtype=torch_dtype, **attrs
-        )
-        return model
-
     def sanitize_parameters(
         self,
         prompt: str,
         max_new_tokens: int | None = None,
         temperature: float | None = None,
         top_k: int | None = None,
         num_return_sequences: int | None = None,
@@ -129,15 +104,14 @@
 
         if self.config.format_outputs:
             return "Generated result:\n" + "\n -".join(generation_result)
         else:
             return "\n".join(generation_result)
 
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
-        with torch.inference_mode():
-            inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-            generated_tensors = self.model.generate(
-                **inputs,
-                do_sample=True,
-                generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
-            )
-            return self.tokenizer.batch_decode(generated_tensors, skip_special_tokens=True)
+        input_ids = self.tokenizer(prompt, return_tensors="tf")
+        generated_tensors = self.model.generate(
+            **input_ids,
+            do_sample=True,
+            generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
+        )
+        return self.tokenizer.batch_decode(generated_tensors, skip_special_tokens=True)
```

### Comparing `openllm-0.2.5/src/openllm/models/opt/modeling_tf_opt.py` & `openllm-0.2.6/src/openllm/models/falcon/modeling_falcon.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,109 +9,107 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
-import logging
 import typing as t
 
-import bentoml
 import openllm
 
-from .configuration_opt import DEFAULT_PROMPT_TEMPLATE
+from .configuration_falcon import DEFAULT_PROMPT_TEMPLATE
 from ..._prompt import default_formatter
-from ...utils import generate_labels
 
 
 if t.TYPE_CHECKING:
+    import torch
+
     import transformers
 else:
+    torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 
 
-logger = logging.getLogger(__name__)
-
-
-class TFOPT(openllm.LLM["transformers.TFOPTForCausalLM", "transformers.GPT2Tokenizer"]):
+class Falcon(openllm.LLM["transformers.PreTrainedModel", "transformers.PreTrainedTokenizerBase"]):
     __openllm_internal__ = True
 
     @property
-    def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]] | None:
-        tokenizer_kwds = {
-            "padding_side": "left",
-            "truncation_side": "left",
-        }
-        return {}, tokenizer_kwds
-
-    def import_model(self, *args: t.Any, trust_remote_code: bool = False, **attrs: t.Any) -> bentoml.Model:
-        _, tokenizer_attrs = self.llm_parameters
-
-        config = transformers.AutoConfig.from_pretrained(self.model_id)
-        tokenizer = transformers.AutoTokenizer.from_pretrained(self.model_id, **tokenizer_attrs)
-        tokenizer.pad_token_id = config.pad_token_id
-        model: transformers.TFOPTForCausalLM = transformers.TFOPTForCausalLM.from_pretrained(
-            self.model_id, trust_remote_code=trust_remote_code, **attrs
-        )
-        return bentoml.transformers.save_model(
-            self.tag,
-            model,
-            custom_objects={"tokenizer": tokenizer},
-            labels=generate_labels(self),
-        )
+    def import_kwargs(self):
+        model_kwds = {"torch_dtype": torch.bfloat16, "device_map": "auto" if torch.cuda.is_available() else None}
+        tokenizer_kwds: dict[str, t.Any] = {}
+        return model_kwds, tokenizer_kwds
 
     def sanitize_parameters(
         self,
         prompt: str,
         max_new_tokens: int | None = None,
-        temperature: float | None = None,
         top_k: int | None = None,
         num_return_sequences: int | None = None,
+        eos_token_id: int | None = None,
         use_default_prompt_template: bool = False,
         **attrs: t.Any,
     ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
         if use_default_prompt_template:
             template_variables = default_formatter.extract_template_variables(DEFAULT_PROMPT_TEMPLATE)
             prompt_variables = {k: v for k, v in attrs.items() if k in template_variables}
             if "instruction" in prompt_variables:
                 raise RuntimeError(
-                    "'instruction' should be passed as the first argument "
-                    "instead of kwargs when 'use_default_prompt_template=True'"
+                    "'instruction' should be passed as the first argument instead of "
+                    "kwargs when 'use_default_prompt_template=True'"
                 )
             try:
                 prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
             except KeyError as e:
                 raise RuntimeError(
                     f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. "
                     "Use 'use_default_prompt_template=False' to disable the default prompt template."
                 ) from None
         else:
             prompt_text = prompt
 
         generation_config = {
             "max_new_tokens": max_new_tokens,
-            "temperature": temperature,
             "top_k": top_k,
             "num_return_sequences": num_return_sequences,
+            "eos_token_id": eos_token_id,
+            **attrs,
         }
-        return prompt_text, generation_config, {}
 
-    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **attrs: t.Any) -> str:
-        if len(generation_result) == 1:
-            if self.config.format_outputs:
-                logger.warning("'format_outputs' doesn't have any effect when 'num_return_sequences=1'")
-            return generation_result[0]
+        return prompt_text, generation_config, {}
 
-        if self.config.format_outputs:
-            return "Generated result:\n" + "\n -".join(generation_result)
-        else:
-            return "\n".join(generation_result)
+    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str:
+        return generation_result[0]
 
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
-        input_ids = self.tokenizer(prompt, return_tensors="tf")
-        generated_tensors = self.model.generate(
-            **input_ids,
-            do_sample=True,
-            generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
+        eos_token_id = attrs.pop("eos_token_id", self.tokenizer.eos_token_id)
+        inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
+        with torch.inference_mode(), torch.autocast("cuda", dtype=torch.float16):
+            outputs = self.model.generate(
+                input_ids=inputs["input_ids"],
+                attention_mask=inputs["attention_mask"],
+                generation_config=self.config.model_construct_env(
+                    eos_token_id=eos_token_id, **attrs
+                ).to_generation_config(),
+            )
+            return self.tokenizer.batch_decode(outputs, skip_special_tokens=True)
+
+    def generate_one(
+        self, prompt: str, stop: list[str], **preprocess_generate_kwds: t.Any
+    ) -> list[dict[t.Literal["generated_text"], str]]:
+        from ..._generation import StopSequenceCriteria
+
+        max_new_tokens = preprocess_generate_kwds.pop("max_new_tokens", 200)
+        encoded_inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
+        src_len = encoded_inputs["input_ids"].shape[1]
+        stopping_criteria = preprocess_generate_kwds.pop("stopping_criteria", transformers.StoppingCriteriaList([]))
+        stopping_criteria.append(StopSequenceCriteria(stop, self.tokenizer))
+        outputs = self.model.generate(
+            encoded_inputs["input_ids"], max_new_tokens=max_new_tokens, stopping_criteria=stopping_criteria
         )
-        return self.tokenizer.batch_decode(generated_tensors, skip_special_tokens=True)
+
+        result = self.tokenizer.decode(outputs[0].tolist()[src_len:])
+        # Inference API returns the stop sequence
+        for stop_seq in stop:
+            if result.endswith(stop_seq):
+                result = result[: -len(stop_seq)]
+        return [{"generated_text": result}]
```

### Comparing `openllm-0.2.5/src/openllm/models/stablelm/__init__.py` & `openllm-0.2.6/src/openllm/models/stablelm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.2.6/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.2.6/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 logger = logging.getLogger(__name__)
 
 
 class StableLM(openllm.LLM["transformers.GPTNeoXForCausalLM", "transformers.GPTNeoXTokenizerFast"]):
     __openllm_internal__ = True
 
     def llm_post_init(self):
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.bettertransformer = True if not torch.cuda.is_available() else False
 
     @property
     def import_kwargs(self):
         model_kwds = {"torch_dtype": torch.float16 if torch.cuda.is_available() else torch.float32}
         tokenizer_kwds: dict[str, t.Any] = {}
         return model_kwds, tokenizer_kwds
```

### Comparing `openllm-0.2.5/src/openllm/models/starcoder/__init__.py` & `openllm-0.2.6/src/openllm/models/starcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.2.6/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.2.6/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,14 @@
 EOD = "<|endoftext|>"
 FIM_INDICATOR = "<FILL_HERE>"
 
 
 class StarCoder(openllm.LLM["transformers.GPTBigCodeForCausalLM", "transformers.GPT2TokenizerFast"]):
     __openllm_internal__ = True
 
-    def llm_post_init(self):
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-
     @property
     def import_kwargs(self):
         model_kwds = {
             "device_map": "auto" if torch.cuda.is_available() and torch.cuda.device_count() > 1 else None,
             "torch_dtype": torch.float16 if torch.cuda.is_available() else torch.float32,
         }
         tokenizer_kwds = {"padding_side": "left"}
```

### Comparing `openllm-0.2.5/src/openllm/playground/__init__.py` & `openllm-0.2.6/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/playground/_meta.yml` & `openllm-0.2.6/src/openllm/playground/_meta.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/playground/falcon_tuned.py` & `openllm-0.2.6/src/openllm/playground/falcon_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/playground/features.py` & `openllm-0.2.6/src/openllm/playground/features.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/playground/llama2_qlora.py` & `openllm-0.2.6/src/openllm/playground/llama2_qlora.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 class TrainingArguments:
     per_device_train_batch_size: int = dataclasses.field(default=1)
     gradient_checkpointing: bool = dataclasses.field(default=True)
     bf16: bool = dataclasses.field(default=torch.cuda.get_device_capability()[0] == 8)
     learning_rate: float = dataclasses.field(default=5e-5)
     num_train_epochs: int = dataclasses.field(default=3)
     logging_steps: int = dataclasses.field(default=1)
-    logging_strategy: str = dataclasses.field(default="steps")
+    report_to: str = dataclasses.field(default="none")
     output_dir: str = dataclasses.field(default=os.path.join(os.getcwd(), "outputs", "llama"))
     save_strategy: str = dataclasses.field(default="no")
 
 
 @dataclasses.dataclass
 class ModelArguments:
     model_id: str = dataclasses.field(default=DEFAULT_MODEL_ID)
```

### Comparing `openllm-0.2.5/src/openllm/playground/opt_tuned.py` & `openllm-0.2.6/src/openllm/playground/opt_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/serialisation/constants.py` & `openllm-0.2.6/src/openllm/serialisation/constants.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/serialisation/ggml.py` & `openllm-0.2.6/src/openllm/serialisation/ggml.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,40 +78,36 @@
 
     By default, it will try to find check the model in the local store.
     If model is not found, it will raises a ``bentoml.exceptions.NotFound``.
     """
     raise NotImplementedError("Currently work in progress.")
 
 
-def load_tokenizer(llm: openllm.LLM[t.Any, T]) -> TokenizerProtocol[T]:
+def load_tokenizer(llm: openllm.LLM[t.Any, T], **tokenizer_attrs: t.Any) -> TokenizerProtocol[T]:
     """Load the tokenizer from BentoML store.
 
     By default, it will try to find the bentomodel whether it is in store..
     If model is not found, it will raises a ``bentoml.exceptions.NotFound``.
     """
-    (_, _), tokenizer_attrs = llm.llm_parameters
-    if llm.__llm_custom_tokenizer__:
-        tokenizer = llm.load_tokenizer(llm.tag, **tokenizer_attrs)
+    bentomodel_fs = llm._bentomodel._fs
+    if bentomodel_fs.isfile(CUSTOM_OBJECTS_FILENAME):
+        with bentomodel_fs.open(CUSTOM_OBJECTS_FILENAME, "rb") as cofile:
+            try:
+                tokenizer = cloudpickle.load(t.cast("t.IO[bytes]", cofile))["tokenizer"]
+            except KeyError:
+                # This could happen if users implement their own import_model
+                raise OpenLLMException(
+                    "Model does not have tokenizer. Make sure to save \
+                    the tokenizer within the model via 'custom_objects'.\
+                    For example: bentoml.transformers.save_model(..., custom_objects={'tokenizer': tokenizer}))"
+                ) from None
     else:
-        bentomodel_fs = llm._bentomodel._fs
-        if bentomodel_fs.isfile(CUSTOM_OBJECTS_FILENAME):
-            with bentomodel_fs.open(CUSTOM_OBJECTS_FILENAME, "rb") as cofile:
-                try:
-                    tokenizer = cloudpickle.load(t.cast("t.IO[bytes]", cofile))["tokenizer"]
-                except KeyError:
-                    # This could happen if users implement their own import_model
-                    raise OpenLLMException(
-                        "Model does not have tokenizer. Make sure to save \
-                        the tokenizer within the model via 'custom_objects'.\
-                        For example: bentoml.transformers.save_model(..., custom_objects={'tokenizer': tokenizer}))"
-                    ) from None
-        else:
-            tokenizer = transformers.AutoTokenizer.from_pretrained(
-                bentomodel_fs.getsyspath("/"),
-                trust_remote_code=llm.__llm_trust_remote_code__,
-                **tokenizer_attrs,
-            )
+        tokenizer = transformers.AutoTokenizer.from_pretrained(
+            bentomodel_fs.getsyspath("/"),
+            trust_remote_code=llm.__llm_trust_remote_code__,
+            **tokenizer_attrs,
+        )
     return t.cast("TokenizerProtocol[T]", tokenizer)
 
 
 def save_pretrained(llm: openllm.LLM[t.Any, t.Any], save_directory: str, **attrs: t.Any) -> None:
     raise NotImplementedError("Currently work in progress.")
```

### Comparing `openllm-0.2.5/src/openllm/serialisation/transformers.py` & `openllm-0.2.6/src/openllm/serialisation/transformers.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,16 @@
 """Serialisation related implementation for Transformers-based implementation."""
 
 from __future__ import annotations
 import copy
 import importlib
 import typing as t
 
-import cloudpickle
-
 import bentoml
 from bentoml._internal.frameworks.transformers import make_default_signatures
-from bentoml._internal.models.model import CUSTOM_OBJECTS_FILENAME
 from bentoml._internal.models.model import ModelOptions
 
 from .constants import FRAMEWORK_TO_AUTOCLASS_MAPPING
 from .constants import HUB_ATTRS
 from ..exceptions import OpenLLMException
 from ..utils import LazyLoader
 from ..utils import first_not_none
@@ -44,16 +41,14 @@
     import openllm
     import transformers as _transformers
     from transformers.models.auto.auto_factory import _BaseAutoModelClass
 
     from .._llm import M
     from .._llm import T
     from .._types import DictStrAny
-    from .._types import ModelProtocol
-    from .._types import TokenizerProtocol
 else:
     autogptq = LazyLoader("autogptq", globals(), "auto_gptq")
     _transformers = LazyLoader("_transformers", globals(), "transformers")
     torch = LazyLoader("torch", globals(), "torch")
 
 
 def process_transformers_config(
@@ -73,15 +68,15 @@
             _transformers.AutoConfig.from_pretrained(
                 model_id, return_unused_kwargs=True, trust_remote_code=trust_remote_code, **hub_attrs, **copied_attrs
             ),
         )
     return config, hub_attrs, attrs
 
 
-def infer_tokenizers_class_for_llm(__llm: openllm.LLM[t.Any, T]) -> TokenizerProtocol[T]:
+def infer_tokenizers_class_for_llm(__llm: openllm.LLM[t.Any, T]) -> T:
     tokenizer_class = __llm.config["tokenizer_class"]
     if tokenizer_class is None:
         tokenizer_class = "AutoTokenizer"
     __cls = getattr(_transformers, tokenizer_class)
     if __cls is None:
         raise ValueError(
             f"{tokenizer_class} is not a valid Tokenizer class from 'transformers.' Set '{__llm}.__config__[\"trust_remote_code\"] = True' and try again."
@@ -134,29 +129,26 @@
     Args:
         llm: The LLM instance for this given model.
         trust_remote_code: Whether to trust the remote code when loading the model.
         *decls: Args to be passed into AutoModelForSeq2SeqLM or AutoModelForCausalLM (+ TF, Flax variants).
         **attrs: Kwargs to be passed into AutoModelForSeq2SeqLM or AutoModelForCausalLM (+ TF, Flax variants).
     """
     config, hub_attrs, attrs = process_transformers_config(llm.model_id, trust_remote_code, **attrs)
-
-    # NOTE: get the base args and attrs, then
-    # allow override via import_model
-    (model_decls, model_attrs), tokenizer_attrs = llm.llm_parameters
-    decls = (*model_decls, *decls)
-    attrs = {**model_attrs, **attrs}
-
-    safe_serialisation = llm._serialisation_format == "safetensors"
+    _, tokenizer_attrs = llm.llm_parameters
     quantize_method = llm._quantize_method
-
+    safe_serialisation = first_not_none(
+        attrs.get("safe_serialization"), default=llm._serialisation_format == "safetensors"
+    )
+    if llm.__llm_implementation__ == "vllm":
+        # Disable safe serialization with vLLM
+        safe_serialisation = False
     metadata: DictStrAny = {
         "safe_serialisation": safe_serialisation,
         "_quantize": quantize_method if quantize_method is not None else False,
     }
-
     signatures: DictStrAny = {}
     if quantize_method == "gptq":
         if not is_autogptq_available():
             raise OpenLLMException(
                 "GPTQ quantisation requires 'auto-gptq' (Not found in local environment). Install it with 'pip install \"openllm[gptq]\"'"
             )
         if llm.config["model_type"] != "causal_lm":
@@ -256,50 +248,42 @@
         return model
     except bentoml.exceptions.NotFound:
         if auto_import:
             return import_model(llm, trust_remote_code=llm.__llm_trust_remote_code__)
         raise
 
 
-def load_model(llm: openllm.LLM[M, t.Any], *decls: t.Any, **attrs: t.Any) -> ModelProtocol[M]:
+def load_model(llm: openllm.LLM[M, t.Any], *decls: t.Any, **attrs: t.Any) -> M:
     """Load the model from BentoML store.
 
     By default, it will try to find check the model in the local store.
     If model is not found, it will raises a ``bentoml.exceptions.NotFound``.
     """
     config, hub_attrs, attrs = process_transformers_config(llm.model_id, llm.__llm_trust_remote_code__, **attrs)
-    # NOTE: get the base args and attrs, then
-    # allow override via import_model
-    (model_decls, model_attrs), _ = llm.llm_parameters
-    decls = (*model_decls, *decls)
-    attrs = {**model_attrs, **attrs}
     metadata = llm._bentomodel.info.metadata
     safe_serialization = first_not_none(
         t.cast(t.Optional[bool], metadata.get("safe_serialisation", None)),
         attrs.pop("safe_serialization", None),
         default=llm._serialisation_format == "safetensors",
     )
     if "_quantize" in metadata and metadata["_quantize"] == "gptq":
         if not is_autogptq_available():
             raise OpenLLMException(
                 "GPTQ quantisation requires 'auto-gptq' (Not found in local environment). Install it with 'pip install \"openllm[gptq]\"'"
             )
         if llm.config["model_type"] != "causal_lm":
             raise OpenLLMException(f"GPTQ only support Causal LM (got {llm.__class__} of {llm.config['model_type']})")
-        return t.cast(
-            "ModelProtocol[M]",
-            autogptq.AutoGPTQForCausalLM.from_quantized(
-                llm._bentomodel.path,
-                *decls,
-                quantize_config=t.cast("autogptq.BaseQuantizeConfig", llm.quantization_config),
-                trust_remote_code=llm.__llm_trust_remote_code__,
-                use_safetensors=safe_serialization,
-                **hub_attrs,
-                **attrs,
-            ),
+        return autogptq.AutoGPTQForCausalLM.from_quantized(
+            llm._bentomodel.path,
+            *decls,
+            quantize_config=t.cast("autogptq.BaseQuantizeConfig", llm.quantization_config),
+            trust_remote_code=llm.__llm_trust_remote_code__,
+            use_safetensors=safe_serialization,
+            **hub_attrs,
+            **attrs,
         )
     model = infer_autoclass_from_llm_config(llm, config).from_pretrained(
         llm._bentomodel.path,
         *decls,
         config=config,
         trust_remote_code=llm.__llm_trust_remote_code__,
         **hub_attrs,
@@ -312,54 +296,22 @@
         or getattr(model, "is_quantized", False)
     )
     if torch.cuda.is_available() and torch.cuda.device_count() == 1 and not loaded_in_kbit:
         try:
             model = model.to("cuda")
         except torch.cuda.OutOfMemoryError as err:
             raise RuntimeError(
-                f"Failed to fit {llm.config['model_name']} with model_id '{llm.model_id}' to CUDA.\nNote: You can try out '--quantize int8' for dynamic quantization."
+                f"Failed to fit {llm.config['model_name']} with model_id '{llm.model_id}' to CUDA.\nNote: You can try out '--quantize int8 | int4' for dynamic quantization."
             ) from err
     if llm.bettertransformer and llm.__llm_implementation__ == "pt" and not isinstance(model, _transformers.Pipeline):
         # BetterTransformer is currently only supported on PyTorch.
         from optimum.bettertransformer import BetterTransformer
 
         model = BetterTransformer.transform(model)  # type: ignore
-    return t.cast("ModelProtocol[M]", model)
-
-
-def load_tokenizer(llm: openllm.LLM[t.Any, T]) -> TokenizerProtocol[T]:
-    """Load the tokenizer from BentoML store.
-
-    By default, it will try to find the bentomodel whether it is in store..
-    If model is not found, it will raises a ``bentoml.exceptions.NotFound``.
-    """
-    (_, _), tokenizer_attrs = llm.llm_parameters
-    bentomodel_fs = llm._bentomodel._fs
-    if bentomodel_fs.isfile(CUSTOM_OBJECTS_FILENAME):
-        with bentomodel_fs.open(CUSTOM_OBJECTS_FILENAME, "rb") as cofile:
-            try:
-                tokenizer = cloudpickle.load(t.cast("t.IO[bytes]", cofile))["tokenizer"]
-            except KeyError:
-                # This could happen if users implement their own import_model
-                raise OpenLLMException(
-                    "Model does not have tokenizer. Make sure to save \
-                    the tokenizer within the model via 'custom_objects'.\
-                    For example: bentoml.transformers.save_model(..., custom_objects={'tokenizer': tokenizer}))"
-                ) from None
-    else:
-        tokenizer = infer_tokenizers_class_for_llm(llm).from_pretrained(
-            bentomodel_fs.getsyspath("/"),
-            trust_remote_code=llm.__llm_trust_remote_code__,
-            **tokenizer_attrs,
-        )
-
-    if tokenizer.pad_token is None:
-        tokenizer.pad_token = tokenizer.eos_token
-
-    return tokenizer
+    return t.cast("M", model)
 
 
 def save_pretrained(
     llm: openllm.LLM[t.Any, t.Any],
     save_directory: str,
     is_main_process: bool = True,
     state_dict: DictStrAny | None = None,
```

### Comparing `openllm-0.2.5/src/openllm/utils/__init__.py` & `openllm-0.2.6/src/openllm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/utils/analytics.py` & `openllm-0.2.6/src/openllm/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/utils/codegen.py` & `openllm-0.2.6/src/openllm/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/utils/dantic.py` & `openllm-0.2.6/src/openllm/utils/dantic.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.2.6/src/openllm/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.2.6/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.2.6/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/utils/dummy_pt_and_triton_objects.py` & `openllm-0.2.6/src/openllm/utils/dummy_pt_and_triton_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.2.6/src/openllm/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.2.6/src/openllm/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/utils/dummy_vllm_objects.py` & `openllm-0.2.6/src/openllm/utils/dummy_vllm_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/utils/import_utils.py` & `openllm-0.2.6/src/openllm/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/utils/lazy.py` & `openllm-0.2.6/src/openllm/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm/utils/representation.py` & `openllm-0.2.6/src/openllm/utils/representation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm_client/__init__.py` & `openllm-0.2.6/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm_client/_prompt.py` & `openllm-0.2.6/src/openllm_client/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm_client/runtimes/__init__.py` & `openllm-0.2.6/src/openllm_client/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm_client/runtimes/base.py` & `openllm-0.2.6/src/openllm_client/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm_client/runtimes/grpc.py` & `openllm-0.2.6/src/openllm_client/runtimes/grpc.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/src/openllm_client/runtimes/http.py` & `openllm-0.2.6/src/openllm_client/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/__init__.py` & `openllm-0.2.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/client_test.py` & `openllm-0.2.6/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/configuration_test.py` & `openllm-0.2.6/tests/configuration_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/conftest.py` & `openllm-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/llm_test.py` & `openllm-0.2.6/tests/llm_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/models_test.py` & `openllm-0.2.6/tests/models_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/package_test.py` & `openllm-0.2.6/tests/package_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/strategies_test.py` & `openllm-0.2.6/tests/strategies_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/_strategies/__init__.py` & `openllm-0.2.6/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/_strategies/_configuration.py` & `openllm-0.2.6/tests/_strategies/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/models/conftest.py` & `openllm-0.2.6/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/models/flan_t5_test.py` & `openllm-0.2.6/tests/models/flan_t5_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/models/opt_test.py` & `openllm-0.2.6/tests/models/opt_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json` & `openllm-0.2.6/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json` & `openllm-0.2.6/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/models/__snapshots__/opt_test/test_opt_125m[container].json` & `openllm-0.2.6/tests/models/__snapshots__/opt_test/test_opt_125m[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/tests/models/__snapshots__/opt_test/test_opt_125m[local].json` & `openllm-0.2.6/tests/models/__snapshots__/opt_test/test_opt_125m[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/.gitignore` & `openllm-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/LICENSE.md` & `openllm-0.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/README.md` & `openllm-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/hatch.toml` & `openllm-0.2.6/hatch.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/pyproject.toml` & `openllm-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.5/PKG-INFO` & `openllm-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.2.5
+Version: 0.2.6
 Summary: OpenLLM: Operating LLMs in production
 Project-URL: Blog, https://modelserving.com
 Project-URL: Discord, https://l.bentoml.com/join-openllm-discord
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: GitHub, https://github.com/bentoml/openllm
 Project-URL: History, https://github.com/bentoml/openllm/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
```

