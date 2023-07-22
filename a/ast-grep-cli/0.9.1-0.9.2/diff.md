# Comparing `tmp/ast_grep_cli-0.9.1.tar.gz` & `tmp/ast_grep_cli-0.9.2.tar.gz`

## Comparing `ast_grep_cli-0.9.1.tar` & `ast_grep_cli-0.9.2.tar`

### file list

```diff
@@ -1,72 +1,75 @@
--rw-r--r--   0        0        0     2116 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/Cargo.toml
--rw-r--r--   0     1001      123     1023 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/cpp.rs
--rw-r--r--   0     1001      123      858 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/csharp.rs
--rw-r--r--   0     1001      123      823 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/css.rs
--rw-r--r--   0     1001      123     1192 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/go.rs
--rw-r--r--   0     1001      123     1216 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/kotlin.rs
--rw-r--r--   0     1001      123    12673 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/lib.rs
--rw-r--r--   0     1001      123     3094 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/parsers.rs
--rw-r--r--   0     1001      123     2043 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/python.rs
--rw-r--r--   0     1001      123     1974 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/rust.rs
--rw-r--r--   0     1001      123     1646 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/scala.rs
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-lsp/Cargo.toml
--rw-r--r--   0     1001      123    11369 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-lsp/src/lib.rs
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/Cargo.toml
--rw-r--r--   0     1001      123     6946 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/constraints.rs
--rw-r--r--   0     1001      123     6838 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/deserialize_env.rs
--rw-r--r--   0     1001      123     4880 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/lib.rs
--rw-r--r--   0     1001      123     2765 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/maybe.rs
--rw-r--r--   0     1001      123     6514 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/referent_rule.rs
--rw-r--r--   0     1001      123    16160 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
--rw-r--r--   0     1001      123     4138 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
--rw-r--r--   0     1001      123    13151 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/rule.rs
--rw-r--r--   0     1001      123     6357 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/rule_collection.rs
--rw-r--r--   0     1001      123    11610 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/rule_config.rs
--rw-r--r--   0     1001      123     6716 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/transform.rs
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/Cargo.toml
--rw-r--r--   0     1001      123     2331 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/language.rs
--rw-r--r--   0     1001      123     3858 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/lib.rs
--rw-r--r--   0     1001      123    14850 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/match_tree.rs
--rw-r--r--   0     1001      123     3480 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/kind.rs
--rw-r--r--   0     1001      123     3783 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/node_match.rs
--rw-r--r--   0     1001      123    11138 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/pattern.rs
--rw-r--r--   0     1001      123      982 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/text.rs
--rw-r--r--   0     1001      123     6540 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher.rs
--rw-r--r--   0     1001      123    11359 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/meta_var.rs
--rw-r--r--   0     1001      123    15493 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/node.rs
--rw-r--r--   0     1001      123    16351 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/ops.rs
--rw-r--r--   0     1001      123     3089 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/pinned.rs
--rw-r--r--   0     1001      123    10936 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer/indent.rs
--rw-r--r--   0     1001      123     6181 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer/structural.rs
--rw-r--r--   0     1001      123     9380 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer/template.rs
--rw-r--r--   0     1001      123     2572 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer.rs
--rw-r--r--   0     1001      123     8489 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/source.rs
--rw-r--r--   0     1001      123    16414 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/traversal.rs
--rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-dynamic/Cargo.toml
--rw-r--r--   0     1001      123     7940 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-dynamic/src/lib.rs
--rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/crates/cli/Cargo.toml
--rw-r--r--   0     1001      123      249 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/bin/ast-grep.rs
--rw-r--r--   0     1001      123    11003 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/config.rs
--rw-r--r--   0     1001      123    10194 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/error.rs
--rw-r--r--   0     1001      123     4312 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/lang.rs
--rw-r--r--   0     1001      123     5396 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/lib.rs
--rw-r--r--   0     1001      123     1015 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/lsp.rs
--rw-r--r--   0     1001      123       94 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/main.rs
--rw-r--r--   0     1001      123    10205 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/new.rs
--rw-r--r--   0     1001      123    23910 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/print/colored_print.rs
--rw-r--r--   0     1001      123     7648 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/print/interactive_print.rs
--rw-r--r--   0     1001      123     9327 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/print/json_print.rs
--rw-r--r--   0     1001      123     3179 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/print/mod.rs
--rw-r--r--   0     1001      123     9061 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/run.rs
--rw-r--r--   0     1001      123    10644 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/scan.rs
--rw-r--r--   0     1001      123     7418 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/utils.rs
--rw-r--r--   0     1001      123    24703 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/verify.rs
--rw-r--r--   0     1001      123      593 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/tests/common/mod.rs
--rw-r--r--   0     1001      123      901 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/tests/run_test.rs
--rw-r--r--   0     1001      123     1363 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/tests/scan_test.rs
--rw-r--r--   0     1001      123     1025 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/tests/verify_test.rs
--rw-r--r--   0     1001      123     1236 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/pyproject.toml
--rw-r--r--   0     1001      123    59830 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/Cargo.lock
--rw-r--r--   0     1001      123     4951 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/README.md
--rw-r--r--   0     1001      123     1077 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/LICENSE
--rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/Cargo.toml
+-rw-r--r--   0     1001      123     2331 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/language.rs
+-rw-r--r--   0     1001      123     3858 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/lib.rs
+-rw-r--r--   0     1001      123    15133 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/match_tree.rs
+-rw-r--r--   0     1001      123     3480 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/kind.rs
+-rw-r--r--   0     1001      123     3783 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      123    11138 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      123      982 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/text.rs
+-rw-r--r--   0     1001      123     6540 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher.rs
+-rw-r--r--   0     1001      123    11359 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/meta_var.rs
+-rw-r--r--   0     1001      123    15558 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/node.rs
+-rw-r--r--   0     1001      123    16351 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/ops.rs
+-rw-r--r--   0     1001      123     3089 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/pinned.rs
+-rw-r--r--   0     1001      123    10936 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer/indent.rs
+-rw-r--r--   0     1001      123     6181 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer/structural.rs
+-rw-r--r--   0     1001      123     9380 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer/template.rs
+-rw-r--r--   0     1001      123     2572 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer.rs
+-rw-r--r--   0     1001      123     8489 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/source.rs
+-rw-r--r--   0     1001      123    16414 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/traversal.rs
+-rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-dynamic/Cargo.toml
+-rw-r--r--   0     1001      123     7940 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-dynamic/src/lib.rs
+-rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/Cargo.toml
+-rw-r--r--   0     1001      123     1023 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/cpp.rs
+-rw-r--r--   0     1001      123      858 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/csharp.rs
+-rw-r--r--   0     1001      123      815 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/css.rs
+-rw-r--r--   0     1001      123     1192 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/go.rs
+-rw-r--r--   0     1001      123     1013 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/json.rs
+-rw-r--r--   0     1001      123     1216 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/kotlin.rs
+-rw-r--r--   0     1001      123    12868 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/lib.rs
+-rw-r--r--   0     1001      123      924 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/lua.rs
+-rw-r--r--   0     1001      123     3198 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/parsers.rs
+-rw-r--r--   0     1001      123     2043 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/python.rs
+-rw-r--r--   0     1001      123     1974 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/rust.rs
+-rw-r--r--   0     1001      123     1646 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/scala.rs
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-lsp/Cargo.toml
+-rw-r--r--   0     1001      123    11369 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-lsp/src/lib.rs
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/Cargo.toml
+-rw-r--r--   0     1001      123     6946 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/constraints.rs
+-rw-r--r--   0     1001      123     6838 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/deserialize_env.rs
+-rw-r--r--   0     1001      123     4880 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/lib.rs
+-rw-r--r--   0     1001      123     2765 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/maybe.rs
+-rw-r--r--   0     1001      123     6514 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/referent_rule.rs
+-rw-r--r--   0     1001      123    16160 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
+-rw-r--r--   0     1001      123     4138 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
+-rw-r--r--   0     1001      123    13151 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/rule.rs
+-rw-r--r--   0     1001      123     6357 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/rule_collection.rs
+-rw-r--r--   0     1001      123    11610 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/rule_config.rs
+-rw-r--r--   0     1001      123     6716 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/transform.rs
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/crates/cli/Cargo.toml
+-rw-r--r--   0     1001      123      249 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/bin/ast-grep.rs
+-rw-r--r--   0     1001      123    11003 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/config.rs
+-rw-r--r--   0     1001      123    10194 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/error.rs
+-rw-r--r--   0     1001      123     4312 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/lang.rs
+-rw-r--r--   0     1001      123     5585 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/lib.rs
+-rw-r--r--   0     1001      123     1015 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/lsp.rs
+-rw-r--r--   0     1001      123       94 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/main.rs
+-rw-r--r--   0     1001      123    10212 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/new.rs
+-rw-r--r--   0     1001      123     4861 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/print/cloud_print.rs
+-rw-r--r--   0     1001      123    23920 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/print/colored_print.rs
+-rw-r--r--   0     1001      123     7648 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/print/interactive_print.rs
+-rw-r--r--   0     1001      123     9327 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/print/json_print.rs
+-rw-r--r--   0     1001      123     3243 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/print/mod.rs
+-rw-r--r--   0     1001      123     9061 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/run.rs
+-rw-r--r--   0     1001      123    10914 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/scan.rs
+-rw-r--r--   0     1001      123     7418 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/utils.rs
+-rw-r--r--   0     1001      123    24703 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/verify.rs
+-rw-r--r--   0     1001      123      593 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/tests/common/mod.rs
+-rw-r--r--   0     1001      123      901 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/tests/run_test.rs
+-rw-r--r--   0     1001      123     1364 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/tests/scan_test.rs
+-rw-r--r--   0     1001      123     1027 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/tests/verify_test.rs
+-rw-r--r--   0     1001      123     1236 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/pyproject.toml
+-rw-r--r--   0     1001      123    60094 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/Cargo.lock
+-rw-r--r--   0     1001      123     4951 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/README.md
+-rw-r--r--   0     1001      123     1077 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/LICENSE
+-rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/PKG-INFO
```

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/Cargo.toml` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.9.1"
+version= "0.9.2"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 serde= { version = "1.0", features = ["derive"] }
 
-tree-sitter-c = { version = "0.20.2", optional = true }
-tree-sitter-cpp = { version = "0.20.0", optional = true }
+tree-sitter-c = { version = "0.20.3", optional = true }
+tree-sitter-cpp = { version = "0.20.1", optional = true }
 tree-sitter-c-sharp = { version = "0.20.0", package = "ast-grep-tree-sitter-c-sharp", optional = true }
 tree-sitter-css = { version = "0.19.0", optional = true }
 tree-sitter-dart= { version = "0.0.3", optional = true }
 tree-sitter-go = { version = "0.19.1", optional = true }
 tree-sitter-html = { version = "0.19.0", optional = true }
 tree-sitter-java = { version = "0.20.0", optional = true }
 tree-sitter-javascript = { version = "0.20.0", optional = true }
+tree-sitter-json = { version = "0.19.0", optional = true }
 tree-sitter-kotlin = { version = "0.2.11", optional = true }
 tree-sitter-lua = { version = "0.0.18", optional = true }
 tree-sitter-python = { version = "0.20.2", optional = true }
 tree-sitter-ruby = { version = "0.20.0", optional = true }
 tree-sitter-rust = { version = "0.20.3", optional = true }
 tree-sitter-scala = { version = "0.20.1", optional = true }
 tree-sitter-swift = { version = "0.3.6", optional = true }
@@ -42,14 +43,15 @@
   "tree-sitter-c-sharp",
   "tree-sitter-css",
   "tree-sitter-dart",
   "tree-sitter-go",
   "tree-sitter-html",
   "tree-sitter-java",
   "tree-sitter-javascript",
+  "tree-sitter-json",
   "tree-sitter-kotlin",
   "tree-sitter-lua",
   "tree-sitter-python",
   "tree-sitter-ruby",
   "tree-sitter-rust",
   "tree-sitter-scala",
   "tree-sitter-swift",
```

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/cpp.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/csharp.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/css.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/css.rs`

 * *Files 12% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 fn test_match(query: &str, source: &str) {
   use crate::test::test_match_lang;
   test_match_lang(query, source, Css);
 }
 
 #[test]
-fn test_c_sharp_pattern() {
+fn test_css_pattern() {
   test_match("$A { color: red; }", ".a { color: red; }");
   test_match(".a { color: $COLOR; }", ".a { color: red; }");
   test_match(".a { $PROP: red; }", ".a { color: red; }");
 }
 
 fn test_replace(src: &str, pattern: &str, replacer: &str) -> Result<String, TSParseError> {
   use crate::test::test_replace_lang;
   test_replace_lang(src, pattern, replacer, Css)
 }
 
 #[test]
-fn test_c_sharp_replace() -> Result<(), TSParseError> {
+fn test_css_replace() -> Result<(), TSParseError> {
   let ret = test_replace(
     ".a {color: red; }",
     ".a { color: $COLOR}",
     ".a {background: $COLOR}",
   )?;
   assert_eq!(ret, ".a {background: red}");
   Ok(())
```

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/go.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/kotlin.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/kotlin.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/lib.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 //! Otherwise, you can define it as a stub language using `impl_lang!`.
 //! To see the full list of languages, visit `<https://ast-grep.github.io/reference/languages.html>`
 
 mod cpp;
 mod csharp;
 mod css;
 mod go;
