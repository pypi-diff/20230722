# Comparing `tmp/council_ai-0.0.6.tar.gz` & `tmp/council_ai-0.0.7.tar.gz`

## Comparing `council_ai-0.0.6.tar` & `council_ai-0.0.7.tar`

### file list

```diff
@@ -1,157 +1,157 @@
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.6/Makefile
--rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.6/engine_flow.png
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 council_ai-0.0.6/requirements.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/agent_tests/__init__.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/agent_tests/agent_tests.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/agents/__init__.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/agents/agent.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/agents/agent_chain.py
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/agents/agent_result.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/chains/__init__.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/chains/chain.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/contexts/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/contexts/cancellation_token.py
--rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/contexts/execution_context.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/contexts/messages.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/controllers/__init__.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/controllers/basic_controller.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/controllers/controller_base.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/controllers/execution_unit.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/controllers/llm_controller.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/evaluators/__init__.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/evaluators/basic_evaluator.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/evaluators/evaluator_base.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/evaluators/llm_evaluator.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/__init__.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/azure_llm.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/azure_llm_configuration.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/llm_base.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/llm_configuration_base.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/llm_exception.py
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/llm_message.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/openai_chat_completions_llm.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/openai_llm.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/openai_llm_configuration.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/mocks/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/prompt/__init__.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/prompt/prompt_builder.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/__init__.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/budget.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/errrors.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/if_runner.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/loop_runner_base.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/parallel.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/parallel_for.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/runner_base.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/runner_executor.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/sequential.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/skill_runner_base.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/types.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/scorers/__init__.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/scorers/llm_similarity_scorer.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/scorers/scorer_base.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/scorers/scorer_exception.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/__init__.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/llm_skill.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/skill_base.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/__init__.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_news_skill.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_search_skill.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_context/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_context/context_provider.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_context/google_news.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_context/google_search.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_context/schemas.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/utils/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/utils/env.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/utils/option.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/utils/result.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/.gitignore
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/.readthedocs.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/Makefile
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/README.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/docker-compose.yaml
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/dockerfile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/make.bat
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/requirements.txt
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/conf.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/index.rst
--rw-r--r--   0        0        0    17142 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/_static/00_chainml_logo.png
--rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/_static/02_chainml_logo_black.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/contributing/contributing.md
--rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/getting_started/first_example.ipynb
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/getting_started/installation.md
--rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/introduction/engine_flow.png
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/introduction/key_concepts.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/introduction/key_features.md
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/introduction/welcome.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/agents.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/chains.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/controllers.rst
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/evaluators.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm.rst
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/scorers.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/skills.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/utils.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/agents/agent.rst
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/agents/agent_result.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/chains/chain.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/agent_context.rst
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/agent_message.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/chain_context.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/chain_history.rst
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/chat_history.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/chat_message_base.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/chat_message_kind.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/iteration_context.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/scored_agent_message.rst
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/skill_context.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/skill_error_message.rst
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/skill_message.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/skill_success_message.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/user_message.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/controllers/basic_controller.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/controllers/controller_base.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/controllers/llm_controller.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/evaluators/basic_evaluator.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/evaluators/evaluator_base.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/evaluators/llm_evaluator.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/azure_llm.rst
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/azure_llm_configuration.rst
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/llm_base.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/llm_configuration_base.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/llm_message.rst
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/llm_message_role.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/openai_llm.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/openai_llm_configuration.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/budget.rst
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/errors.rst
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/if.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/loop_runner_base.rst
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/parallel.rst
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/parallel_for.rst
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/runner_base.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/runner_executor.rst
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/sequential.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/skill_runner_base.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/scorers/llm_similarity_scorer.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/scorers/scorer_base.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/scorers/scorer_exception.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/skills/google.rst
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/skills/llm_skill.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/skills/skill_base.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/skills/google/google_news_skill.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/skills/google/google_search_skill.rst
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/utils/option.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/utils/option_exception.rst
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/use_cases/langchain_llm_integration.ipynb
--rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/use_cases/multi_chain_agent.ipynb
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 council_ai-0.0.6/stubs/GoogleNews.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 council_ai-0.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 council_ai-0.0.6/LICENSE
--rw-r--r--   0        0        0     9277 2020-02-02 00:00:00.000000 council_ai-0.0.6/README.md
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 council_ai-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 council_ai-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.7/Makefile
+-rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.7/engine_flow.png
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 council_ai-0.0.7/env.example
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 council_ai-0.0.7/requirements.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/agent_tests/__init__.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/agent_tests/agent_tests.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/agents/__init__.py
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/agents/agent.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/agents/agent_chain.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/agents/agent_result.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/chains/__init__.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/chains/chain.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/contexts/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/contexts/cancellation_token.py
+-rw-r--r--   0        0        0    12196 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/contexts/execution_context.py
+-rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/contexts/messages.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/controllers/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/controllers/basic_controller.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/controllers/controller_base.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/controllers/execution_unit.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/controllers/llm_controller.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/evaluators/__init__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/evaluators/basic_evaluator.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/evaluators/evaluator_base.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/evaluators/llm_evaluator.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/__init__.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/azure_llm.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/azure_llm_configuration.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/llm_base.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/llm_configuration_base.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/llm_exception.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/llm_message.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/openai_chat_completions_llm.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/openai_llm.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/openai_llm_configuration.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/mocks/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/prompt/__init__.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/prompt/prompt_builder.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/__init__.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/budget.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/errrors.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/if_runner.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/loop_runner_base.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/parallel.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/parallel_for.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/runner_base.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/runner_context.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/runner_executor.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/sequential.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/skill_runner_base.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/types.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/scorers/__init__.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/scorers/llm_similarity_scorer.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/scorers/scorer_base.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/scorers/scorer_exception.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/__init__.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/llm_skill.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/skill_base.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/__init__.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_news_skill.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_search_skill.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_context/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_context/context_provider.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_context/google_news.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_context/google_search.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_context/schemas.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/utils/__init__.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/utils/env.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/utils/option.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/utils/parameter.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/utils/result.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/.gitignore
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/.readthedocs.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/Makefile
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/README.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/docker-compose.yaml
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/dockerfile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/make.bat
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/requirements.txt
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/conf.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/index.rst
+-rw-r--r--   0        0        0    17142 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/_static/00_chainml_logo.png
+-rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/_static/02_chainml_logo_black.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/contributing/contributing.md
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/getting_started/first_example.ipynb
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/getting_started/installation.md
+-rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/introduction/engine_flow.png
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/introduction/key_concepts.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/introduction/key_features.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/introduction/welcome.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/agents.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/chains.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/controllers.rst
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/evaluators.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm.rst
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/scorers.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/skills.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/utils.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/agents/agent.rst
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/agents/agent_result.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/chains/chain.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/agent_context.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/chain_context.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/chain_history.rst
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/chat_history.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/chat_message.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/chat_message_kind.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/iteration_context.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/message_collection.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/scored_chat_message.rst
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/skill_context.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/controllers/basic_controller.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/controllers/controller_base.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/controllers/execution_unit.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/controllers/llm_controller.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/evaluators/basic_evaluator.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/evaluators/evaluator_base.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/evaluators/llm_evaluator.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/azure_llm.rst
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/azure_llm_configuration.rst
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/llm_base.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/llm_configuration_base.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/llm_message.rst
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/llm_message_role.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/openai_llm.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/openai_llm_configuration.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/budget.rst
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/errors.rst
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/if.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/loop_runner_base.rst
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/parallel.rst
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/parallel_for.rst
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/runner_base.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/runner_executor.rst
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/sequential.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/skill_runner_base.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/scorers/llm_similarity_scorer.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/scorers/scorer_base.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/scorers/scorer_exception.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/skills/google.rst
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/skills/llm_skill.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/skills/skill_base.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/skills/google/google_news_skill.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/skills/google/google_search_skill.rst
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/utils/option.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/utils/option_exception.rst
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/use_cases/langchain_llm_integration.ipynb
+-rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/use_cases/multi_chain_agent.ipynb
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 council_ai-0.0.7/stubs/GoogleNews.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 council_ai-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 council_ai-0.0.7/LICENSE
+-rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 council_ai-0.0.7/README.md
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 council_ai-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 council_ai-0.0.7/PKG-INFO
```

### Comparing `council_ai-0.0.6/engine_flow.png` & `council_ai-0.0.7/engine_flow.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/council/agent_tests/agent_tests.py` & `council_ai-0.0.7/council/agent_tests/agent_tests.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/council/agents/agent.py` & `council_ai-0.0.7/council/agents/agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
-from typing import List
+from typing import List, Optional
 
 from council.chains import Chain
 from council.contexts import AgentContext, ChatHistory
 from council.controllers import ControllerBase, BasicController
 from council.evaluators import BasicEvaluator, EvaluatorBase
 from council.runners import Budget, new_runner_executor
 from council.skills import SkillBase
 from .agent_result import AgentResult
+from ..runners.budget import InfiniteBudget
 
 logger = logging.getLogger(__name__)
 
 
 class Agent:
     """
     Represents an agent that executes a set of chains to interact with the environment.
@@ -35,45 +36,48 @@
             chains (List[Chain]): The list of chains that the agent executes.
             evaluator (EvaluatorBase): The evaluator responsible for evaluating the agent's performance.
         """
         self.controller = controller
         self.chains = chains
         self.evaluator = evaluator
 
-    def execute(self, context: AgentContext, budget: Budget = Budget.default()) -> AgentResult:
+    def execute(self, context: AgentContext, budget: Optional[Budget] = None) -> AgentResult:
         """
         Executes the agent's chains based on the provided context and budget.
 
         Args:
             context (AgentContext): The context for executing the chains.
-            budget (Budget): The budget for agent execution.
+            budget (Optional[Budget]): The budget for agent execution. Defaults to :meth:`Budget.default` if `None`
 
         Returns:
             AgentResult:
 
         Raises:
             None
         """
         executor = new_runner_executor("agent")
+        budget = budget or Budget.default()
         try:
             logger.info('message="agent execution started"')
             while not budget.is_expired():
                 logger.info(f'message="agent iteration started" iteration="{len(context.evaluationHistory)+1}"')
                 plan = self.controller.get_plan(context=context, chains=self.chains, budget=budget)
                 logger.debug(f'message="agent controller returned {len(plan)} execution plan(s)"')
 
                 if len(plan) == 0:
                     return AgentResult()
                 for unit in plan:
                     chain = unit.chain
                     budget = unit.budget
-                    logger.info(f'message="chain execution started" chain="{chain.name}"')
-                    chain_context = context.new_chain_context(chain.name)
+                    logger.info(f'message="chain execution started" chain="{chain.name}" execution_unit="{unit.name}"')
+                    chain_context = context.new_chain_context(unit.name)
+                    if unit.initial_state is not None:
+                        chain_context.current.append(unit.initial_state)
                     chain.execute(chain_context, budget)
-                    logger.info(f'message="chain execution ended" chain="{chain.name}"')
+                    logger.info(f'message="chain execution ended" chain="{chain.name}" execution_unit="{unit.name}"')
 
                 result = self.evaluator.execute(context, budget)
                 context.evaluationHistory.append(result)
 
                 result = self.controller.select_responses(context)
                 logger.debug("controller selected %d responses", len(result))
                 if len(result) > 0:
@@ -81,31 +85,32 @@
 
             return AgentResult()
         finally:
             logger.info('message="agent execution ended"')
             executor.shutdown(wait=False, cancel_futures=True)
 
     @staticmethod
-    def from_skill(skill: SkillBase) -> "Agent":
+    def from_skill(skill: SkillBase, chain_description: Optional[str] = None) -> "Agent":
         """
         Helper function to create a new agent with a  :class:`.BasicController`, a
             :class:`.BasicEvaluator` and a single :class:`.SkillBase` wrapped into a :class:`.Chain`
 
         Parameters:
              skill(SkillBase): a skill
+             chain_description(str): Optional, chain description
         Returns:
             Agent: a new instance
         """
-        chain = Chain(name="BasicChain", description="basic chain", runners=[skill])
+        chain = Chain(name="BasicChain", description=chain_description or "basic chain", runners=[skill])
         return Agent(controller=BasicController(), chains=[chain], evaluator=BasicEvaluator())
 
     def execute_from_user_message(self, message: str) -> AgentResult:
         """
         Helper function that executes an agent with a simple user message.
 
         Parameters:
             message(str): the user message
         Returns:
              AgentResult:
         """
         context = AgentContext(ChatHistory.from_user_message(message))
-        return self.execute(context)
+        return self.execute(context, budget=InfiniteBudget())
```

### Comparing `council_ai-0.0.6/council/agents/agent_chain.py` & `council_ai-0.0.7/council/agents/agent_chain.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Optional, Any
 
 from .agent import Agent
 from council.chains import Chain
-from council.contexts import AgentContext, ChainContext, SkillSuccessMessage
+from council.contexts import AgentContext, ChainContext, ChatMessage
 from council.runners import Budget, RunnerExecutor
 
 
 class AgentChain(Chain):
     def __init__(self, name: str, description: str, agent: Agent):
         super().__init__(name, description, [])
         self.agent = agent
 
     def execute(
         self,
         context: ChainContext,
         budget: Budget,
         executor: Optional[RunnerExecutor] = None,
     ) -> Any:
-        agent_context = AgentContext(context.chatHistory)
+        agent_context = AgentContext(context.chat_history)
         result = self.agent.execute(agent_context, budget)
         maybe_message = result.try_best_message
         if maybe_message.is_some():
             message = maybe_message.unwrap()
-            context.current.messages.append(SkillSuccessMessage(self.name, message.message, message.data))
+            context.current.append(ChatMessage.skill(message.message, message.data, message.source, message.is_error))
```

### Comparing `council_ai-0.0.6/council/agents/agent_result.py` & `council_ai-0.0.7/council/agents/agent_result.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 from collections.abc import Sequence
 from typing import List, Optional
 
-from council.contexts import ScoredAgentMessage, AgentMessage
+from council.contexts import ScoredChatMessage, ChatMessage
 from council.utils import Option
 
 
 class AgentResult:
     """
     Represent the execution result of an :class:`Agent`
     """
 
-    _messages: List[ScoredAgentMessage]
+    _messages: List[ScoredChatMessage]
 
-    def __init__(self, messages: Optional[List[ScoredAgentMessage]] = None):
+    def __init__(self, messages: Optional[List[ScoredChatMessage]] = None):
         """
         Initialize a new instance.
 
         Parameters:
-            messages(Optional[List[ScoredAgentMessage]]): an optional list of messages
+            messages(Optional[List[ScoredChatMessage]]): an optional list of messages
         """
         self._messages = messages if messages is not None else []
 
     @property
-    def messages(self) -> Sequence[ScoredAgentMessage]:
+    def messages(self) -> Sequence[ScoredChatMessage]:
         """
         An unordered list of messages, with their scores.
 
         Returns:
-            Sequence[ScoredAgentMessage]:
+            Sequence[ScoredChatMessage]:
         """
         return self._messages
 
     @property
-    def best_message(self) -> AgentMessage:
+    def best_message(self) -> ChatMessage:
         """
         The message with the highest score. If multiple messages have the highest score, the first one is returned.
 
         Returns:
-            AgentMessage:
+            ChatMessage:
 
         Raises:
             ValueError: there is no messages
         """
         return max(self._messages, key=lambda item: item.score).message
 
     @property
-    def try_best_message(self) -> Option[AgentMessage]:
+    def try_best_message(self) -> Option[ChatMessage]:
         """
         The message with the highest score, if any. See :meth:`best_message` for more details
 
         Returns:
-            Option[AgentMessage]: the message with the highest score, wrapped into :meth:`.Option.some`, if some,
+            Option[ChatMessage]: the message with the highest score, wrapped into :meth:`.Option.some`, if some,
                 :meth:`.Option.none` otherwise
         """
         if len(self._messages) == 0:
             return Option.none()
         return Option.some(self.best_message)
```

### Comparing `council_ai-0.0.6/council/chains/chain.py` & `council_ai-0.0.7/council/chains/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,14 @@
 
         Raises:
             None
         """
         executor = (
             RunnerExecutor(max_workers=10, thread_name_prefix=f"chain_{self.name}") if executor is None else executor
         )
-        self.runner.run(context, budget, executor)
+        self.runner.run_from_chain_context(context, budget, executor)
 
     def __repr__(self):
         return f"Chain({self.name}, {self.description})"
 
     def __str__(self):
         return f"Chain {self.name}, description: {self.description}"
```

### Comparing `council_ai-0.0.6/council/controllers/basic_controller.py` & `council_ai-0.0.7/council/controllers/basic_controller.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import List
 
 from council.chains import Chain
-from council.contexts import AgentContext, ScoredAgentMessage
+from council.contexts import AgentContext, ScoredChatMessage
 from council.runners import Budget
 
 from .controller_base import ControllerBase
 from .execution_unit import ExecutionUnit
 
 
 class BasicController(ControllerBase):
     """a basic controller that requests all chains to be executed and returns all results"""
 
     def get_plan(self, context: AgentContext, chains: List[Chain], budget: Budget) -> List[ExecutionUnit]:
         return [ExecutionUnit(chain, budget) for chain in chains]
 
-    def select_responses(self, context: AgentContext) -> List[ScoredAgentMessage]:
+    def select_responses(self, context: AgentContext) -> List[ScoredChatMessage]:
         return context.evaluationHistory[-1]
```

### Comparing `council_ai-0.0.6/council/controllers/controller_base.py` & `council_ai-0.0.7/council/controllers/controller_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import List
 
 from council.chains import Chain
-from council.contexts import AgentContext, ScoredAgentMessage
+from council.contexts import AgentContext, ScoredChatMessage
 from council.runners import Budget
 from .execution_unit import ExecutionUnit
 
 
 class ControllerBase(ABC):
     """
     Abstract base class for an agent controller.
@@ -30,21 +30,21 @@
 
         Raises:
             None
         """
         pass
 
     @abstractmethod
-    def select_responses(self, context: AgentContext) -> List[ScoredAgentMessage]:
+    def select_responses(self, context: AgentContext) -> List[ScoredChatMessage]:
         """
         Selects responses from the agent's context.
 
         Args:
             context (AgentContext): The context for selecting responses.
 
         Returns:
-            List[ScoredAgentMessage]: A list of scored agent messages representing the selected responses.
+            List[ScoredChatMessage]: A list of scored agent messages representing the selected responses.
 
         Raises:
             None
         """
         pass
```

### Comparing `council_ai-0.0.6/council/controllers/llm_controller.py` & `council_ai-0.0.7/council/controllers/llm_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import List, Tuple
 
-from council.contexts import AgentContext, ScoredAgentMessage
+from council.contexts import AgentContext, ScoredChatMessage
 from council.chains import Chain
 from council.llm import LLMMessage, LLMBase
 from council.utils import Option
 from council.runners import Budget
 
 from .controller_base import ControllerBase
 from .execution_unit import ExecutionUnit
@@ -29,15 +29,15 @@
             response_threshold (float): a minimum threshold to select a response from its score
             top_k_execution_plan (int): maximum number of execution plan returned
         """
         self._llm = llm
         self._response_threshold = response_threshold
         self._top_k = top_k_execution_plan
 