+mod json;
 mod kotlin;
+mod lua;
 mod parsers;
 mod python;
 mod rust;
 mod scala;
 
 use ast_grep_core::language::TSLanguage;
 use ast_grep_core::meta_var::MetaVariable;
@@ -96,14 +98,15 @@
 
 // Stub Language without preprocessing
 // Language Name, tree-sitter-name, alias, extension
 impl_lang!(Dart, language_dart);
 impl_lang!(Html, language_html);
 impl_lang!(Java, language_java);
 impl_lang!(JavaScript, language_javascript);
+impl_lang!(Json, language_json);
 impl_lang!(Lua, language_lua);
 impl_lang!(Scala, language_scala);
 impl_lang!(Swift, language_swift);
 impl_lang!(Thrift, language_thrift);
 impl_lang!(Tsx, language_tsx);
 impl_lang!(TypeScript, language_typescript);
 // See ripgrep for extensions
@@ -117,14 +120,15 @@
   CSharp,
   Css,
   Dart,
   Go,
   Html,
   Java,
   JavaScript,
+  Json,
   Kotlin,
   Lua,
   Python,
   Ruby,
   Rust,
   Scala,
   Swift,
@@ -133,15 +137,15 @@
   TypeScript,
 }
 
 impl SupportLang {
   pub const fn all_langs() -> &'static [SupportLang] {
     use SupportLang::*;
     &[
-      C, Cpp, CSharp, Css, Dart, Go, Html, Java, JavaScript, Kotlin, Lua, Python, Ruby, Rust,
+      C, Cpp, CSharp, Css, Dart, Go, Html, Java, JavaScript, Json, Kotlin, Lua, Python, Ruby, Rust,
       Scala, Swift, Thrift, Tsx, TypeScript,
     ]
   }
 
   pub fn file_types(&self) -> Types {
     file_types(self)
   }