-    def select_responses(self, context: AgentContext) -> List[ScoredAgentMessage]:
+    def select_responses(self, context: AgentContext) -> List[ScoredChatMessage]:
         return context.evaluationHistory[-1]
 
     def get_plan(self, context: AgentContext, chains: List[Chain], budget: Budget) -> List[ExecutionUnit]:
         answer_choices = "\n ".join([f"name: {c.name}, description: {c.description}" for c in chains])
         task_description = [
             "You are an assistant responsible to identify the intent of the user. ",
             "Categories are given as a name and a category (name: {name}, description: {description})",
@@ -47,19 +47,19 @@
             "# Each response is provided on a new line",
             "# When no category is relevant, you will answer exactly with 'unknown'",
         ]
 
         messages = [
             LLMMessage.system_message("\n".join(task_description)),
             LLMMessage.user_message(
-                f"what are most relevant categories for: {context.chatHistory.last_user_message().unwrap().message}"
+                f"what are most relevant categories for: {context.chatHistory.try_last_user_message.unwrap().message}"
             ),
         ]
 
-        response = self._llm.post_chat_request(messages)
+        response = self._llm.post_chat_request(messages)[0]
         logger.debug(f"llm response: {response}")
 
         parsed = [self.parse_line(line, chains) for line in response.splitlines()]
         filtered = [r.unwrap() for r in parsed if r.is_some() and r.unwrap()[1] > self._response_threshold]
         if (filtered is None) or (len(filtered) == 0):
             return []
```

### Comparing `council_ai-0.0.6/council/evaluators/basic_evaluator.py` & `council_ai-0.0.7/council/evaluators/basic_evaluator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 from typing import List
 
-from council.contexts import AgentContext, ScoredAgentMessage, SkillSuccessMessage, AgentMessage
+from council.contexts import (
+    AgentContext,
+    ScoredChatMessage,
+    ChatMessage,
+)
 from council.runners.budget import Budget
 from .evaluator_base import EvaluatorBase
 
 
 class BasicEvaluator(EvaluatorBase):
-    def execute(self, context: AgentContext, budget: Budget) -> List[ScoredAgentMessage]:
+    def execute(self, context: AgentContext, budget: Budget) -> List[ScoredChatMessage]:
         result = []
         for chain_history in context.chainHistory.values():
             chain_result = chain_history[-1].messages[-1]
-            score = 1 if isinstance(chain_result, SkillSuccessMessage) else 0
-            result.append(ScoredAgentMessage(AgentMessage(chain_result.message, chain_result.data), score))
+            score = 1 if chain_result.is_kind_skill and chain_result.is_ok else 0
+            result.append(
+                ScoredChatMessage(
+                    ChatMessage.agent(chain_result.message, chain_result.data, is_error=chain_result.is_error),
+                    score,
+                )
+            )
         return result
```

### Comparing `council_ai-0.0.6/council/evaluators/evaluator_base.py` & `council_ai-0.0.7/council/evaluators/evaluator_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from abc import ABC, abstractmethod
 from typing import List
 
-from council.contexts import AgentContext, ScoredAgentMessage
+from council.contexts import AgentContext, ScoredChatMessage
 from council.runners import Budget
 
 
 class EvaluatorBase(ABC):
     """
     Abstract base class for an agent evaluator.
 
     """
 
     @abstractmethod
-    def execute(self, context: AgentContext, budget: Budget) -> List[ScoredAgentMessage]:
+    def execute(self, context: AgentContext, budget: Budget) -> List[ScoredChatMessage]:
         """
         Executes the evaluator on the agent's context within the given budget.
 
         Args:
             context (AgentContext): The context for executing the evaluator.
             budget (Budget): The budget for evaluator execution.
 
         Returns:
-            List[ScoredAgentMessage]: A list of scored agent messages resulting from the evaluation.
+            List[ScoredChatMessage]: A list of scored agent messages resulting from the evaluation.
 
         Raises:
             None
         """
         pass
```

### Comparing `council_ai-0.0.6/council/evaluators/llm_evaluator.py` & `council_ai-0.0.7/council/evaluators/llm_evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 LLMEvaluator implementation.
 
 This evaluator uses the given `LLM` to evaluate the chain's responses.
 """
 import logging
 from typing import List
 
-from council.contexts import AgentContext, ScoredAgentMessage, AgentMessage, SkillMessage, UserMessage
+from council.contexts import AgentContext, ScoredChatMessage, ChatMessage
 from council.evaluators import EvaluatorBase
 from council.llm import LLMBase, LLMMessage
 from council.runners import Budget
 from council.utils import Option
 
 
 class LLMEvaluator(EvaluatorBase):
@@ -22,47 +22,47 @@
 
         :param llm: model to use for the evaluation.
         """
         """Build a new LLMEvaluator."""
         super().__init__()
         self.llm = llm
 
-    def execute(self, context: AgentContext, budget: Budget) -> List[ScoredAgentMessage]:
-        query = context.chatHistory.last_user_message().unwrap()
+    def execute(self, context: AgentContext, budget: Budget) -> List[ScoredChatMessage]:
+        query = context.chatHistory.try_last_user_message.unwrap()
         chain_results = [
-            chain_history[-1].last_message().unwrap()
+            chain_history[-1].try_last_message.unwrap()
             for chain_history in context.chainHistory.values()
-            if chain_history[-1].last_message().is_some()
+            if chain_history[-1].try_last_message.is_some()
         ]
         scored_messages = self.__score_responses(query=query, skill_messages=chain_results)
         return list(scored_messages)
 
-    def __score_responses(self, query: UserMessage, skill_messages: list[SkillMessage]) -> List[ScoredAgentMessage]:
+    def __score_responses(self, query: ChatMessage, skill_messages: list[ChatMessage]) -> List[ScoredChatMessage]:
         """
         Score agent response.
 
         :param query: Query used to build the responses.
         :param skill_messages: Responses generated by the chain.
         :return: list of scored messages.
         """
         # Build prompt to send to the inner LLM
         responses = [skill_message.message for skill_message in skill_messages]
         prompt = self.__build_prompt(query.message, responses=responses)
 
         # Send prompt to inner LLM
         messages = [LLMMessage.system_message(prompt)]
-        llm_response = self.llm.post_chat_request(messages=messages)
+        llm_response = self.llm.post_chat_request(messages=messages)[0]
 
         # Parse LLM response with the score for each message we want to score
         scores = [self.__parse_eval(line) for line in llm_response.split("\n")]
 
         agent_messages = []
         for skill_message, score in filter(lambda tuple: tuple[1].is_some(), zip(skill_messages, scores)):