@@ -187,14 +191,15 @@
     CSharp => &["cs", "csharp"],
     Css => &["css"],
     Dart => &["dart"],
     Go => &["go", "golang"],
     Html => &["html"],
     Java => &["java"],
     JavaScript => &["javascript", "js", "jsx"],
+    Json => &["json"],
     Kotlin => &["kotlin", "kt"],
     Lua => &["lua"],
     Python => &["py", "python"],
     Ruby => &["rb", "ruby"],
     Rust => &["rs", "rust"],
     Scala => &["scala"],
     Swift => &["swift"],
@@ -228,14 +233,15 @@
       S::CSharp => CSharp.$method($($pname,)*),
       S::Css => Css.$method($($pname,)*),
       S::Dart => Dart.$method($($pname,)*),
       S::Go => Go.$method($($pname,)*),
       S::Html => Html.$method($($pname,)*),
       S::Java => Java.$method($($pname,)*),
       S::JavaScript => JavaScript.$method($($pname,)*),
+      S::Json => Json.$method($($pname,)*),
       S::Kotlin => Kotlin.$method($($pname,)*),
       S::Lua => Lua.$method($($pname,)*),
       S::Python => Python.$method($($pname,)*),
       S::Ruby => Ruby.$method($($pname,)*),
       S::Rust => Rust.$method($($pname,)*),
       S::Scala => Scala.$method($($pname,)*),
       S::Swift => Swift.$method($($pname,)*),
@@ -278,14 +284,15 @@
     CSharp => &["cs"],
     Css => &["css", "scss"],
     Dart => &["dart"],
     Go => &["go"],
     Html => &["html", "htm", "xhtml"],
     Java => &["java"],
     JavaScript => &["cjs", "js", "mjs", "jsx"],
+    Json => &["json"],
     Kotlin => &["kt", "ktm", "kts"],
     Lua => &["lua"],
     Python => &["py", "py3", "pyi", "bzl"],
     Ruby => &["rb", "rbw", "gemspec"],
     Rust => &["rs"],
     Scala => &["scala", "sc", "sbt"],
     Swift => &["swift"],
@@ -331,14 +338,15 @@
     L::Dart => builder.select("dart"),
     L::Go => builder.select("go"),
     L::Html => builder.select("html"),
     L::Java => builder.select("java"),
     L::JavaScript => {
       add_custom_file_type(&mut builder, "myjs", &["*.js", "*.cjs", "*.jsx", "*.mjs"])
     }
+    L::Json => builder.select("json"),
     L::Kotlin => builder.select("kotlin"),
     L::Lua => builder.select("lua"),
     L::Python => builder.select("py"),
     L::Ruby => builder.select("ruby"),
     L::Rust => builder.select("rust"),
     L::Scala => builder.select("scala"),
     L::Swift => builder.select("swift"),
```

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/parsers.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/parsers.rs`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
   }
   pub fn language_java() -> TSLanguage {
     tree_sitter_java::language().into()
   }
   pub fn language_javascript() -> TSLanguage {
     tree_sitter_javascript::language().into()
   }
+  pub fn language_json() -> TSLanguage {
+    tree_sitter_json::language().into()
+  }
   pub fn language_kotlin() -> TSLanguage {
     tree_sitter_kotlin::language().into()
   }
   pub fn language_lua() -> TSLanguage {
     tree_sitter_lua::language().into()
   }
   pub fn language_python() -> TSLanguage {
@@ -92,14 +95,15 @@
     language_c_sharp,
     language_css,
     language_dart,
     language_go,
     language_html,
     language_java,
     language_javascript,
+    language_json,
     language_kotlin,
     language_lua,
     language_python,
     language_ruby,
     language_rust,
     language_scala,
     language_swift,
```

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/python.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/rust.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/rust.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/scala.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/scala.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-lsp/Cargo.toml` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-lsp/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 name = "ast-grep-lsp"
 description = "Search and Rewrite code at large scale using precise AST pattern"
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
-version= "0.9.1"
+version= "0.9.2"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
 
 [dependencies]
```

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-lsp/src/lib.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-lsp/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/Cargo.toml` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.9.1"
+version= "0.9.2"
 
 [features]
 default = ["regex"]
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 anyhow = "1.0"
 bit-set= { version = "0.5.3" }
 globset = "0.4.11"
 regex = { version = "1.9.1" , optional = true }
 serde= { version = "1.0", features = ["derive"] }
-serde_yaml = "0.9.23"
-thiserror= "1.0.43"
+serde_yaml = "0.9.25"
+thiserror= "1.0.44"
```

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/constraints.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/constraints.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/deserialize_env.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/lib.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/maybe.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/referent_rule.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/relational_rule/mod.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/relational_rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/rule.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/rule_collection.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/rule_config.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/rule_config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/transform.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/transform.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/Cargo.toml` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 edition= "2021"
 homepage= "https://ast-grep.github.io/"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.9.1"
+version= "0.9.2"
 
 [dependencies]
 bit-set= { version = "0.5.3" }
 regex = { version = "1.9.1" , optional = true }
-thiserror= "1.0.43"
+thiserror= "1.0.44"
 tree-sitter= { version = "0.9.2", package = "tree-sitter-facade-sg" }
 
 [features]
 default = ["regex"]
```

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/language.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/lib.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/match_tree.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/match_tree.rs`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,21 @@
     MV::NamedEllipsis(name) => {
       env.to_mut().insert(name, candidate.clone())?;
       Some(candidate)
     }
   }
 }
 