-            agent_message = ScoredAgentMessage(
-                AgentMessage(message=skill_message.message, data=skill_message.data), score.unwrap()
+            agent_message = ScoredChatMessage(
+                ChatMessage.agent(message=skill_message.message, data=skill_message.data), score.unwrap()
             )
             agent_messages.append(agent_message)
 
         return agent_messages
 
     @staticmethod
     def __parse_eval(line: str) -> Option[int]:
```

### Comparing `council_ai-0.0.6/council/llm/azure_llm.py` & `council_ai-0.0.7/council/llm/azure_llm.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/council/llm/azure_llm_configuration.py` & `council_ai-0.0.7/council/llm/azure_llm_configuration.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/council/llm/llm_base.py` & `council_ai-0.0.7/council/llm/llm_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class LLMBase(abc.ABC):
     """
     Abstract base class representing a language model.
     """
 
-    def post_chat_request(self, messages: List[LLMMessage], **kwargs: Any) -> str:
+    def post_chat_request(self, messages: List[LLMMessage], **kwargs: Any) -> List[str]:
         """
         Sends a chat request to the language model.
 
         Parameters:
             messages (List[LLMMessage]): A list of LLMMessage objects representing the chat messages.
             **kwargs: Additional keyword arguments for the chat request.
 
@@ -33,9 +33,9 @@
         except Exception as e:
             logger.exception('message="failed execution of llm request"')
             raise e
         finally:
             logger.debug('message="done execution of llm request"')
 
     @abc.abstractmethod
-    def _post_chat_request(self, messages: List[LLMMessage], **kwargs: Any) -> str:
+    def _post_chat_request(self, messages: List[LLMMessage], **kwargs: Any) -> List[str]:
         pass
```

### Comparing `council_ai-0.0.6/council/llm/llm_message.py` & `council_ai-0.0.7/council/llm/llm_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
-from typing import Optional, List
+from typing import Optional, List, Iterable
 
-from council.contexts import ChatMessageBase, ChatMessageKind
+from council.contexts import ChatMessage, ChatMessageKind
 
 
 class LLMMessageRole(str, Enum):
     """
     Enum representing the roles of messages in a conversation or dialogue.
     """
 
@@ -69,15 +69,15 @@
 
         Parameters:
             content (str): the message content
         """
         return LLMMessage(role=LLMMessageRole.Assistant, content=content)
 
     def dict(self) -> dict[str, str]:
-        return {"role": self._role, "content": self._content}
+        return {"role": self._role.value, "content": self._content}
 
     @property
     def content(self) -> str:
         """Retrieve the content of this instance"""
         return self._content
 
     @property
@@ -86,19 +86,19 @@
         return self._role
 
     def is_of_role(self, role: LLMMessageRole) -> bool:
         """Check the role of this instance"""
         return self._role == role
 
     @staticmethod
-    def from_chat_message(chat_message: ChatMessageBase) -> Optional["LLMMessage"]:
-        """Convert :class:`~.ChatMessageBase` into :class:`.LLMMessage`"""
+    def from_chat_message(chat_message: ChatMessage) -> Optional["LLMMessage"]:
+        """Convert :class:`~.ChatMessage` into :class:`.LLMMessage`"""
         if chat_message.kind == ChatMessageKind.User:
             return LLMMessage.user_message(chat_message.message)
         elif chat_message.kind == ChatMessageKind.Agent:
             return LLMMessage.assistant_message(chat_message.message)
         return None
 
     @staticmethod
-    def from_chat_messages(messages: List[ChatMessageBase]) -> List["LLMMessage"]:
+    def from_chat_messages(messages: Iterable[ChatMessage]) -> List["LLMMessage"]:
         m = map(LLMMessage.from_chat_message, messages)
         return [msg for msg in m if msg is not None]
```

### Comparing `council_ai-0.0.6/council/llm/openai_llm.py` & `council_ai-0.0.7/council/llm/openai_llm.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/council/llm/openai_llm_configuration.py` & `council_ai-0.0.7/council/llm/openai_llm_configuration.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/council/mocks/__init__.py` & `council_ai-0.0.7/council/mocks/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 import time
 import random
 from typing import List, Any, Callable, Optional, Protocol
 
 from council.agents import Agent, AgentResult
-from council.contexts import AgentContext, ScoredAgentMessage, AgentMessage, SkillContext, SkillMessage
+from council.contexts import AgentContext, ScoredChatMessage, SkillContext, ChatMessage
 from council.llm import LLMBase, LLMMessage
 from council.runners import Budget
 from council.scorers import ScorerBase
 from council.skills import SkillBase
 
 
 class LLMMessagesToStr(Protocol):
-    def __call__(self, messages: List[LLMMessage]) -> str:
+    def __call__(self, messages: List[LLMMessage]) -> List[str]:
         ...
 
 
-def llm_message_content_to_str(messages: List[LLMMessage]) -> str:
-    return "\n".join([msg.content for msg in messages])
+def llm_message_content_to_str(messages: List[LLMMessage]) -> List[str]:
+    return [msg.content for msg in messages]
 
 
 class MockSkill(SkillBase):
-    def __init__(self, name: str = "mock", action: Optional[Callable[[SkillContext, Budget], SkillMessage]] = None):
+    def __init__(self, name: str = "mock", action: Optional[Callable[[SkillContext, Budget], ChatMessage]] = None):
         super().__init__(name)
         self._action = action if action is not None else self.empty_message
 
-    def execute(self, context: SkillContext, budget: Budget) -> SkillMessage:
+    def execute(self, context: SkillContext, budget: Budget) -> ChatMessage:
         return self._action(context, budget)
 
     def empty_message(self, context: SkillContext, budget: Budget):
         return self.build_success_message("")
 
     def set_action_custom_message(self, message: str) -> None:
         self._action = lambda context, budget: self.build_success_message(message)
 
 
 class MockLLM(LLMBase):
     def __init__(self, action: Optional[LLMMessagesToStr] = None):
         self._action = action
 
-    def _post_chat_request(self, messages: List[LLMMessage], **kwargs: Any) -> str:
+    def _post_chat_request(self, messages: List[LLMMessage], **kwargs: Any) -> List[str]:
         if self._action is not None:
             return self._action(messages)
-        return f"{self.__class__.__name__}"
+        return [f"{self.__class__.__name__}"]
 
     @staticmethod
     def from_responses(responses: List[str]) -> "MockLLM":
-        value = "\n".join([r for r in responses])
-        return MockLLM(action=(lambda x: value))
+        return MockLLM(action=(lambda x: responses))
 
     @staticmethod
     def from_response(response: str) -> "MockLLM":
-        return MockLLM(action=(lambda x: response))
+        return MockLLM(action=(lambda x: [response]))
+
+    @staticmethod
+    def from_multi_line_response(responses: List[str]) -> "MockLLM":
+        response = "\n".join(responses)
+        return MockLLM(action=(lambda x: [response]))
 
 
 class MockErrorSimilarityScorer(ScorerBase):
     def __init__(self, exception: Exception = Exception()):
         self.exception = exception
 
-    def _score(self, message: AgentMessage) -> float:
+    def _score(self, message: ChatMessage) -> float:
         raise self.exception
 
 
 class MockAgent(Agent):
     # noinspection PyMissingConstructor
     def __init__(
         self,
@@ -73,19 +77,19 @@
     ):
         self.message = message
         self.data = data
         self.score = score
         self.sleep = sleep
         self.sleep_interval = sleep_interval
 
-    def execute(self, context: AgentContext, budget: Budget = Budget.default()) -> AgentResult:
+    def execute(self, context: AgentContext, budget: Optional[Budget] = None) -> AgentResult:
         time.sleep(random.uniform(self.sleep, self.sleep + self.sleep_interval))
-        return AgentResult([ScoredAgentMessage(AgentMessage(self.message, self.data), score=self.score)])
+        return AgentResult([ScoredChatMessage(ChatMessage.agent(self.message, self.data), score=self.score)])
 
 
 class MockErrorAgent(Agent):
     # noinspection PyMissingConstructor
     def __init__(self, exception: Exception = Exception()):
         self.exception = exception
 
-    def execute(self, context: AgentContext, budget: Budget = Budget.default()) -> AgentResult:
+    def execute(self, context: AgentContext, budget: Optional[Budget] = None) -> AgentResult:
         raise self.exception
```

### Comparing `council_ai-0.0.6/council/prompt/prompt_builder.py` & `council_ai-0.0.7/council/prompt/prompt_builder.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Any, List, Optional
 
 from jinja2 import Template
 
-from council.contexts import ChainContext, ChatMessageKind
+from council.contexts import SkillContext, ChatMessageKind
 
 logger = logging.getLogger(__name__)
 
 
 class PromptBuilder:
     """
     A class for building prompts using a Jinja2 template and optional instructions.
@@ -38,20 +38,20 @@
         self._template = Template(t)
         if instructions is not None and len(instructions) > 0:
             self._instructions = "\n# Instructions: "
             self._instructions += "\n".join(instructions)
         else:
             self._instructions = ""
 
-    def apply(self, context: ChainContext) -> str:
+    def apply(self, context: SkillContext) -> str:
         """
         Builds and returns the prompt by rendering the template and appending instructions.
 
         Args:
-            context (ChainContext): The context object containing the necessary data for rendering the template.
+            context (SkillContext): The context object containing the necessary data for rendering the template.
 
         Returns:
             str: The generated prompt string.
 
         """
 
         template_context = {
@@ -60,42 +60,42 @@
         }
 
         prompt = self._template.render(template_context)
         prompt += self._instructions
         return prompt
 
     @staticmethod
-    def __build_chat_history(context: ChainContext) -> dict[str, Any]:
-        last_message = context.chatHistory.last_message()
-        last_user_message = context.chatHistory.last_user_message()
-        last_agent_message = context.chatHistory.last_agent_message()
+    def __build_chat_history(context: SkillContext) -> dict[str, Any]:
+        last_message = context.chat_history.try_last_message
+        last_user_message = context.chat_history.try_last_user_message
+        last_agent_message = context.chat_history.try_last_agent_message
 
         return {
             "agent": {
                 "messages": [
-                    msg.message for msg in context.chatHistory.messages if msg.is_of_kind(ChatMessageKind.Agent)
+                    msg.message for msg in context.chat_history.messages if msg.is_of_kind(ChatMessageKind.Agent)
                 ],
                 "last_message": last_agent_message.map_or(lambda m: m.message, ""),
             },
             "user": {
                 "messages": [
-                    msg.message for msg in context.chatHistory.messages if msg.is_of_kind(ChatMessageKind.User)
+                    msg.message for msg in context.chat_history.messages if msg.is_of_kind(ChatMessageKind.User)
                 ],
                 "last_message": last_user_message.map_or(lambda m: m.message, ""),
             },
-            "messages": [msg.message for msg in context.chatHistory.messages],
+            "messages": [msg.message for msg in context.chat_history.messages],
             "last_message": last_message.map_or(lambda m: m.message, ""),
         }
 
     @staticmethod
-    def __build_chain_history(context: ChainContext) -> dict[str, Any]:
-        if len(context.chainHistory) == 0:
+    def __build_chain_history(context: SkillContext) -> dict[str, Any]:
+        if len(context.chain_histories) == 0:
             return {
                 "messages": [],
                 "last_message": "",
             }
 
-        last_message = context.current.last_message()
+        last_message = context.current.try_last_message
         return {
             "messages": [msg.message for msg in context.current.messages],
             "last_message": last_message.map_or(lambda m: m.message, ""),
         }
```

### Comparing `council_ai-0.0.6/council/runners/__init__.py` & `council_ai-0.0.7/council/runners/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .errrors import RunnerError, RunnerTimeoutError, RunnerSkillError, RunnerPredicateError, RunnerGeneratorError
+from .runner_context import RunnerContext
 from .budget import Budget
 from .types import RunnerPredicate, RunnerGenerator
 from .runner_executor import RunnerExecutor, new_runner_executor
 from .runner_base import RunnerBase
 from .skill_runner_base import SkillRunnerBase
 from .sequential import Sequential
 from .parallel import Parallel
```

### Comparing `council_ai-0.0.6/council/runners/budget.py` & `council_ai-0.0.7/council/runners/budget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 import time
 
+from council.utils import read_env_int
+
 
 class BudgetExpiredException(Exception):
     pass
 
 
 class Budget:
     """
@@ -49,15 +51,16 @@
     def default() -> "Budget":
         """
         Helper function that create a new Budget with a default value.
 
         Returns:
             Budget
         """
-        return Budget(duration=30)
+        duration = read_env_int("COUNCIL_DEFAULT_BUDGET", required=False, default=30)
+        return Budget(duration=duration.unwrap())
 
 
 class InfiniteBudget(Budget):
     def __init__(self):
         super().__init__(10000)
 
     def remaining(self) -> Budget:
```

### Comparing `council_ai-0.0.6/council/runners/errrors.py` & `council_ai-0.0.7/council/runners/errrors.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/council/runners/if_runner.py` & `council_ai-0.0.7/council/runners/if_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from council.contexts import ChainContext, SkillErrorMessage
+from council.contexts import ChatMessage
 
-from .budget import Budget
+from .runner_context import RunnerContext
 from .errrors import RunnerPredicateError
 from .runner_base import RunnerBase
 from .runner_executor import RunnerExecutor
 from .types import RunnerPredicate
 
 
 class If(RunnerBase):
@@ -14,18 +14,17 @@
 
     def __init__(self, predicate: RunnerPredicate, runner: RunnerBase):
         self.predicate = predicate
         self.runner = runner
 
     def _run(
         self,
-        context: ChainContext,
-        budget: Budget,
+        context: RunnerContext,
         executor: RunnerExecutor,
     ) -> None:
         try:
-            result = self.predicate(context, budget)
+            result = self.predicate(context.make_chain_context(), context.budget.remaining())
         except Exception as e:
-            context.current.messages.append(SkillErrorMessage("IfRunner", f"predicate raised exception: {e}"))
+            context.append(ChatMessage.skill("IfRunner", f"predicate raised exception: {e}", is_error=True))
             raise RunnerPredicateError from e
         if result:
-            self.runner.run(context, budget, executor)
+            self.runner.run(context, executor)
```

### Comparing `council_ai-0.0.6/council/runners/parallel.py` & `council_ai-0.0.7/council/runners/parallel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from concurrent import futures
-from council.contexts import ChainContext
 
-from .budget import Budget
+from .runner_context import RunnerContext
 from .runner_base import RunnerBase
 from .runner_executor import RunnerExecutor
 
 
 class Parallel(RunnerBase):
     """
     Runner that execution multiple :class:`.RunnerBase` in parallel
     """
 
     def __init__(self, *runners: RunnerBase):
         self.runners = runners
 
     def _run(
         self,
-        context: ChainContext,
-        budget: Budget,
+        context: RunnerContext,
         executor: RunnerExecutor,
     ) -> None:
-        fs = [executor.submit(lambda: runner.run(context, budget, executor)) for runner in self.runners]
+        contexts = [(runner, context.fork()) for runner in self.runners]
+
+        # Seems like it is a bad idea using lambda as the function in submit,
+        # which results into inconsistent invocation (wrong arguments)
+        fs = [executor.submit(runner.run, inner, executor) for (runner, inner) in contexts]
         try:
-            dones, not_dones = futures.wait(fs, budget.remaining().duration, futures.FIRST_EXCEPTION)
+            dones, not_dones = futures.wait(fs, context.budget.remaining().duration, futures.FIRST_EXCEPTION)
             self.rethrow_if_exception(dones)
         finally:
+            context.merge([context for (_, context) in contexts])
             [f.cancel() for f in fs]
```

### Comparing `council_ai-0.0.6/council/runners/parallel_for.py` & `council_ai-0.0.7/council/runners/parallel_for.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 from concurrent import futures
 from typing import Iterable
 
 from more_itertools import batched
 
-from council.contexts import ChainContext, SkillContext, IterationContext
+from council.contexts import IterationContext, ChainContext
 from council.utils import Option
+from . import RunnerContext, Budget
 
-from .budget import Budget
 from .errrors import RunnerGeneratorError
 from .loop_runner_base import LoopRunnerBase
 from .runner_executor import RunnerExecutor
 from .types import RunnerGenerator
 from .skill_runner_base import SkillRunnerBase
 
 logger = logging.getLogger(__name__)
@@ -42,28 +42,37 @@
             generator(RunnerGenerator): a generator function that yields results
 
         """
         self._generator = generator
         self._skill = skill
         self._parallelism = parallelism
 
-    def _run(self, context: ChainContext, budget: Budget, executor: RunnerExecutor) -> None:
-        for batch in batched(self._generate(context, budget), self._parallelism):
-            fs = [executor.submit(self._run_skill, context, item, budget) for item in batch]
-            try:
-                dones, not_dones = futures.wait(fs, budget.remaining().duration, futures.FIRST_EXCEPTION)
+    def _run(self, context: RunnerContext, executor: RunnerExecutor) -> None:
+        chain_context = context.make_chain_context()
+        inner_contexts = []
+        all_fs = []
+        try:
+            for batch in batched(self._generate(chain_context, context.budget.remaining()), self._parallelism):
+                inner = [context.fork() for _ in batch]
+                inner_contexts.extend(inner)
+                fs = [executor.submit(self._run_skill, inner, iteration) for (inner, iteration) in zip(inner, batch)]
+                all_fs.extend(fs)
+                dones, not_dones = futures.wait(fs, context.budget.remaining().duration, futures.FIRST_EXCEPTION)
                 self.rethrow_if_exception(dones)
-            finally:
-                [f.cancel() for f in fs]
+        finally:
+            [f.cancel() for f in all_fs]
+            context.merge(inner_contexts)
 
-    def _run_skill(self, context: ChainContext, iteration: IterationContext, budget: Budget):
+    def _run_skill(self, context: RunnerContext, iteration: IterationContext):
         index = iteration.index
         logger.debug(f'message="start iteration" index="{index}"')
-        self._skill.execute_skill(SkillContext(context, Option.some(iteration)), budget)
-        logger.debug(f'message="end iteration" index="{index}"')
+        try:
+            self._skill.run_in_current_thread(context, Option.some(iteration))
+        finally:
+            logger.debug(f'message="end iteration" index="{index}"')
 
-    def _generate(self, chain_context: ChainContext, budget: Budget) -> Iterable[IterationContext]:
+    def _generate(self, context: ChainContext, budget: Budget) -> Iterable[IterationContext]:
         try:
-            for index, item in enumerate(self._generator(chain_context, budget)):
+            for index, item in enumerate(self._generator(context, budget.remaining())):
                 yield IterationContext(index, item)
         except Exception as e:
             raise RunnerGeneratorError from e
```

### Comparing `council_ai-0.0.6/council/runners/runner_base.py` & `council_ai-0.0.7/council/runners/runner_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,63 @@
 import abc
 from collections.abc import Set
 from concurrent import futures
 import logging
 
 from council.contexts import ChainContext
+from .runner_context import RunnerContext
 from .budget import Budget
 from .errrors import RunnerTimeoutError, RunnerError
 from .runner_executor import RunnerExecutor
 
 logger = logging.getLogger(__name__)
 
 
 class RunnerBase(abc.ABC):
+    def run_from_chain_context(self, chain_context: ChainContext, budget: Budget, executor: RunnerExecutor):
+        context = RunnerContext(chain_context, budget)
+        try:
+            self.run(context, executor)
+        finally:
+            chain_context.current.extend(context.messages)
+
     """
     Base runner class that handles common execution logic, including error management and timeout
     """
 
     def run(
         self,
-        context: ChainContext,
-        budget: Budget,
+        context: RunnerContext,
         executor: RunnerExecutor,
     ) -> None:
-        if self.should_stop(context, budget):
+        if context.should_stop():
             return
 
         logger.debug("start running %s", self.__class__.__name__)
         try:
-            return self._run(context, budget, executor)
+            self._run(context, executor)
         except futures.TimeoutError as e:
             logger.debug("timeout running %s", self.__class__.__name__)
-            context.cancellationToken.cancel()
+            context.cancellation_token.cancel()
             raise RunnerTimeoutError(self.__class__.__name__) from e
         except RunnerError:
-            context.cancellationToken.cancel()
+            logger.debug("runner error running %s", self.__class__.__name__)
+            context.cancellation_token.cancel()
             raise
         except Exception as e:
             logger.exception("an unexpected error occurred running %s", self.__class__.__name__)
-            context.cancellationToken.cancel()
+            context.cancellation_token.cancel()
             raise RunnerError(f"an unexpected error occurred in {self.__class__.__name__}") from e
         finally:
             logger.debug("done running %s", self.__class__.__name__)
 
     @staticmethod
     def rethrow_if_exception(fs: Set[futures.Future]):
         [f.result(timeout=0) for f in fs]
 
-    @staticmethod
-    def should_stop(context: ChainContext, budget: Budget) -> bool:
-        if budget.is_expired():
-            logger.debug('message="stopping" reason="budget expired"')
-        if context.cancellationToken.cancelled:
-            logger.debug('message="stopping" reason="cancellation token is set"')
-        return budget.is_expired() or context.cancellationToken.cancelled
-
     @abc.abstractmethod
     def _run(
         self,
-        context: ChainContext,
-        budget: Budget,
+        context: RunnerContext,
         executor: RunnerExecutor,
     ) -> None:
         pass
```

### Comparing `council_ai-0.0.6/council/scorers/llm_similarity_scorer.py` & `council_ai-0.0.7/council/scorers/llm_similarity_scorer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Dict, Any
 
 from .scorer_base import ScorerBase
-from council.contexts import AgentMessage
+from council.contexts import ChatMessage
 from council.llm import LLMBase, LLMMessage
 
 
 class LLMSimilarityScorer(ScorerBase):
     """
     Using an LLM to compute a similarity score between two messages.
     """
@@ -22,20 +22,22 @@
         self._expected = expected
 
     def to_dict(self) -> Dict[str, Any]:
         result = super().to_dict()
         result["expected"] = self._expected
         return result
 
-    def _score(self, message: AgentMessage) -> float:
+    def _score(self, message: ChatMessage) -> float:
         messages = self._build_messages(message)
-        llm_response = self._llm.post_chat_request(messages)
-        return self._parse_response(llm_response)
+        choices = self._llm.post_chat_request(messages)
+        if len(choices) < 1:
+            return self._parse_response("")
+        return self._parse_response(choices[0])
 
-    def _build_messages(self, message: AgentMessage) -> List[LLMMessage]:
+    def _build_messages(self, message: ChatMessage) -> List[LLMMessage]:
         prompt = [
             "You are an assistant specialized in evaluating the similarity between two messages.",
             "# Instructions",
             "# compare the {expected} message and the {actual} message",
             "# given a similarity score out of 100%",
             "# provide the result exactly in the format `score: {similarity score}`",
             "Expected message:",
```

### Comparing `council_ai-0.0.6/council/scorers/scorer_base.py` & `council_ai-0.0.7/council/scorers/scorer_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import abc
 import logging
 from typing import Any, Dict
 
-from council.contexts import AgentMessage
+from council.contexts import ChatMessage
 from .scorer_exception import ScorerException
 
 
 logger = logging.getLogger(__name__)
 
 
 class ScorerBase(abc.ABC):
     """
     Base class for implementing a Scorer
     """
 
-    def score(self, message: AgentMessage) -> float:
+    def score(self, message: ChatMessage) -> float:
         """
         Score the given message
 
         Parameters:
-            message (AgentMessage): the message to be scored
+            message (ChatMessage): the message to be scored
 
         Returns:
             similarity score. The greater the value to higher the similarity
 
         Raises:
             SimilarityScorerException: an unexpected error occurs
         """
         try:
             return self._score(message)
         except Exception:
             logging.exception('message="execution failed"')
             raise ScorerException
 
     @abc.abstractmethod
-    def _score(self, message: AgentMessage) -> float:
+    def _score(self, message: ChatMessage) -> float:
         """
         To be implemented with in derived classes with actual scoring logic
         """
         pass
 
     def to_dict(self) -> Dict[str, Any]:
         """
```

### Comparing `council_ai-0.0.6/council/skills/llm_skill.py` & `council_ai-0.0.7/council/skills/llm_skill.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import logging
 from typing import List, Protocol
 
-from council.contexts import ChainContext, SkillMessage, SkillSuccessMessage, SkillContext
+from council.contexts import SkillContext, ChatMessage
 from council.llm import LLMBase, LLMMessage
 from council.prompt import PromptBuilder
 from council.runners import Budget
 from council.skills import SkillBase
 
 
 class ReturnMessages(Protocol):
     def __call__(self, context: SkillContext) -> List[LLMMessage]:
         ...
 
 
 def get_chat_history(context: SkillContext) -> List[LLMMessage]:
     # Convert chat's history and give it to the inner llm
-    return LLMMessage.from_chat_messages(context.chatHistory.messages)
+    return LLMMessage.from_chat_messages(context.chat_history.messages)
 
 
 def get_last_messages(context: SkillContext) -> List[LLMMessage]:
     if context.iteration.is_some():
         it_ctxt = context.iteration.unwrap()
         msg = LLMMessage.user_message(it_ctxt.value)
         return [msg]
-    last_message = context.current.last_message()
+    last_message = context.current.try_last_message
     if last_message.is_none():
         return get_chat_history(context)
     msg = LLMMessage.user_message(last_message.unwrap().message)
     return [msg]
 
 
 class PromptToMessages:
     def __init__(self, prompt_builder: PromptBuilder):
         self._builder = prompt_builder
 
-    def to_system_message(self, context: ChainContext) -> List[LLMMessage]:
+    def to_system_message(self, context: SkillContext) -> List[LLMMessage]:
         msg = self._builder.apply(context)
         logging.debug(msg=f'prompt="{msg}')
         return [LLMMessage.system_message(msg)]
 
-    def to_user_message(self, context: ChainContext) -> List[LLMMessage]:
+    def to_user_message(self, context: SkillContext) -> List[LLMMessage]:
         msg = self._builder.apply(context)
         logging.debug(msg=f'prompt="{msg}')
         return [LLMMessage.user_message(msg)]
 
 
 class LLMSkill(SkillBase):
     """Skill to interact with an `LLM`."""
@@ -57,28 +57,29 @@
     ):
         """
         Initialize a new instance of LLMSkill.
 
         Parameters:
             llm (LLMBase): The instance of the LLM (Language Model) to interact with.
             system_prompt (str): Optional system prompt to provide to the language model.
-            context_messages (Callable[[ChainContext], List[LLMMessage]]): Optional callable to retrieve
+            context_messages (Callable[[SkillContext], List[LLMMessage]]): Optional callable to retrieve
                 context messages.
 
         Returns:
             None
         """
 
         super().__init__(name=name)
         self._llm = llm
         self._context_messages = context_messages
         self._builder = PromptBuilder(system_prompt)
 
-    def execute(self, context: SkillContext, _budget: Budget) -> SkillMessage:
+    def execute(self, context: SkillContext, _budget: Budget) -> ChatMessage:
         """Execute `LLMSkill`."""
 
         history_messages = self._context_messages(context)
         system_prompt = LLMMessage.system_message(self._builder.apply(context))
         messages = [system_prompt, *history_messages]
         llm_response = self._llm.post_chat_request(messages=messages)
-
-        return SkillSuccessMessage(skill_name=self.name, message=llm_response, data=None)
+        if len(llm_response) < 1:
+            return self.build_error_message(message="no response")
+        return self.build_success_message(message=llm_response[0], data=llm_response)
```

### Comparing `council_ai-0.0.6/council/skills/skill_base.py` & `council_ai-0.0.7/council/skills/skill_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 from typing import Any
 from abc import abstractmethod
 
-from council.contexts import SkillMessage, SkillErrorMessage, SkillSuccessMessage, SkillContext
-from council.runners import RunnerSkillError, SkillRunnerBase, Budget
+from council.contexts import SkillContext, ChatMessage
+from council.runners import SkillRunnerBase, Budget
 
 logger = logging.getLogger(__name__)
 
 
 class SkillBase(SkillRunnerBase):
     """
     Abstract base class for a skill.
@@ -39,70 +39,58 @@
 
         Raises:
             None
         """
         return self._name
 
     @abstractmethod