+#[inline]
+fn is_node_eligible_for_meta_var(goal: &Node<impl Doc>, is_leaf: bool) -> bool {
+  // allow Error as meta_var
+  // see https://github.com/ast-grep/ast-grep/issues/526
+  is_leaf || goal.is_error()
+}
+
 fn try_get_ellipsis_mode(node: &Node<impl Doc>) -> Result<Option<String>, ()> {
   match extract_var_from_node(node).ok_or(())? {
     MetaVariable::Ellipsis => Ok(None),
     MetaVariable::NamedEllipsis(n) => Ok(Some(n)),
     _ => Err(()),
   }
 }
@@ -63,15 +70,15 @@
 }
 
 pub fn match_end_non_recursive<D: Doc>(
   goal: &Node<impl Doc<Lang = D::Lang>>,
   candidate: Node<D>,
 ) -> Option<usize> {
   let is_leaf = goal.is_named_leaf();
-  if is_leaf && extract_var_from_node(goal).is_some() {
+  if is_node_eligible_for_meta_var(goal, is_leaf) && extract_var_from_node(goal).is_some() {
     return Some(candidate.range().end);
   }
   if goal.kind_id() != candidate.kind_id() {
     return None;
   }
   if is_leaf {
     if extract_var_from_node(goal).is_some() {
@@ -167,15 +174,15 @@
 
 pub fn match_node_non_recursive<'tree, D: Doc>(
   goal: &Node<impl Doc>,
   candidate: Node<'tree, D>,
   env: &mut Cow<MetaVarEnv<'tree, D>>,
 ) -> Option<Node<'tree, D>> {
   let is_leaf = goal.is_named_leaf();
-  if is_leaf {
+  if is_node_eligible_for_meta_var(goal, is_leaf) {
     if let Some(matched) = match_leaf_meta_var(goal, candidate.clone(), env) {
       return Some(matched);
     }
   }
   if goal.kind_id() != candidate.kind_id() {
     return None;
   }
```

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/kind.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/node_match.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/pattern.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/pattern.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/text.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/meta_var.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/meta_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/node.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/node.rs`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,17 @@
   }
   pub fn is_leaf(&self) -> bool {
     self.inner.child_count() == 0
   }
   pub fn is_named_leaf(&self) -> bool {
     self.inner.named_child_count() == 0
   }
+  pub fn is_error(&self) -> bool {
+    self.inner.is_error()
+  }
   pub fn kind(&self) -> Cow<str> {
     self.inner.kind()
   }
   pub fn kind_id(&self) -> KindId {
     self.inner.kind_id()
   }
```

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/ops.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/pinned.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer/indent.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer/structural.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer/template.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/source.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/traversal.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-dynamic/Cargo.toml` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-dynamic/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.9.1"
+version= "0.9.2"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 libloading = "0.8"
 serde= { version = "1.0", features = ["derive"] }
-thiserror= "1.0.43"
+thiserror= "1.0.44"
 tree-sitter-native = { version = "0.20.10", package = "tree-sitter" }
```

### Comparing `ast_grep_cli-0.9.1/local_dependencies/ast-grep-dynamic/src/lib.rs` & `ast_grep_cli-0.9.2/local_dependencies/ast-grep-dynamic/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/crates/cli/Cargo.toml` & `ast_grep_cli-0.9.2/crates/cli/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 categories = ["command-line-utilities", "development-tools", "parsing"]
 default-run = "sg"
 # use relative path because maturin does not recognize
 readme = "../../README.md"
 license-file = "../../LICENSE"
 
-version= "0.9.1"
+version= "0.9.2"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 # license.workspace = true
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 homepage= "https://ast-grep.github.io/"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
@@ -31,18 +31,18 @@
 ast-grep-dynamic.path = "../../local_dependencies/ast-grep-dynamic"
 ast-grep-language.path = "../../local_dependencies/ast-grep-language"
 ast-grep-lsp.path = "../../local_dependencies/ast-grep-lsp"
 
 ansi_term = "0.12"
 anyhow = "1.0"
 atty = "0.2.14"
-clap = { version = "4.3.12", features = ["derive"] }
+clap = { version = "4.3.19", features = ["derive"] }
 codespan-reporting = "0.11.1"
 crossterm = "0.26.1"
 ignore= { version = "0.4.20" }
 inquire = "0.6.2"
 num_cpus = "1.16.0"
 serde= { version = "1.0", features = ["derive"] }
 serde_json = "1.0.103"
-serde_yaml = "0.9.23"
+serde_yaml = "0.9.25"
 similar = { version = "2.2.1", features = ["inline"] }
 tokio = { version = "1", features = ["rt-multi-thread", "io-std"] }
```

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/config.rs` & `ast_grep_cli-0.9.2/crates/cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/error.rs` & `ast_grep_cli-0.9.2/crates/cli/src/error.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/lang.rs` & `ast_grep_cli-0.9.2/crates/cli/src/lang.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/lib.rs` & `ast_grep_cli-0.9.2/crates/cli/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -172,17 +172,23 @@
     ok("scan");
     ok("scan dir");
     ok("scan -r test-rule.yml dir");
     ok("scan -c test-rule.yml dir");
     ok("scan -c test-rule.yml");
     ok("scan --report-style short"); // conflict
     ok("scan dir1 dir2 dir3"); // multiple paths
+    ok("scan -r test.yml --format github");
+    ok("scan -f github");
+    ok("scan --interactive");
     error("scan -i --json dir"); // conflict
     error("scan --report-style rich --json dir"); // conflict
     error("scan -r test.yml -c test.yml --json dir"); // conflict
+    error("scan -f gitlab");
+    error("scan -f github -i");
+    error("scan -f local");
   }
 
   #[test]
   fn test_test() {
     ok("test");
     ok("test -c sgconfig.yml");
     ok("test --skip-snapshot-tests");
```

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/lsp.rs` & `ast_grep_cli-0.9.2/crates/cli/src/lsp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/new.rs` & `ast_grep_cli-0.9.2/crates/cli/src/new.rs`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,16 @@
   }
 }
 
 fn create_new_project(arg: NewArg) -> Result<()> {
   println!("Creating a new ast-grep project...");
   let rule_dirs = arg.ask_dir_and_create("Where do you want to have your rules?", "rules")?;
   let test_dirs = if arg.confirm("Do you want to create rule tests?")? {
-    let test_dirs = arg.ask_dir_and_create("Where do you want to have your tests?", "rule-test")?;
+    let test_dirs =
+      arg.ask_dir_and_create("Where do you want to have your tests?", "rule-tests")?;
     Some(TestConfig::from(test_dirs))
   } else {
     None
   };
   let utils = if arg.confirm("Do you want to create folder for utility rules?")? {
     let util_dirs = arg.ask_dir_and_create("Where do you want to have your utilities?", "utils")?;
     Some(util_dirs)
```

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/print/colored_print.rs` & `ast_grep_cli-0.9.2/crates/cli/src/print/colored_print.rs`

 * *Files 1% similar despite different names*

```diff
@@ -301,27 +301,27 @@
       styles.push_matched_to_ret(&mut ret, &display.matched)?;
       continue;
     }
     ret.push_str(merger.last_trailing);
     let lines = ret.lines().count();
     let mut num = merger.last_start_line;
     let width = (lines + num).to_string().chars().count();
-    write!(writer, "{num:>width$}:")?; // initial line num
+    write!(writer, "{num:>width$}│")?; // initial line num
     print_highlight(ret.lines(), width, &mut num, writer)?;
     writeln!(writer)?; // end match new line
                        //
     merger.conclude_match(&nm);
     ret = display.leading.to_string();
     styles.push_matched_to_ret(&mut ret, &display.matched)?;
   }
   ret.push_str(merger.last_trailing);
   let lines = ret.lines().count();
   let mut num = merger.last_start_line;
   let width = (lines + num).to_string().chars().count();
-  write!(writer, "{num:>width$}:")?; // initial line num
+  write!(writer, "{num:>width$}│")?; // initial line num
   print_highlight(ret.lines(), width, &mut num, writer)?;
   writeln!(writer)?; // end match new line
   writeln!(writer)?; // end
   Ok(())
 }
 
 fn print_matches_with_prefix<'a, W: WriteColor>(