-    def execute(self, context: SkillContext, budget: Budget) -> SkillMessage:
+    def execute(self, context: SkillContext, budget: Budget) -> ChatMessage:
         """
         Executes the skill on the provided chain context and budget.
 
         Args:
             context (SkillContext): The context for executing the skill.
             budget (Budget): The budget for skill execution.
 
         Returns:
-            SkillMessage: The result of skill execution.
+            ChatMessage: The result of skill execution.
 
         Raises:
             None
         """
         pass
 
-    def build_success_message(self, message: str, data: Any = None) -> SkillSuccessMessage:
+    def build_success_message(self, message: str, data: Any = None) -> ChatMessage:
         """
         Builds a success message for the skill with the provided message and optional data.
 
         Args:
             message (str): The success message.
             data (Any, optional): Additional data to include in the message. Defaults to None.
 
         Returns:
-            SkillSuccessMessage: The success message.
+            ChatMessage: The success message.
 
         Raises:
             None
         """
-        return SkillSuccessMessage(self._name, message, data)
+        return ChatMessage.skill(message, data, source=self._name, is_error=False)
 
-    def build_error_message(self, message: str, data: Any = None) -> SkillErrorMessage:
-        return SkillErrorMessage(self._name, message, data)
+    def build_error_message(self, message: str, data: Any = None) -> ChatMessage:
+        return ChatMessage.skill(message, data, source=self._name, is_error=True)
 
-    def from_exception(self, exception: Exception) -> SkillErrorMessage:
-        return self.build_error_message(f"skill '{self._name}' raised exception: {exception}")
-
-    def execute_skill(self, context: SkillContext, budget: Budget) -> None:
-        try:
-            logger.info(f'message="skill execution started" skill="{self.name}"')
-            skill_message = self.execute(context, budget)
-            if skill_message.is_ok():
-                logger.info(
-                    f'message="skill execution ended" skill="{self.name}" skill_message="{skill_message.message}"'
-                )
-            else:
-                logger.warning(
-                    f'message="skill execution ended" skill="{self.name}" skill_message="{skill_message.message}"'
-                )
-        except Exception as e:
-            logger.exception("unexpected error during execution of skill %s", self.name)
-            skill_message = self.from_exception(e)
-            raise RunnerSkillError(f"an unexpected error occurred in skill {self.name}") from e
-        finally:
-            if not self.should_stop(context, budget):
-                context.current.messages.append(skill_message)
+    def execute_skill(self, context: SkillContext, budget: Budget) -> ChatMessage:
+        logger.info(f'message="skill execution started" skill="{self.name}"')
+        skill_message = self.execute(context, budget)
+        if skill_message.is_ok:
+            logger.info(f'message="skill execution ended" skill="{self.name}" skill_message="{skill_message.message}"')
+        else:
+            logger.warning(
+                f'message="skill execution ended" skill="{self.name}" skill_message="{skill_message.message}"'
+            )
+        return skill_message
 
     def __repr__(self):
         return f"SkillBase({self.name})"
 
     def __str__(self):
         return f"Skill {self.name}"
```

### Comparing `council_ai-0.0.6/council/skills/google/google_news_skill.py` & `council_ai-0.0.7/council/skills/google/google_news_skill.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-from council.contexts import ChainContext, SkillMessage
+from council.contexts import ChatMessage, SkillContext
 from council.runners import Budget
 from .google_context import GoogleNewsSearchEngine
 from .. import SkillBase
 
 
 class GoogleNewsSkill(SkillBase):
     """
@@ -12,16 +12,16 @@
 
     """
 
     def __init__(self, suffix: str = ""):
         super().__init__("gnews")
         self.gn = GoogleNewsSearchEngine(period="90d", suffix=suffix)
 
-    def execute(self, context: ChainContext, budget: Budget) -> SkillMessage:
-        prompt = context.chatHistory.last_user_message().unwrap("no user message")
+    def execute(self, context: SkillContext, budget: Budget) -> ChatMessage:
+        prompt = context.chat_history.try_last_user_message.unwrap("no user message")
 
         resp = self.gn.execute(query=prompt.message, nb_results=5)
         response_count = len(resp)
         if response_count > 0:
             return self.build_success_message(
                 f"gnews {response_count} responses for {prompt.message}", json.dumps([r.dict() for r in resp])
             )
```

### Comparing `council_ai-0.0.6/council/skills/google/google_search_skill.py` & `council_ai-0.0.7/council/skills/google/google_search_skill.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-from council.contexts import ChainContext, SkillMessage
+from council.contexts import ChatMessage, SkillContext
 from council.runners import Budget
 from .google_context import GoogleSearchEngine
 from .. import SkillBase
 
 
 class GoogleSearchSkill(SkillBase):
     """
@@ -16,16 +16,16 @@
 
     """
 
     def __init__(self):
         super().__init__("gsearch")
         self.gs = GoogleSearchEngine.from_env()
 
-    def execute(self, context: ChainContext, budget: Budget) -> SkillMessage:
-        prompt = context.chatHistory.last_user_message().unwrap("no user message")
+    def execute(self, context: SkillContext, budget: Budget) -> ChatMessage:
+        prompt = context.chat_history.try_last_user_message.unwrap("no user message")
         resp = self.gs.execute(query=prompt.message, nb_results=5)
         response_count = len(resp)
         if response_count > 0:
             return self.build_success_message(
                 f"{self._name} {response_count} responses for {prompt.message}", json.dumps([r.dict() for r in resp])
             )
         return self.build_error_message("no response")
```

### Comparing `council_ai-0.0.6/council/skills/google/google_context/context_provider.py` & `council_ai-0.0.7/council/skills/google/google_context/context_provider.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/council/skills/google/google_context/google_news.py` & `council_ai-0.0.7/council/skills/google/google_context/google_news.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/council/skills/google/google_context/google_search.py` & `council_ai-0.0.7/council/skills/google/google_context/google_search.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/council/skills/google/google_context/schemas.py` & `council_ai-0.0.7/council/skills/google/google_context/schemas.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/council/utils/option.py` & `council_ai-0.0.7/council/utils/option.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/council/utils/result.py` & `council_ai-0.0.7/council/utils/result.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import Union
+from typing import Union, Optional, Any
 
 
 class Ok:
-    def __init__(self, value):
+    def __init__(self, value: Optional[Any] = None):
         self.value = value
 
     def __repr__(self):
         return f"Ok({self.value})"
 
     @staticmethod
     def is_ok() -> bool:
```

### Comparing `council_ai-0.0.6/docs/.readthedocs.yaml` & `council_ai-0.0.7/docs/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/docs/Makefile` & `council_ai-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/docs/make.bat` & `council_ai-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/docs/source/conf.py` & `council_ai-0.0.7/docs/source/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -62,8 +62,33 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_title = f"{project} {release}"
 html_theme = "furo"
 html_show_copyright = False
 html_show_sphinx = False
 html_static_path = ["_static"]
+html_css_files = [
+    "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/fontawesome.min.css",
+    "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/solid.min.css",
+    "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/brands.min.css",
+]
+# fmt: off
+# so that black does not mess with it
+html_theme_options = {
+    "footer_icons": [
+        {
+            "name": "Discord",
+            "url": "https://discord.gg/uhusYQcP",
+            "html": "",
+            "class": "fa-brands fa-solid fa-discord",
+        },
+        {
+            "name": "Github",
+            "url": "https://github.com/chain-ml/council",
+            "html": "",
+            "class": "fa-brands fa-solid fa-github",
+        },
+    ]
+}
+# fmt: on
+
 # html_theme_options = {"dark_logo": "00_chainml_logo.png", "light_logo": "02_chainml_logo_black.png"}
```

### Comparing `council_ai-0.0.6/docs/source/index.rst` & `council_ai-0.0.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/docs/source/_static/00_chainml_logo.png` & `council_ai-0.0.7/docs/source/_static/00_chainml_logo.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/docs/source/_static/02_chainml_logo_black.png` & `council_ai-0.0.7/docs/source/_static/02_chainml_logo_black.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/docs/source/getting_started/first_example.ipynb` & `council_ai-0.0.7/docs/source/getting_started/first_example.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976003086419754%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'from council.llm import OpenAILLM, "*

 * *            "OpenAILLMConfiguration\\n')], delete: [2]}}, 4: {'source': {insert: [(3, 'openai_llm "*

 * *            "= OpenAILLM(config=OpenAILLMConfiguration.from_env())\\n')], delete: [3]}}, 15: "*

 * *            "{'source': ['Now, we are ready to invoke the agent.\\n']}, 16: {'source': {insert: "*

 * *            '[(0, \'result = agent.execute_from_user_message("hello world?!")\\n\')], delete: [6, '*

 * *            '5, 4, 3, 2, 1, 0]}}}'}*

```diff
@@ -24,15 +24,15 @@
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from council.chains import Chain\n",
                 "from council.skills import LLMSkill\n",
-                "from council.llm import OpenAILLM, OpenAIConfiguration\n"
+                "from council.llm import OpenAILLM, OpenAILLMConfiguration\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
@@ -47,15 +47,15 @@
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "import dotenv\n",
                 "\n",
                 "dotenv.load_dotenv()\n",
-                "openai_llm = OpenAILLM(config=OpenAIConfiguration.from_env())\n"
+                "openai_llm = OpenAILLM(config=OpenAILLMConfiguration.from_env())\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
@@ -167,32 +167,26 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "Now, we are ready to invoke the agent. The ChatHistory object is used to track message history between User and Agents.\n"
+                "Now, we are ready to invoke the agent.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
-                "from council.contexts import AgentContext, ChatHistory\n",
-                "from council.runners import Budget\n",
-                "\n",
-                "chat_history = ChatHistory()\n",
-                "chat_history.add_user_message(message=\"hello world?!\")\n",
-                "context = AgentContext(chat_history=chat_history)\n",
-                "result = agent.execute(context=context, budget=Budget(20))\n",
+                "result = agent.execute_from_user_message(\"hello world?!\")\n",
                 "print(result.best_message.message)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
```

### Comparing `council_ai-0.0.6/docs/source/getting_started/installation.md` & `council_ai-0.0.7/docs/source/getting_started/installation.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/docs/source/introduction/engine_flow.png` & `council_ai-0.0.7/docs/source/introduction/engine_flow.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/docs/source/introduction/key_concepts.md` & `council_ai-0.0.7/docs/source/introduction/key_concepts.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/docs/source/introduction/key_features.md` & `council_ai-0.0.7/docs/source/introduction/key_features.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/docs/source/introduction/welcome.md` & `council_ai-0.0.7/docs/source/introduction/welcome.md`

 * *Files 6% similar despite different names*

```diff
@@ -56,8 +56,17 @@
 00000370: 6869 6c65 2065 6e61 626c 696e 6720 656e  hile enabling en
 00000380: 7465 7270 7269 7365 2d67 7261 6465 206d  terprise-grade m
 00000390: 6f6e 6974 6f72 696e 6720 616e 6420 6164  onitoring and ad
 000003a0: 7661 6e63 6564 2071 7561 6c69 7479 2063  vanced quality c
 000003b0: 6f6e 7472 6f6c 2069 6e20 6120 6675 7475  ontrol in a futu
 000003c0: 7265 2072 656c 6561 7365 2028 636f 6e74  re release (cont
 000003d0: 7269 6275 7469 6f6e 7320 6172 6520 7765  ributions are we
-000003e0: 6c63 6f6d 6529 2e0a                      lcome)..
+000003e0: 6c63 6f6d 6529 2e0a 0a23 2043 6f6d 6d75  lcome)...# Commu
+000003f0: 6e69 7479 0a0a 4a6f 696e 206f 7572 2044  nity..Join our D
+00000400: 6973 636f 7264 2063 6f6d 6d75 6e69 7479  iscord community
+00000410: 2074 6f20 636f 6e6e 6563 7420 7769 7468   to connect with
+00000420: 2074 6865 2063 6f72 6520 6465 7665 6c6f   the core develo
+00000430: 706d 656e 7420 7465 616d 2061 6e64 2075  pment team and u
+00000440: 7365 7273 203c 6120 6872 6566 3d22 6874  sers <a href="ht
+00000450: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
+00000460: 2f75 6875 7359 5163 5022 3e68 6572 653c  /uhusYQcP">here<
+00000470: 2f61 3e2e 0a0a                           /a>...
```

### Comparing `council_ai-0.0.6/docs/source/reference/runners.rst` & `council_ai-0.0.7/docs/source/reference/runners.rst`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/docs/source/reference/runners/parallel_for.rst` & `council_ai-0.0.7/docs/source/reference/runners/parallel_for.rst`

 * *Files 19% similar despite different names*