@@ -405,15 +405,15 @@
 ) -> Result<()> {
   if let Some(line) = lines.next() {
     write!(writer, "{line}")?;
   }
   for line in lines {
     writeln!(writer)?;
     *num += 1;
-    write!(writer, "{num:>width$}:{line}")?;
+    write!(writer, "{num:>width$}│{line}")?;
   }
   Ok(())
 }
 
 fn index_display(index: Option<usize>, style: Style, width: usize) -> impl Display {
   let index_str = match index {
     None => format!("{:width$}", ""),
@@ -454,15 +454,15 @@
         let (sign, s, em) = match change.tag() {
           ChangeTag::Delete => ("-", styles.delete, styles.delete_emphasis),
           ChangeTag::Insert => ("+", styles.insert, styles.insert_emphasis),
           ChangeTag::Equal => (" ", Style::new(), Style::new()),
         };
         write!(
           writer,
-          "{} {}:{}",
+          "{} {}│{}",
           index_display(change.old_index(), s, old_width),
           index_display(change.new_index(), s, new_width),
           s.paint(sign),
         )?;
         for (emphasized, value) in change.iter_strings_lossy() {
           if emphasized {
             write!(writer, "{}", em.paint(value))?;
@@ -690,15 +690,15 @@
       let printer = make_test_printer().heading(Heading::Always);
       let grep = SgLang::from(SupportLang::Tsx).ast_grep(source);
       let matches = grep.root().find_all(pattern);
       printer.print_matches(matches, "test.tsx".as_ref()).unwrap();
       let expected: String = source
         .lines()
         .enumerate()
-        .map(|(i, l)| format!("{}:{l}\n", i + 1))
+        .map(|(i, l)| format!("{}│{l}\n", i + 1))
         .collect();
       // append heading to expected
       let output = format!("test.tsx\n{expected}\n");
       assert_eq!(get_text(&printer), output, "{note}");
     }
   }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/print/interactive_print.rs` & `ast_grep_cli-0.9.2/crates/cli/src/print/interactive_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/print/json_print.rs` & `ast_grep_cli-0.9.2/crates/cli/src/print/json_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/print/mod.rs` & `ast_grep_cli-0.9.2/crates/cli/src/print/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+mod cloud_print;
 mod colored_print;
 mod interactive_print;
 mod json_print;
 
 use crate::lang::SgLang;
 use ast_grep_config::RuleConfig;
 use ast_grep_core::replacer::Fixer;
@@ -9,14 +10,15 @@
 
 use anyhow::Result;
 use clap::ValueEnum;
 
 use std::borrow::Cow;
 use std::path::Path;
 
+pub use cloud_print::{CloudPrinter, Platform};
 pub use codespan_reporting::files::SimpleFile;
 pub use codespan_reporting::term::termcolor::ColorChoice;
 pub use colored_print::{print_diff, ColoredPrinter, Heading, PrintStyles, ReportStyle};
 pub use interactive_print::InteractivePrinter;
 pub use json_print::JSONPrinter;
 
 type NodeMatch<'a, L> = SgNodeMatch<'a, StrDoc<L>>;
```

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/run.rs` & `ast_grep_cli-0.9.2/crates/cli/src/run.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/scan.rs` & `ast_grep_cli-0.9.2/crates/cli/src/scan.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 use clap::Args;
 use ignore::WalkParallel;
 
 use crate::config::{find_rules, read_rule_file, register_custom_language, IgnoreFile, NoIgnore};
 use crate::error::ErrorContext as EC;
 use crate::lang::SgLang;
 use crate::print::{
-  ColorArg, ColoredPrinter, Diff, InteractivePrinter, JSONPrinter, Printer, ReportStyle, SimpleFile,
+  CloudPrinter, ColorArg, ColoredPrinter, Diff, InteractivePrinter, JSONPrinter, Platform, Printer,
+  ReportStyle, SimpleFile,
 };
 use crate::utils::filter_file_interactive;
 use crate::utils::{is_from_stdin, run_std_in, StdInWorker};
 use crate::utils::{run_worker, Items, Worker};
 
 type AstGrep = ast_grep_core::AstGrep<StrDoc<SgLang>>;
 
@@ -26,21 +27,24 @@
   config: Option<PathBuf>,
 
   /// Scan the codebase with one specified rule, without project config setup.
   #[clap(short, long, conflicts_with = "config")]
   rule: Option<PathBuf>,
 
   /// Start interactive edit session. Code rewrite only happens inside a session.
-  #[clap(short, long, conflicts_with = "json")]
+  #[clap(short, long, conflicts_with = "json", conflicts_with = "format")]
   interactive: bool,
 
   /// Controls output color.
   #[clap(long, default_value = "auto")]
   color: ColorArg,
 
+  #[clap(short, long, conflicts_with = "json")]
+  format: Option<Platform>,
+
   #[clap(long, default_value = "rich")]
   report_style: ReportStyle,
 
   /// Output matches in structured JSON text. This is useful for tools like jq.
   /// Conflicts with color and report-style.
   #[clap(long, conflicts_with = "color", conflicts_with = "report_style")]
   json: bool,
@@ -67,14 +71,18 @@
 
 pub fn run_with_config(arg: ScanArg) -> Result<()> {
   register_custom_language(arg.config.clone());
   if arg.json {
     let printer = JSONPrinter::stdout();
     return run_scan(arg, printer);
   }
+  if let Some(_format) = &arg.format {
+    let printer = CloudPrinter::stdout();
+    return run_scan(arg, printer);
+  }
   let printer = ColoredPrinter::stdout(arg.color).style(arg.report_style);
   let interactive = arg.interactive || arg.update_all;
   if interactive {
     let from_stdin = arg.stdin && is_from_stdin();
     let printer = InteractivePrinter::new(printer, arg.update_all, from_stdin)?;
     run_scan(arg, printer)
   } else {
@@ -345,11 +353,12 @@
       color: ColorArg::Never,
       no_ignore: vec![],
       interactive: false,
       json: false,
       update_all: false,
       paths: vec![PathBuf::from(".")],
       stdin: false,
+      format: None,
     };
     assert!(run_with_config(arg).is_ok());
   }
 }
```

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/utils.rs` & `ast_grep_cli-0.9.2/crates/cli/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/crates/cli/src/verify.rs` & `ast_grep_cli-0.9.2/crates/cli/src/verify.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/crates/cli/tests/common/mod.rs` & `ast_grep_cli-0.9.2/crates/cli/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/crates/cli/tests/run_test.rs` & `ast_grep_cli-0.9.2/crates/cli/tests/run_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/crates/cli/tests/scan_test.rs` & `ast_grep_cli-0.9.2/crates/cli/tests/scan_test.rs`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 use predicates::str::contains;
 use tempdir::TempDir;
 
 const CONFIG: &str = "
 ruleDirs:
 - rules
 testConfigs:
-- testDir: rule-test
+- testDir: rule-tests
 ";
 const RULE1: &str = "
 id: on-rule
 message: test rule
 severity: warning
 language: TypeScript
 rule:
```

### Comparing `ast_grep_cli-0.9.1/crates/cli/tests/verify_test.rs` & `ast_grep_cli-0.9.2/crates/cli/tests/verify_test.rs`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 use common::create_test_files;
 use tempdir::TempDir;
 
 const CONFIG: &str = "
 ruleDirs:
 - rules
 testConfigs:
-- testDir: rule-test
+- testDir: rule-tests
 ";
 const RULE: &str = "
 id: test-rule
 message: test rule
 severity: warning
 language: TypeScript
 rule:
@@ -28,15 +28,15 @@
 - Some(123)
 ";
 
 fn setup() -> Result<TempDir> {
   let dir = create_test_files([
     ("sgconfig.yml", CONFIG),
     ("rules/test-rule.yml", RULE),
-    ("rule-test/test-rule-test.yml", TEST),
+    ("rule-tests/test-rule-test.yml", TEST),
     ("test.ts", "Some(123)"),
   ])?;
   assert!(dir.path().join("sgconfig.yml").exists());
   Ok(dir)
 }
 
 fn sg(s: &str) -> Result<()> {
```

### Comparing `ast_grep_cli-0.9.1/pyproject.toml` & `ast_grep_cli-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-cli"
-version = "0.9.1"
+version = "0.9.2"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_cli-0.9.1/crates/cli/Cargo.lock` & `ast_grep_cli-0.9.2/crates/cli/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -122,15 +122,15 @@
  "similar",
  "tempdir",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "serde",
@@ -138,77 +138,78 @@
  "tempdir",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "libloading 0.8.0",
  "serde",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
 name = "ast-grep-language"
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
  "ast-grep-core",
  "ast-grep-tree-sitter-c-sharp",
  "ignore",
  "serde",
  "tree-sitter-c",
  "tree-sitter-cpp",
  "tree-sitter-css",
  "tree-sitter-dart",
  "tree-sitter-go",
  "tree-sitter-html",
  "tree-sitter-java",
  "tree-sitter-javascript",
+ "tree-sitter-json",
  "tree-sitter-kotlin",
  "tree-sitter-lua",
  "tree-sitter-python",
  "tree-sitter-ruby",
  "tree-sitter-rust",
  "tree-sitter-scala",
  "tree-sitter-swift",
  "tree-sitter-thrift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "dashmap",
  "serde",
  "serde_json",
  "tower-lsp",
 ]
 
 [[package]]
 name = "ast-grep-napi"
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
@@ -269,15 +270,15 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "benches"
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
 
@@ -374,28 +375,28 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.12"
+version = "4.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3eab9e8ceb9afdade1ab3f0fd8dbce5b1b2f468ad653baf10e771781b2b67b73"
+checksum = "5fd304a20bff958a57f04c4e96a2e7594cc4490a0e809cbd48bb6437edaa452d"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.12"
+version = "4.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f2763db829349bf00cfc06251268865ed4363b93a943174f638daf3ecdba2cd"
+checksum = "01c6a3f08f1fe5662a35cfe393aec09c4df95f60ee93b7556505260f75eee9e1"
 dependencies = [
  "anstream",
  "anstyle",
  "clap_lex",
  "strsim",
 ]
 
@@ -1455,17 +1456,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.98",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.9.23"
+version = "0.9.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da6075b41c7e3b079e5f246eb6094a44850d3a4c25a67c581c80796c80134012"
+checksum = "1a49e178e4452f45cb61d0cd8cebc1b0fafd3e41929e996cef79aa3aca91f574"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
@@ -1572,26 +1573,26 @@
 name = "termtree"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95059e91184749cb66be6dc994f67f182b6d897cb3df74a5bf66b5e709295fd8"
 
 [[package]]
 name = "thiserror"
-version = "1.0.43"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
+checksum = "611040a08a0439f8248d1990b111c95baa9c704c805fa1f62104b39655fd7f90"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.43"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
+checksum = "090198534930841fab3a5d1bb637cde49e339654e606195f8d9c76eeb081dc96"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.23",
 ]
 
 [[package]]
@@ -1771,27 +1772,27 @@
 dependencies = [
  "cc",
  "regex",
 ]
 
 [[package]]
 name = "tree-sitter-c"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cca211f4827d4b4dc79f388bf67b6fa3bc8a8cfa642161ef24f99f371ba34c7b"
+checksum = "4dc4f11ece4d78d5a62591fe2456e9ca76211f0a60939913852ff6dfa023cb07"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-cpp"
-version = "0.20.0"
+version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a869e3c5cef4e5db4e9ab16a8dc84d73010e60ada14cdc60d2f6d8aed17779d"
+checksum = "0dbedbf4066bfab725b3f9e2a21530507419a7d2f98621d3c13213502b734ec0"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-css"
@@ -1863,14 +1864,24 @@
 checksum = "2490fab08630b2c8943c320f7b63473cbf65511c8d83aec551beb9b4375906ed"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
+name = "tree-sitter-json"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "90b04c4e1a92139535eb9fca4ec8fa9666cc96b618005d3ae35f3c957fa92f92"
+dependencies = [
+ "cc",
+ "tree-sitter",
+]
+
+[[package]]
 name = "tree-sitter-kotlin"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a69eb13ef18972f820d9a5c3989e3edfcbde227d89fdebce93904a99e3d5c7fc"
 dependencies = [
  "cc",
  "tree-sitter",
```

### Comparing `ast_grep_cli-0.9.1/README.md` & `ast_grep_cli-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/LICENSE` & `ast_grep_cli-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.1/PKG-INFO` & `ast_grep_cli-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ast-grep-cli
-Version: 0.9.1
+Version: 0.9.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.9.1 Classifier: Development
+Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.9.2 Classifier: Development
 Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Rust Classifier: Topic :: Security Classifier: Topic :: Software Development
 :: Quality Assurance Classifier: Topic :: Software Development Classifier:
 Topic :: Text Processing License-File: LICENSE License-File: LICENSE Summary:
 Structural Search and Rewrite code at large scale using precise AST pattern.
```