```diff
@@ -26,33 +26,33 @@
 ---------
 
 This example builds on the previous one and shows how to consume the iteration into a skill.
 
 .. testcode::
 
     from council.chains import Chain
-    from council.contexts import ChainContext, SkillMessage, SkillContext
+    from council.contexts import ChatMessage, ChainContext, SkillContext
     from council.runners import Budget, ParallelFor
     from council.skills import SkillBase
 
     def generator(context: ChainContext, budget: Budget):
         for i in range(0, 5):
             yield f"hi {i}"
 
     class MySkill(SkillBase):
         def __init__(self):
             super().__init__("mySkill")
 
-        def execute(self, context: SkillContext, budget: Budget) -> SkillMessage:
+        def execute(self, context: SkillContext, budget: Budget) -> ChatMessage:
             it = context.iteration.unwrap()
             message = f"index {it.index}, {it.value}"
             print(message)
             return self.build_success_message(message=message)
 
-    chain = Chain(name="name", description="parallel for", runners=[ParallelFor(generator, MySkill(), parallelism=1)])
+    chain = Chain(name="name", description="parallel for", runners=[ParallelFor(generator, MySkill(), parallelism=5)])
     context = ChainContext.empty()
     context.new_iteration()
     chain.execute(context, Budget(1))
 
 The output would looks like.
 
 .. testoutput::
```

### Comparing `council_ai-0.0.6/docs/source/use_cases/langchain_llm_integration.ipynb` & `council_ai-0.0.7/docs/source/use_cases/langchain_llm_integration.ipynb`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/docs/source/use_cases/multi_chain_agent.ipynb` & `council_ai-0.0.7/docs/source/use_cases/multi_chain_agent.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994444444444445%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'from council.llm import AzureLLM, "*

 * *            "AzureLLMConfiguration\\n')], delete: [2]}}, 4: {'source': {insert: [(1, 'azure_llm = "*

 * *            "AzureLLM(config=AzureLLMConfiguration.from_env())')], delete: [1]}}}"}*

```diff
@@ -47,15 +47,15 @@
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from council.chains import Chain\n",
                 "from council.skills import LLMSkill\n",
-                "from council.llm import AzureLLM, AzureConfiguration\n",
+                "from council.llm import AzureLLM, AzureLLMConfiguration\n",
                 "import dotenv"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
@@ -69,15 +69,15 @@
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "dotenv.load_dotenv()\n",
-                "azure_llm = AzureLLM(config=AzureConfiguration.from_env())"
+                "azure_llm = AzureLLM(config=AzureLLMConfiguration.from_env())"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
```

### Comparing `council_ai-0.0.6/stubs/GoogleNews.pyi` & `council_ai-0.0.7/stubs/GoogleNews.pyi`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/LICENSE` & `council_ai-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.6/README.md` & `council_ai-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: council-ai
+Version: 0.0.7
+Summary: Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications
+Project-URL: Source, https://github.com/chain-ml/council
+Project-URL: Documentation, https://council.dev
+License-Expression: Apache-2.0
+License-File: LICENSE
+Requires-Python: >=3.9
+Requires-Dist: google-api-python-client-stubs
+Requires-Dist: google-api-python-client==2.93.0
+Requires-Dist: googlenews==1.6.8
+Requires-Dist: httpx==0.24.1
+Requires-Dist: jinja2~=3.1.2
+Requires-Dist: more-itertools~=9.1.0
+Requires-Dist: progressbar==2.5
+Requires-Dist: python-dotenv==1.0.0
+Requires-Dist: requests~=2.31.0
+Description-Content-Type: text/markdown
+
 <h1><p align="center">Council - AI Agent Platform with Advanced Control and Scalable Oversight</p></h1>
 
 # Welcome
 
 Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications using teams of `agents` - built in Python and (soon) Rust.
 
 Council extends the LLM tool ecosystem by enabling advanced control and scalable oversight for AI agents. Users can create sophisticated agents with predictable behavior by leveraging Council's powerful approach to control flow using Controllers, Filters, Evaluators and Budgets for agents. This allows the automated routing between agents, comparing, evaluating and selecting the best results for a (sub-)task. 
@@ -66,24 +86,24 @@
 ## Usage
 
 Import Council.
 
 ```python
 from council.chains import Chain
 from council.skills import LLMSkill
-from council.llm import OpenAILLM, OpenAIConfiguration
+from council.llm import OpenAILLM, OpenAILLMConfiguration
 ```
 
 Setup API keys in .env file (example in repository) and use it to setup the LLM (here: OpenAILLM).
 
 ```python
 import dotenv
 
 dotenv.load_dotenv()
-openai_llm = OpenAILLM(config=OpenAIConfiguration.from_env())
+openai_llm = OpenAILLM(config=OpenAILLMConfiguration.from_env())
 ```
 
 Create your first Hello World Skill and Wrap it in a Chain.
 
 ```python
 prompt = "You are responding to every prompt with a short poem titled hello world"
 hw_skill = LLMSkill(llm=openai_llm, system_prompt=prompt)
@@ -120,24 +140,18 @@
 
 ```python
 from council.agents import Agent
 
 agent = Agent(controller=controller, chains=[hw_chain, em_chain], evaluator=evaluator)
 ```
 
-Now, we are ready to invoke the agent. The ChatHistory object is used to track message history between User and Agents.
+Now, we are ready to invoke the agent.
 
 ```python
-from council.contexts import AgentContext, ChatHistory
-from council.runners import Budget
-
-chat_history = ChatHistory()
-chat_history.add_user_message(message="hello world?!")
-context = AgentContext(chat_history=chat_history)
-result = agent.execute(context=context, budget=Budget(20))
+result = agent.execute_from_user_message("hello world?!")
 print(result.best_message.message)
 ```
 
 ## Linter
 
 Use `make lint` to verify your code.
 
@@ -170,9 +184,9 @@
 
 # Contributors
 
 Council is a project under active development. We welcome all contributions, pull requests, feature requests or reported issues.
 
 # Community
 
-Join our Discord community to connect with the core development team and users here: (link to be provided soon).
+Join our Discord community to connect with the core development team and users <a href="https://discord.gg/uhusYQcP">here</a>.
```

### Comparing `council_ai-0.0.6/pyproject.toml` & `council_ai-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "council-ai"
-version = "0.0.6"
+version = "0.0.7"
 description = "Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = []
 license = "Apache-2.0"
 
 dynamic = ["dependencies"]
```

### Comparing `council_ai-0.0.6/PKG-INFO` & `council_ai-0.0.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: council-ai
-Version: 0.0.6
-Summary: Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications
-Project-URL: Source, https://github.com/chain-ml/council
-Project-URL: Documentation, https://council.dev
-License-Expression: Apache-2.0
-License-File: LICENSE
-Requires-Python: >=3.9
-Requires-Dist: google-api-python-client-stubs
-Requires-Dist: google-api-python-client==2.93.0
-Requires-Dist: googlenews==1.6.8
-Requires-Dist: httpx==0.24.1
-Requires-Dist: jinja2~=3.1.2
-Requires-Dist: more-itertools~=9.1.0
-Requires-Dist: progressbar==2.5
-Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: requests~=2.31.0
-Description-Content-Type: text/markdown
-
 <h1><p align="center">Council - AI Agent Platform with Advanced Control and Scalable Oversight</p></h1>
 
 # Welcome
 
 Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications using teams of `agents` - built in Python and (soon) Rust.
 
 Council extends the LLM tool ecosystem by enabling advanced control and scalable oversight for AI agents. Users can create sophisticated agents with predictable behavior by leveraging Council's powerful approach to control flow using Controllers, Filters, Evaluators and Budgets for agents. This allows the automated routing between agents, comparing, evaluating and selecting the best results for a (sub-)task. 
@@ -86,24 +66,24 @@
 ## Usage
 
 Import Council.
 
 ```python
 from council.chains import Chain
 from council.skills import LLMSkill
-from council.llm import OpenAILLM, OpenAIConfiguration
+from council.llm import OpenAILLM, OpenAILLMConfiguration
 ```
 
 Setup API keys in .env file (example in repository) and use it to setup the LLM (here: OpenAILLM).
 
 ```python
 import dotenv
 
 dotenv.load_dotenv()
-openai_llm = OpenAILLM(config=OpenAIConfiguration.from_env())
+openai_llm = OpenAILLM(config=OpenAILLMConfiguration.from_env())
 ```
 
 Create your first Hello World Skill and Wrap it in a Chain.
 
 ```python
 prompt = "You are responding to every prompt with a short poem titled hello world"
 hw_skill = LLMSkill(llm=openai_llm, system_prompt=prompt)
@@ -140,24 +120,18 @@
 
 ```python
 from council.agents import Agent
 
 agent = Agent(controller=controller, chains=[hw_chain, em_chain], evaluator=evaluator)
 ```
 
-Now, we are ready to invoke the agent. The ChatHistory object is used to track message history between User and Agents.
+Now, we are ready to invoke the agent.
 
 ```python
-from council.contexts import AgentContext, ChatHistory
-from council.runners import Budget
-
-chat_history = ChatHistory()
-chat_history.add_user_message(message="hello world?!")
-context = AgentContext(chat_history=chat_history)
-result = agent.execute(context=context, budget=Budget(20))
+result = agent.execute_from_user_message("hello world?!")
 print(result.best_message.message)
 ```
 
 ## Linter
 
 Use `make lint` to verify your code.
 
@@ -190,9 +164,9 @@
 
 # Contributors
 
 Council is a project under active development. We welcome all contributions, pull requests, feature requests or reported issues.
 
 # Community
 
-Join our Discord community to connect with the core development team and users here: (link to be provided soon).
+Join our Discord community to connect with the core development team and users <a href="https://discord.gg/uhusYQcP">here</a>.
```

