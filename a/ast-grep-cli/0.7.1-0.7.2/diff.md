# Comparing `tmp/ast_grep_cli-0.7.1.tar.gz` & `tmp/ast_grep_cli-0.7.2.tar.gz`

## Comparing `ast_grep_cli-0.7.1.tar` & `ast_grep_cli-0.7.2.tar`

### file list

```diff
@@ -1,70 +1,71 @@
--rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/Cargo.toml
--rw-r--r--   0     1001      123     1911 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/cpp.rs
--rw-r--r--   0     1001      123     1815 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/csharp.rs
--rw-r--r--   0     1001      123     1515 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/css.rs
--rw-r--r--   0     1001      123     2024 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/go.rs
--rw-r--r--   0     1001      123     9828 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/lib.rs
--rw-r--r--   0     1001      123     2990 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/parsers.rs
--rw-r--r--   0     1001      123     3114 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/python.rs
--rw-r--r--   0     1001      123     2915 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/rust.rs
--rw-r--r--   0     1001      123     2041 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/scala.rs
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/Cargo.toml
--rw-r--r--   0     1001      123     2331 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/language.rs
--rw-r--r--   0     1001      123     3858 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/lib.rs
--rw-r--r--   0     1001      123    14850 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/match_tree.rs
--rw-r--r--   0     1001      123     3480 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/kind.rs
--rw-r--r--   0     1001      123     3783 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/node_match.rs
--rw-r--r--   0     1001      123    10723 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/pattern.rs
--rw-r--r--   0     1001      123      982 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/text.rs
--rw-r--r--   0     1001      123     6540 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher.rs
--rw-r--r--   0     1001      123    11359 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/meta_var.rs
--rw-r--r--   0     1001      123    15431 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/node.rs
--rw-r--r--   0     1001      123    16351 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/ops.rs
--rw-r--r--   0     1001      123     3089 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/pinned.rs
--rw-r--r--   0     1001      123    10936 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer/indent.rs
--rw-r--r--   0     1001      123     6181 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer/structural.rs
--rw-r--r--   0     1001      123     9380 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer/template.rs
--rw-r--r--   0     1001      123     2572 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer.rs
--rw-r--r--   0     1001      123     8489 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/source.rs
--rw-r--r--   0     1001      123    16414 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/traversal.rs
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/Cargo.toml
--rw-r--r--   0     1001      123     6946 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/constraints.rs
--rw-r--r--   0     1001      123     6838 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/deserialize_env.rs
--rw-r--r--   0     1001      123     4880 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/lib.rs
--rw-r--r--   0     1001      123     2765 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/maybe.rs
--rw-r--r--   0     1001      123     6514 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/referent_rule.rs
--rw-r--r--   0     1001      123    16160 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
--rw-r--r--   0     1001      123     4138 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
--rw-r--r--   0     1001      123    13151 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/rule.rs
--rw-r--r--   0     1001      123     6268 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/rule_collection.rs
--rw-r--r--   0     1001      123    11320 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/rule_config.rs
--rw-r--r--   0     1001      123     6716 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/transform.rs
--rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-dynamic/Cargo.toml
--rw-r--r--   0     1001      123     7730 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-dynamic/src/lib.rs
--rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-lsp/Cargo.toml
--rw-r--r--   0     1001      123    11291 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-lsp/src/lib.rs
--rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/crates/cli/Cargo.toml
--rw-r--r--   0     1001      123      249 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/bin/ast-grep.rs
--rw-r--r--   0     1001      123    11003 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/config.rs
--rw-r--r--   0     1001      123    10194 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/error.rs
--rw-r--r--   0     1001      123     4105 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/lang.rs
--rw-r--r--   0     1001      123     4996 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/lib.rs
--rw-r--r--   0     1001      123     1015 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/lsp.rs
--rw-r--r--   0     1001      123       94 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/main.rs
--rw-r--r--   0     1001      123    10196 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/new.rs
--rw-r--r--   0     1001      123    22465 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/print/colored_print.rs
--rw-r--r--   0     1001      123     7675 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/print/interactive_print.rs
--rw-r--r--   0     1001      123     9327 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/print/json_print.rs
--rw-r--r--   0     1001      123     3179 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/print/mod.rs
--rw-r--r--   0     1001      123     8602 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/run.rs
--rw-r--r--   0     1001      123    10361 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/scan.rs
--rw-r--r--   0     1001      123     6866 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/utils.rs
--rw-r--r--   0     1001      123    24629 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/verify.rs
--rw-r--r--   0     1001      123      593 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/tests/common/mod.rs
--rw-r--r--   0     1001      123      975 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/tests/run_test.rs
--rw-r--r--   0     1001      123     1046 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/tests/verify_test.rs
--rw-r--r--   0     1001      123     1236 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/pyproject.toml
--rw-r--r--   0     1001      123    60179 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/Cargo.lock
--rw-r--r--   0     1001      123     4980 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/README.md
--rw-r--r--   0     1001      123     1077 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/LICENSE
--rw-r--r--   0        0        0     6235 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-lsp/Cargo.toml
+-rw-r--r--   0     1001      123    11369 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-lsp/src/lib.rs
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/Cargo.toml
+-rw-r--r--   0     1001      123     2331 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/language.rs
+-rw-r--r--   0     1001      123     3858 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/lib.rs
+-rw-r--r--   0     1001      123    14850 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/match_tree.rs
+-rw-r--r--   0     1001      123     3480 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/kind.rs
+-rw-r--r--   0     1001      123     3783 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      123    11138 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      123      982 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/text.rs
+-rw-r--r--   0     1001      123     6540 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher.rs
+-rw-r--r--   0     1001      123    11359 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/meta_var.rs
+-rw-r--r--   0     1001      123    15431 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/node.rs
+-rw-r--r--   0     1001      123    16351 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/ops.rs
+-rw-r--r--   0     1001      123     3089 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/pinned.rs
+-rw-r--r--   0     1001      123    10936 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer/indent.rs
+-rw-r--r--   0     1001      123     6181 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer/structural.rs
+-rw-r--r--   0     1001      123     9380 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer/template.rs
+-rw-r--r--   0     1001      123     2572 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer.rs
+-rw-r--r--   0     1001      123     8489 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/source.rs
+-rw-r--r--   0     1001      123    16414 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/traversal.rs
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/Cargo.toml
+-rw-r--r--   0     1001      123     6946 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/constraints.rs
+-rw-r--r--   0     1001      123     6838 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/deserialize_env.rs
+-rw-r--r--   0     1001      123     4880 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/lib.rs
+-rw-r--r--   0     1001      123     2765 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/maybe.rs
+-rw-r--r--   0     1001      123     6514 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/referent_rule.rs
+-rw-r--r--   0     1001      123    16160 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
+-rw-r--r--   0     1001      123     4138 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
+-rw-r--r--   0     1001      123    13151 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/rule.rs
+-rw-r--r--   0     1001      123     6357 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/rule_collection.rs
+-rw-r--r--   0     1001      123    11610 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/rule_config.rs
+-rw-r--r--   0     1001      123     6716 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/transform.rs
+-rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-dynamic/Cargo.toml
+-rw-r--r--   0     1001      123     7730 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-dynamic/src/lib.rs
+-rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/Cargo.toml
+-rw-r--r--   0     1001      123     1911 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/cpp.rs
+-rw-r--r--   0     1001      123     1815 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/csharp.rs
+-rw-r--r--   0     1001      123     1515 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/css.rs
+-rw-r--r--   0     1001      123     2024 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/go.rs
+-rw-r--r--   0     1001      123    10142 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/lib.rs
+-rw-r--r--   0     1001      123     2990 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/parsers.rs
+-rw-r--r--   0     1001      123     3114 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/python.rs
+-rw-r--r--   0     1001      123     2915 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/rust.rs
+-rw-r--r--   0     1001      123     2041 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/scala.rs
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/crates/cli/Cargo.toml
+-rw-r--r--   0     1001      123      249 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/bin/ast-grep.rs
+-rw-r--r--   0     1001      123    11003 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/config.rs
+-rw-r--r--   0     1001      123    10194 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/error.rs
+-rw-r--r--   0     1001      123     4312 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/lang.rs
+-rw-r--r--   0     1001      123     4996 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/lib.rs
+-rw-r--r--   0     1001      123     1015 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/lsp.rs
+-rw-r--r--   0     1001      123       94 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/main.rs
+-rw-r--r--   0     1001      123    10205 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/new.rs
+-rw-r--r--   0     1001      123    22621 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/print/colored_print.rs
+-rw-r--r--   0     1001      123     7648 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/print/interactive_print.rs
+-rw-r--r--   0     1001      123     9327 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/print/json_print.rs
+-rw-r--r--   0     1001      123     3179 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/print/mod.rs
+-rw-r--r--   0     1001      123     9072 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/run.rs
+-rw-r--r--   0     1001      123    10673 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/scan.rs
+-rw-r--r--   0     1001      123     7418 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/utils.rs
+-rw-r--r--   0     1001      123    24629 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/verify.rs
+-rw-r--r--   0     1001      123      593 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/tests/common/mod.rs
+-rw-r--r--   0     1001      123      971 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/tests/run_test.rs
+-rw-r--r--   0     1001      123     1409 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/tests/scan_test.rs
+-rw-r--r--   0     1001      123     1025 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/tests/verify_test.rs
+-rw-r--r--   0     1001      123     1236 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/pyproject.toml
+-rw-r--r--   0     1001      123    60241 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/Cargo.lock
+-rw-r--r--   0     1001      123     4951 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/README.md
+-rw-r--r--   0     1001      123     1077 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/LICENSE
+-rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/PKG-INFO
```

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/Cargo.toml` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.7.1"
+version= "0.7.2"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 serde= { version = "1.0", features = ["derive"] }
```

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/cpp.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/csharp.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/css.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/css.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/go.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/lib.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/lib.rs`

 * *Files 13% similar despite different names*

```diff
@@ -44,25 +44,28 @@
 pub use css::Css;
 pub use go::Go;
 pub use python::Python;
 pub use rust::Rust;
 pub use scala::Scala;
 
 // Stub Language without preprocessing
+// Language Name, tree-sitter-name, alias, extension
 impl_lang!(C, language_c);
 impl_lang!(Dart, language_dart);
 impl_lang!(Html, language_html);
 impl_lang!(Java, language_java);
 impl_lang!(JavaScript, language_javascript);
 impl_lang!(Kotlin, language_kotlin);
 impl_lang!(Lua, language_lua);
 impl_lang!(Swift, language_swift);
 impl_lang!(Thrift, language_thrift);
 impl_lang!(Tsx, language_tsx);
 impl_lang!(TypeScript, language_typescript);
+// See ripgrep for extensions
+// https://github.com/BurntSushi/ripgrep/blob/master/crates/ignore/src/default_types.rs
 
 /// Represents all built-in languages.
 #[derive(Clone, Copy, Debug, PartialEq, Eq, Serialize, Hash)]
 pub enum SupportLang {
   C,
   Cpp,
   CSharp,
@@ -80,17 +83,17 @@
   Swift,
   Thrift,
   Tsx,
   TypeScript,
 }
 
 impl SupportLang {
-  pub fn all_langs() -> Vec<SupportLang> {
+  pub const fn all_langs() -> &'static [SupportLang] {
     use SupportLang::*;
-    vec![
+    &[
       C, Cpp, CSharp, Css, Dart, Go, Html, Java, JavaScript, Kotlin, Lua, Python, Rust, Scala,
       Swift, Thrift, Tsx, TypeScript,
     ]
   }
 
   pub fn file_types(&self) -> Types {
     file_types(self)
@@ -125,41 +128,50 @@
     D: Deserializer<'de>,
   {
     let s = String::deserialize(deserializer)?;
     FromStr::from_str(&s).map_err(de::Error::custom)
   }
 }
 
+const fn alias(lang: &SupportLang) -> &[&str] {
+  use SupportLang::*;
+  match lang {
+    C => &["c"],
+    Cpp => &["cc", "c++", "cpp", "cxx"],
+    CSharp => &["cs", "csharp"],
+    Css => &["css"],
+    Dart => &["dart"],
+    Go => &["go", "golang"],
+    Html => &["html"],
+    Java => &["java"],
+    JavaScript => &["javascript", "js", "jsx"],
+    Kotlin => &["kotlin", "kt"],
+    Lua => &["lua"],
+    Python => &["py", "python"],
+    Rust => &["rs", "rust"],
+    Scala => &["scala"],
+    Swift => &["swift"],
+    Thrift => &["thrift"],
+    TypeScript => &["ts", "typescript"],
+    Tsx => &["tsx"],
+  }
+}
+
 /// Implements the language names and aliases.
 impl FromStr for SupportLang {
   type Err = SupportLangErr;
   fn from_str(s: &str) -> Result<Self, Self::Err> {
-    use SupportLang::*;
-    let normalized = s.to_lowercase();
-    match normalized.as_str() {
-      "c" => Ok(C),
-      "cc" | "c++" | "cpp" | "cxx" => Ok(Cpp),
-      "cs" | "csharp" => Ok(CSharp),
-      "css" | "scss" => Ok(Css),
-      "dart" => Ok(Dart),
-      "go" | "golang" => Ok(Go),
-      "html" => Ok(Html),
-      "java" => Ok(Java),
-      "javascript" | "js" | "jsx" => Ok(JavaScript),
-      "kotlin" | "kt" | "ktm" | "kts" => Ok(Kotlin),
-      "lua" => Ok(Lua),
-      "py" | "python" => Ok(Python),
-      "rs" | "rust" => Ok(Rust),
-      "scala" => Ok(Scala),
-      "swift" => Ok(Swift),
-      "thrift" => Ok(Thrift),
-      "ts" | "typescript" => Ok(TypeScript),
-      "tsx" => Ok(Tsx),
-      _ => Err(SupportLangErr::LanguageNotSupported(s.to_string())),
+    for lang in Self::all_langs() {
+      for moniker in alias(lang) {
+        if s.eq_ignore_ascii_case(moniker) {
+          return Ok(*lang);
+        }
+      }
     }
+    Err(SupportLangErr::LanguageNotSupported(s.to_string()))
   }
 }
 
 macro_rules! execute_lang_method {
   ($me: path, $method: ident, $($pname:tt),*) => {
     use SupportLang as S;
     match $me {
@@ -205,40 +217,47 @@
   impl_lang_method!(extract_meta_var, (source: &str) => Option<MetaVariable>);
 
   fn pre_process_pattern<'q>(&self, query: &'q str) -> Cow<'q, str> {
     execute_lang_method! { self, pre_process_pattern, query }
   }
 }
 
+fn extensions(lang: &SupportLang) -> &[&str] {
+  use SupportLang::*;
+  match lang {
+    C => &["c", "h"],
+    Cpp => &["cc", "hpp", "cpp", "c++", "hh", "cxx", "cu", "ino"],
+    CSharp => &["cs"],
+    Css => &["css", "scss"],
+    Dart => &["dart"],
+    Go => &["go"],
+    Html => &["html", "htm", "xhtml"],
+    Java => &["java"],
+    JavaScript => &["cjs", "js", "mjs", "jsx"],
+    Kotlin => &["kt", "ktm", "kts"],
+    Lua => &["lua"],
+    Python => &["py", "py3", "pyi", "bzl"],
+    Rust => &["rs"],
+    Scala => &["scala", "sc", "sbt"],
+    Swift => &["swift"],
+    Thrift => &["thrift"],
+    TypeScript => &["ts", "cts", "mts"],
+    Tsx => &["tsx"],
+  }
+}
+
 /// Guess which programming language a file is written in
 /// Adapt from `<https://github.com/Wilfred/difftastic/blob/master/src/parse/guess_language.rs>`
 /// N.B do not confuse it with `FromStr` trait. This function is to guess language from file extension.
 fn from_extension(path: &Path) -> Option<SupportLang> {
-  use SupportLang::*;
-  match path.extension()?.to_str()? {
-    "c" | "h" => Some(C),
-    "cc" | "hpp" | "cpp" | "c++" | "hh" | "cxx" | "cu" | "ino" => Some(Cpp),
-    "cs" => Some(CSharp),
-    "css" | "scss" => Some(Css),
-    "dart" => Some(Dart),
-    "go" => Some(Go),
-    "html" | "htm" | "xhtml" => Some(Html),
-    "java" => Some(Java),
-    "cjs" | "js" | "mjs" | "jsx" => Some(JavaScript),
-    "kt" | "ktm" | "kts" => Some(Kotlin),
-    "lua" => Some(Lua),
-    "py" | "py3" | "pyi" | "bzl" => Some(Python),
-    "rs" => Some(Rust),
-    "scala" | "sc" | "sbt" => Some(Scala),
-    "swift" => Some(Swift),
-    "thrift" => Some(Thrift),
-    "ts" | "cts" | "mts" => Some(TypeScript),
-    "tsx" => Some(Tsx),
-    _ => None,
-  }
+  let ext = path.extension()?.to_str()?;
+  SupportLang::all_langs()
+    .iter()
+    .copied()
+    .find(|l| extensions(l).contains(&ext))
 }
 
 fn add_custom_file_type<'b>(
   builder: &'b mut TypesBuilder,
   file_type: &str,
   suffix_list: &[&str],
 ) -> &'b mut TypesBuilder {
```

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/parsers.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/parsers.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/python.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/rust.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/rust.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/scala.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/scala.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/Cargo.toml` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 edition= "2021"
 homepage= "https://ast-grep.github.io/"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.7.1"
+version= "0.7.2"
 
 [dependencies]
 bit-set= { version = "0.5.3" }
-regex = { version = "1.8.4" , optional = true }
-thiserror= "1.0.40"
+regex = { version = "1.9.1" , optional = true }
+thiserror= "1.0.43"
 tree-sitter= { version = "0.9.2", package = "tree-sitter-facade-sg" }
 
 [features]
 default = ["regex"]
```

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/language.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/lib.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/match_tree.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/match_tree.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/kind.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/node_match.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/pattern.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/pattern.rs`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,28 @@
     _ => false,
   }
 }
 impl<L: Language> Pattern<StrDoc<L>> {
   pub fn str(src: &str, lang: L) -> Self {
     Self::new(src, lang)
   }
+
+  pub fn fixed_string(&self) -> Cow<str> {
+    let node = match &self.style {
+      PatternStyle::Single => self.single_matcher(),
+      PatternStyle::Selector(kind) => self.kind_matcher(kind),
+    };
+    let mut fixed = Cow::Borrowed("");
+    for n in node.dfs() {
+      if n.is_leaf() && extract_var_from_node(&n).is_none() && n.text().len() > fixed.len() {
+        fixed = n.text();
+      }
+    }
+    fixed
+  }
 }
 
 impl<D: Doc> Pattern<D> {
   pub fn try_new(src: &str, lang: D::Lang) -> Result<Self, PatternError> {
     let processed = lang.pre_process_pattern(src);
     let root = Root::try_new(&processed, lang)?;
     let goal = root.root();
```

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/text.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/meta_var.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/meta_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/node.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/ops.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/pinned.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer/indent.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer/structural.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer/template.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/source.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/traversal.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/Cargo.toml` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.7.1"
+version= "0.7.2"
 
 [features]
 default = ["regex"]
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 anyhow = "1.0"
 bit-set= { version = "0.5.3" }
 globset = "0.4.10"
-regex = { version = "1.8.4" , optional = true }
+regex = { version = "1.9.1" , optional = true }
 serde= { version = "1.0", features = ["derive"] }
 serde_yaml = "0.9.22"
-thiserror= "1.0.40"
+thiserror= "1.0.43"
```

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/constraints.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/constraints.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/deserialize_env.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/lib.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/maybe.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/referent_rule.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/relational_rule/mod.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/relational_rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/rule.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/rule_collection.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/rule_collection.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::RuleConfig;
+use crate::{RuleConfig, Severity};
 use ast_grep_core::language::Language;
 use globset::{Glob, GlobSet, GlobSetBuilder};
 use std::path::Path;
 
 /// RuleBucket stores rules of the same language id.
 /// Rules for different language will stay in separate buckets.
 pub struct RuleBucket<L: Language> {
@@ -78,15 +78,17 @@
 }
 
 impl<L: Language + Eq> RuleCollection<L> {
   pub fn try_new(configs: Vec<RuleConfig<L>>) -> Result<Self, globset::Error> {
     let mut tenured = vec![];
     let mut contingent = vec![];
     for config in configs {
-      if config.files.is_none() && config.ignores.is_none() {
+      if matches!(config.severity, Severity::Off) {
+        continue;
+      } else if config.files.is_none() && config.ignores.is_none() {
         Self::add_tenured_rule(&mut tenured, config);
       } else {
         contingent.push(ContingentRule::try_from(config)?);
       }
     }
     Ok(Self {
       tenured,
```

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/rule_config.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/rule_config.rs`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,24 @@
 
 // type Pattern<L> = PatternCore<StrDoc<L>>;
 
 #[derive(Serialize, Deserialize, Clone, Default)]
 #[serde(rename_all = "camelCase")]
 pub enum Severity {
   #[default]
+  /// A kind reminder for code with potential improvement.
   Hint,
+  /// A suggestion that code can be improved or optimized.
   Info,
+  /// A warning that code might produce bugs or does not follow best practice.
   Warning,
+  /// An error that code produces bugs or has logic errors.
   Error,
+  /// Turns off the rule.
+  Off,
 }
 
 #[derive(Serialize, Deserialize, Clone)]
 pub struct SerializableRuleCore<L: Language> {
   /// Specify the language to parse and the file extension to includ in matching.
   pub language: L,
   /// Pattern rules to find matching AST nodes
```

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/transform.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/transform.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-dynamic/Cargo.toml` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-dynamic/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.7.1"
+version= "0.7.2"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 libloading = "0.8"
 serde= { version = "1.0", features = ["derive"] }
-thiserror= "1.0.40"
+thiserror= "1.0.43"
 tree-sitter-native = { version = "0.20.10", package = "tree-sitter" }
```

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-dynamic/src/lib.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-dynamic/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-lsp/Cargo.toml` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-lsp/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [package]
 name = "ast-grep-lsp"
 description = "Search and Rewrite code at large scale using precise AST pattern"
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
-version= "0.7.1"
+version= "0.7.2"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 ast-grep-config.path = "../ast-grep-config"
 
 dashmap = "5.4.0"
 serde= { version = "1.0", features = ["derive"] }
-serde_json = "1.0.99"
+serde_json = "1.0.100"
 tower-lsp = "0.19.0"
```

### Comparing `ast_grep_cli-0.7.1/local_dependencies/ast-grep-lsp/src/lib.rs` & `ast_grep_cli-0.7.2/local_dependencies/ast-grep-lsp/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,15 @@
     code: Some(NumberOrString::String(rule.id.clone())),
     code_description: url_to_code_description(&rule.url),
     severity: Some(match rule.severity {
       Severity::Error => DiagnosticSeverity::ERROR,
       Severity::Warning => DiagnosticSeverity::WARNING,
       Severity::Info => DiagnosticSeverity::INFORMATION,
       Severity::Hint => DiagnosticSeverity::HINT,
+      Severity::Off => unreachable!("turned-off rule should not have match"),
     }),
     message: rule.get_message(&node_match),
     source: Some(String::from("ast-grep")),
     tags: None,
     related_information: collect_labels(&node_match, uri),
     data: None,
   }
```

### Comparing `ast_grep_cli-0.7.1/crates/cli/Cargo.toml` & `ast_grep_cli-0.7.2/crates/cli/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 categories = ["command-line-utilities", "development-tools", "parsing"]
 default-run = "sg"
 # use relative path because maturin does not recognize
 readme = "../../README.md"
 license-file = "../../LICENSE"
 
-version= "0.7.1"
+version= "0.7.2"
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
-clap = { version = "4.3.8", features = ["derive"] }
+clap = { version = "4.3.11", features = ["derive"] }
 codespan-reporting = "0.11.1"
 crossterm = "0.26.1"
 ignore= { version = "0.4.20" }
 inquire = "0.6.2"
-num_cpus = "1.15.0"
+num_cpus = "1.16.0"
 serde= { version = "1.0", features = ["derive"] }
-serde_json = "1.0.99"
+serde_json = "1.0.100"
 serde_yaml = "0.9.22"
 similar = { version = "2.2.1", features = ["inline"] }
 tokio = { version = "1", features = ["rt-multi-thread", "io-std"] }
```

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/config.rs` & `ast_grep_cli-0.7.2/crates/cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/error.rs` & `ast_grep_cli-0.7.2/crates/cli/src/error.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/lang.rs` & `ast_grep_cli-0.7.2/crates/cli/src/lang.rs`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
       .map(|(name, custom)| custom_lang_to_registration(name, custom, &base))
       .collect();
     // TODO, add error handling
     unsafe { DynamicLang::register(registrations).expect("TODO") }
   }
 
   pub fn all_langs() -> Vec<Self> {
-    let builtin = SupportLang::all_langs().into_iter().map(Self::Builtin);
+    let builtin = SupportLang::all_langs().iter().copied().map(Self::Builtin);
     let customs = DynamicLang::all_langs().into_iter().map(Self::Custom);
     builtin.chain(customs).collect()
   }
 }
 
 impl Debug for SgLang {
   fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
@@ -73,14 +73,23 @@
     symbol: sym,
     meta_var_char: custom_lang.meta_var_char,
     expando_char: custom_lang.expando_char,
     extensions: custom_lang.extensions,
   }
 }
 
+impl Display for SgLang {
+  fn fmt(&self, f: &mut Formatter) -> std::fmt::Result {
+    match self {
+      Builtin(b) => write!(f, "{:?}", b),
+      Custom(c) => write!(f, "{:?}", c.name()),
+    }
+  }
+}
+
 #[derive(Debug)]
 pub enum SgLangErr {
   LanguageNotSupported(String),
 }
 
 impl Display for SgLangErr {
   fn fmt(&self, f: &mut Formatter<'_>) -> Result<(), std::fmt::Error> {
```

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/lib.rs` & `ast_grep_cli-0.7.2/crates/cli/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/lsp.rs` & `ast_grep_cli-0.7.2/crates/cli/src/lsp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/new.rs` & `ast_grep_cli-0.7.2/crates/cli/src/new.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use crate::config::{read_config_from_dir, register_custom_language, AstGrepConfig, TestConfig};
 use crate::error::ErrorContext as EC;
+use crate::lang::SgLang;
 
 use anyhow::Result;
-use ast_grep_language::SupportLang;
 use clap::{Parser, Subcommand};
 use inquire::validator::ValueRequiredValidator;
 
 use std::fmt::Display;
 use std::fs::{self, File};
 use std::path::PathBuf;
 
@@ -16,15 +16,15 @@
   #[clap(subcommand)]
   entity: Option<Entity>,
   /// The id of the item to create.
   #[arg(value_parser, global = true)]
   name: Option<String>,
   /// The language of the item. Appliable to rule and utils.
   #[arg(short, long, global = true)]
-  lang: Option<SupportLang>,
+  lang: Option<SgLang>,
   /// Accept all default options without interactive input during creation.
   #[arg(short, long, global = true)]
   yes: bool,
   #[arg(short, long, global = true, default_value = ".")]
   base_dir: PathBuf,
 }
 
@@ -60,22 +60,22 @@
         vec![Entity::Rule, Entity::Test, Entity::Util],
       )
       .prompt()?;
       Ok(entity)
     }
   }
 
-  fn choose_language(&self) -> Result<SupportLang> {
+  fn choose_language(&self) -> Result<SgLang> {
     if self.yes {
       self
         .lang
         .map(Ok)
         .unwrap_or_else(|| Err(anyhow::anyhow!(EC::InsufficientCLIArgument("lang"))))
     } else {
-      Ok(inquire::Select::new("Choose rule's language", SupportLang::all_langs()).prompt()?)
+      Ok(inquire::Select::new("Choose rule's language", SgLang::all_langs()).prompt()?)
     }
   }
 
   fn ask_name(&self, entity: &'static str) -> Result<String> {
     if let Some(name) = &self.name {
       Ok(name.to_string())
     } else if self.yes {
@@ -183,15 +183,15 @@
   let config_path = arg.base_dir.join("sgconfig.yml");
   let f = File::create(config_path)?;
   serde_yaml::to_writer(f, &root_config)?;
   println!("Your new ast-grep project has been created!");
   Ok(())
 }
 
-fn default_rule(id: &str, lang: SupportLang) -> String {
+fn default_rule(id: &str, lang: SgLang) -> String {
   format!(
     r#"id: {id}
 message: Add your rule message here....
 severity: error # error, warning, hint, info
 language: {lang}
 rule:
   pattern: Your Rule Pattern here...
@@ -263,15 +263,15 @@
     return Err(anyhow::anyhow!(EC::FileAlreadyExist(path)));
   }
   fs::write(&path, default_test(&name))?;
   println!("Created test at {}", path.display());
   Ok(())
 }
 
-fn default_util(id: &str, lang: SupportLang) -> String {
+fn default_util(id: &str, lang: SgLang) -> String {
   format!(
     r#"id: {id}
 language: {lang}
 rule:
   pattern: Your Rule Pattern here...
 # utils: Extract repeated rule as local utility here."#
   )
@@ -304,14 +304,15 @@
   println!("Created util at {}", path.display());
   Ok(())
 }
 
 #[cfg(test)]
 mod test {
   use super::*;
+  use ast_grep_language::SupportLang;
   use std::path::Path;
   use tempdir::TempDir;
 
   fn create_project(tempdir: &Path) -> Result<()> {
     let arg = NewArg {
       entity: None,
       name: None,
@@ -324,15 +325,15 @@
     Ok(())
   }
 
   fn create_rule(temp: &Path) -> Result<()> {
     let arg = NewArg {
       entity: Some(Entity::Rule),
       name: Some("test-rule".into()),
-      lang: Some(SupportLang::Rust),
+      lang: Some(SupportLang::Rust.into()),
       yes: true,
       base_dir: temp.to_path_buf(),
     };
     run_create_new(arg).unwrap();
     assert!(temp.join("rules/test-rule.yml").exists());
     Ok(())
   }
```

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/print/colored_print.rs` & `ast_grep_cli-0.7.2/crates/cli/src/print/colored_print.rs`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     let config = &self.config;
     let mut writer = self.writer.lock().expect("should not fail");
     let serverity = match rule.severity {
       Severity::Error => diagnostic::Severity::Error,
       Severity::Warning => diagnostic::Severity::Warning,
       Severity::Info => diagnostic::Severity::Note,
       Severity::Hint => diagnostic::Severity::Help,
+      Severity::Off => unreachable!("turned-off rule should not have match."),
     };
     for m in matches {
       let range = m.range();
       let mut labels = vec![Label::primary((), range)];
       if let Some(secondary_nodes) = m.get_env().get_labels("secondary") {
         labels.extend(secondary_nodes.iter().map(|n| {
           let range = n.range();
@@ -174,14 +175,15 @@
   writer: &mut W,
 ) -> Result<()> {
   let (level, level_style) = match rule.severity {
     Severity::Error => ("error", style.error),
     Severity::Warning => ("warning", style.warning),
     Severity::Info => ("note", style.info),
     Severity::Hint => ("help", style.hint),
+    Severity::Off => unreachable!("turned-off rule should not have match."),
   };
   let header = format!("{level}[{}]:", &rule.id);
   let header = level_style.paint(header);
   let message = style.message.paint(&rule.message);
   writeln!(writer, "{header} {message}")?;
   Ok(())
 }
```

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/print/interactive_print.rs` & `ast_grep_cli-0.7.2/crates/cli/src/print/interactive_print.rs`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 pub struct InteractivePrinter<P: Printer> {
   accept_all: AtomicBool,
   from_stdin: bool,
   inner: P,
 }
 
 impl<P: Printer> InteractivePrinter<P> {
-  pub fn new(inner: P, accept_all: bool) -> Result<Self> {
-    let from_stdin = utils::is_from_stdin();
+  pub fn new(inner: P, accept_all: bool, from_stdin: bool) -> Result<Self> {
     if from_stdin && !accept_all {
       Err(anyhow::anyhow!(EC::StdInIsNotInteractive))
     } else {
       Ok(Self {
         accept_all: AtomicBool::new(accept_all),
         from_stdin,
         inner,
```

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/print/json_print.rs` & `ast_grep_cli-0.7.2/crates/cli/src/print/json_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/print/mod.rs` & `ast_grep_cli-0.7.2/crates/cli/src/print/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/run.rs` & `ast_grep_cli-0.7.2/crates/cli/src/run.rs`

 * *Files 9% similar despite different names*

```diff
@@ -10,36 +10,37 @@
 
 use crate::config::{register_custom_language, IgnoreFile, NoIgnore};
 use crate::error::ErrorContext as EC;
 use crate::lang::SgLang;
 use crate::print::{
   ColorArg, ColoredPrinter, Diff, Heading, InteractivePrinter, JSONPrinter, Printer,
 };
-use crate::utils::{filter_file_interactive, is_from_stdin, MatchUnit};
+use crate::utils::{filter_file_pattern, is_from_stdin, MatchUnit};
 use crate::utils::{run_std_in, StdInWorker};
 use crate::utils::{run_worker, Items, Worker};
 
 type Pattern<L> = SgPattern<StrDoc<L>>;
 
 // NOTE: have to register custom lang before clap read arg
 // RunArg has a field of SgLang
 pub fn register_custom_language_if_is_run(args: &[String]) {
   if !args.is_empty() || args[1].starts_with('-') || args[1] == "run" {
     register_custom_language(None);
   }
 }
 
-// TODO: add long_help
 fn lang_help() -> String {
   format!(
     "The language of the pattern. Supported languages are:\n{:?}",
     SgLang::all_langs()
   )
 }
 
+const LANG_HELP_LONG: &str = "The language of the pattern. For full language list, visit https://ast-grep.github.io/reference/languages.html";
+
 #[derive(Parser)]
 pub struct RunArg {
   /// AST pattern to match.
   #[clap(short, long)]
   pattern: String,
 
   /// String to replace the matched AST node.
@@ -47,15 +48,15 @@
   rewrite: Option<String>,
 
   /// Print query pattern's tree-sitter AST. Requires lang be set explicitly.
   #[clap(long, requires = "lang")]
   debug_query: bool,
 
   /// The language of the pattern query.
-  #[clap(short, long, help(lang_help()))]
+  #[clap(short, long, help(lang_help()), long_help=LANG_HELP_LONG)]
   lang: Option<SgLang>,
 
   /// Start interactive edit session. Code rewrite only happens inside a session.
   #[clap(short, long)]
   interactive: bool,
 
   /// The paths to search. You can provide multiple paths separated by spaces.
@@ -81,34 +82,42 @@
   #[clap(long, default_value = "auto")]
   color: ColorArg,
 
   /// Do not respect hidden file system or ignore files (.gitignore, .ignore, etc.).
   /// You can suppress multiple ignore files by passing `no-ignore` multiple times.
   #[clap(long, action = clap::ArgAction::Append)]
   no_ignore: Vec<IgnoreFile>,
+
+  /// Disable search code from StdIn.
+  ///
+  /// Use this if you need search files but ast-grep is launched from another process.
+  /// You can also use the environment variable `AST_GREP_NO_STDIN` to disable StdIn mode.
+  #[clap(long)]
+  no_stdin: bool,
 }
 
 // Every run will include Search or Replace
 // Search or Replace by arguments `pattern` and `rewrite` passed from CLI
 pub fn run_with_pattern(arg: RunArg) -> Result<()> {
   if arg.json {
     return run_pattern_with_printer(arg, JSONPrinter::stdout());
   }
   let printer = ColoredPrinter::stdout(arg.color).heading(arg.heading);
   let interactive = arg.interactive || arg.accept_all;
   if interactive {
-    let printer = InteractivePrinter::new(printer, arg.accept_all)?;
+    let from_stdin = !arg.no_stdin && is_from_stdin();
+    let printer = InteractivePrinter::new(printer, arg.accept_all, from_stdin)?;
     run_pattern_with_printer(arg, printer)
   } else {
     run_pattern_with_printer(arg, printer)
   }
 }
 
 fn run_pattern_with_printer(arg: RunArg, printer: impl Printer + Sync) -> Result<()> {
-  if is_from_stdin() {
+  if !arg.no_stdin && is_from_stdin() {
     run_std_in(RunWithSpecificLang::new(arg, printer)?)
   } else if arg.lang.is_some() {
     run_worker(RunWithSpecificLang::new(arg, printer)?)
   } else {
     run_worker(RunWithInferredLang { arg, printer })
   }
 }
@@ -128,15 +137,15 @@
       .threads(threads)
       .build_parallel()
   }
 
   fn produce_item(&self, path: &Path) -> Option<Self::Item> {
     let lang = SgLang::from_path(path)?;
     let matcher = Pattern::try_new(&self.arg.pattern, lang).ok()?;
-    let match_unit = filter_file_interactive(path, lang, matcher)?;
+    let match_unit = filter_file_pattern(path, lang, matcher)?;
     Some((match_unit, lang))
   }
 
   fn consume_items(&self, items: Items<Self::Item>) -> Result<()> {
     let rewrite = &self.arg.rewrite;
     let printer = &self.printer;
     printer.before_print()?;
@@ -190,15 +199,15 @@
       .types(lang.file_types())
       .build_parallel()
   }
   fn produce_item(&self, path: &Path) -> Option<Self::Item> {
     let arg = &self.arg;
     let pattern = self.pattern.clone();
     let lang = arg.lang.expect("must present");
-    filter_file_interactive(path, lang, pattern)
+    filter_file_pattern(path, lang, pattern)
   }
   fn consume_items(&self, items: Items<Self::Item>) -> Result<()> {
     let printer = &self.printer;
     printer.before_print()?;
     let arg = &self.arg;
     let lang = arg.lang.expect("must present");
     if arg.debug_query {
@@ -252,20 +261,20 @@
 
 #[cfg(test)]
 mod test {
   use super::*;
   use ast_grep_language::SupportLang;
   #[test]
   fn test_run_with_pattern() {
-    std::env::set_var("AST_GREP_ALWAYS_TTY", "1");
     let arg = RunArg {
       pattern: "console.log".to_string(),
       rewrite: None,
       color: ColorArg::Never,
       no_ignore: vec![],
+      no_stdin: true,
       interactive: false,
       lang: None,
       json: false,
       heading: Heading::Never,
       debug_query: false,
       accept_all: false,
       paths: vec![PathBuf::from(".")],
@@ -282,12 +291,13 @@
       no_ignore: vec![],
       interactive: false,
       lang: Some(SupportLang::Rust.into()),
       json: false,
       heading: Heading::Never,
       debug_query: false,
       accept_all: false,
+      no_stdin: false,
       paths: vec![PathBuf::from(".")],
     };
     assert!(run_with_pattern(arg).is_ok())
   }
 }
```

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/scan.rs` & `ast_grep_cli-0.7.2/crates/cli/src/scan.rs`

 * *Files 9% similar despite different names*

```diff
@@ -52,34 +52,42 @@
   /// The paths to search. You can provide multiple paths separated by spaces.
   #[clap(value_parser, default_value = ".")]
   paths: Vec<PathBuf>,
 
   /// Do not respect ignore files. You can suppress multiple ignore files by passing `no-ignore` multiple times.
   #[clap(long, action = clap::ArgAction::Append)]
   no_ignore: Vec<IgnoreFile>,
+
+  /// Disable search code from StdIn.
+  ///
+  /// Use this if you need search files but ast-grep is launched from another process.
+  /// You can also use the environment variable `AST_GREP_NO_STDIN` to disable StdIn mode.
+  #[clap(long)]
+  no_stdin: bool,
 }
 
 pub fn run_with_config(arg: ScanArg) -> Result<()> {
   register_custom_language(arg.config.clone());
   if arg.json {
     let printer = JSONPrinter::stdout();
     return run_scan(arg, printer);
   }
   let printer = ColoredPrinter::stdout(arg.color).style(arg.report_style);
   let interactive = arg.interactive || arg.accept_all;
   if interactive {
-    let printer = InteractivePrinter::new(printer, arg.accept_all)?;
+    let from_stdin = !arg.no_stdin && is_from_stdin();
+    let printer = InteractivePrinter::new(printer, arg.accept_all, from_stdin)?;
     run_scan(arg, printer)
   } else {
     run_scan(arg, printer)
   }
 }
 
 fn run_scan<P: Printer + Sync>(arg: ScanArg, printer: P) -> Result<()> {
-  if is_from_stdin() {
+  if !arg.no_stdin && is_from_stdin() {
     let worker = ScanWithRule::try_new(arg, printer)?;
     run_std_in(worker)
   } else {
     let worker = ScanWithConfig::try_new(arg, printer)?;
     run_worker(worker)
   }
 }
@@ -326,22 +334,22 @@
     let mut file = File::create(dir.path().join("rules/test.yml")).unwrap();
     file.write_all(RULE.as_bytes()).unwrap();
     let mut file = File::create(dir.path().join("test.rs")).unwrap();
     file
       .write_all("fn test() { Some(123) }".as_bytes())
       .unwrap();
     file.sync_all().unwrap();
-    std::env::set_var("AST_GREP_ALWAYS_TTY", "1");
     let arg = ScanArg {
       config: Some(dir.path().join("sgconfig.yml")),
       rule: None,
       report_style: ReportStyle::Rich,
       color: ColorArg::Never,
       no_ignore: vec![],
       interactive: false,
       json: false,
       accept_all: false,
       paths: vec![PathBuf::from(".")],
+      no_stdin: true,
     };
     assert!(run_with_config(arg).is_ok());
   }
 }
```

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/utils.rs` & `ast_grep_cli-0.7.2/crates/cli/src/utils.rs`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 use crossterm::{
   event::{self, Event, KeyCode},
   execute,
   terminal::{self, EnterAlternateScreen, LeaveAlternateScreen},
 };
 use ignore::{DirEntry, WalkParallel, WalkState};
 
+use ast_grep_core::Pattern;
 use ast_grep_core::{AstGrep, Matcher, StrDoc};
 use ast_grep_language::Language;
 
 use std::env;
 use std::fs::read_to_string;
 use std::io::stdout;
 use std::io::Write;
@@ -160,26 +161,51 @@
   if exit.success() {
     Ok(())
   } else {
     Err(anyhow!(EC::OpenEditor))
   }
 }
 
-pub fn filter_file_interactive<M: Matcher<SgLang>>(
-  path: &Path,
-  lang: SgLang,
-  matcher: M,
-) -> Option<MatchUnit<M>> {
+fn read_file(path: &Path) -> Option<String> {
   let file_content = read_to_string(path)
     .with_context(|| format!("Cannot read file {}", path.to_string_lossy()))
     .map_err(|err| eprintln!("{err}"))
     .ok()?;
   // skip large files or empty file
   if file_too_large(&file_content) || file_content.is_empty() {
     // TODO add output
+    None
+  } else {
+    Some(file_content)
+  }
+}
+
+pub fn filter_file_interactive<M: Matcher<SgLang>>(
+  path: &Path,
+  lang: SgLang,
+  matcher: M,
+) -> Option<MatchUnit<M>> {
+  let file_content = read_file(path)?;
+  let grep = lang.ast_grep(file_content);
+  let has_match = grep.root().find(&matcher).is_some();
+  has_match.then(|| MatchUnit {
+    grep,
+    path: path.to_path_buf(),
+    matcher,
+  })
+}
+
+pub fn filter_file_pattern(
+  path: &Path,
+  lang: SgLang,
+  matcher: Pattern<StrDoc<SgLang>>,
+) -> Option<MatchUnit<Pattern<StrDoc<SgLang>>>> {
+  let file_content = read_file(path)?;
+  let fixed = matcher.fixed_string();
+  if !fixed.is_empty() && !file_content.contains(&*fixed) {
     return None;
   }
   let grep = lang.ast_grep(file_content);
   let has_match = grep.root().find(&matcher).is_some();
   has_match.then(|| MatchUnit {
     grep,
     path: path.to_path_buf(),
@@ -214,19 +240,15 @@
   pub matcher: M,
 }
 
 #[inline]
 pub fn is_from_stdin() -> bool {
   // disable stdin if tty env presents or is_atty == true
   // env is used for testing purpose only
-  if cfg!(debug_assertions) {
-    env::var_os("AST_GREP_ALWAYS_TTY").is_none() && !atty::is(atty::Stream::Stdin)
-  } else {
-    !atty::is(atty::Stream::Stdin)
-  }
+  env::var_os("AST_GREP_NO_STDIN").is_none() && !atty::is(atty::Stream::Stdin)
 }
 
 #[cfg(test)]
 mod test {
   use super::*;
 
   #[test]
```

### Comparing `ast_grep_cli-0.7.1/crates/cli/src/verify.rs` & `ast_grep_cli-0.7.2/crates/cli/src/verify.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/crates/cli/tests/common/mod.rs` & `ast_grep_cli-0.7.2/crates/cli/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/crates/cli/tests/run_test.rs` & `ast_grep_cli-0.7.2/crates/cli/tests/run_test.rs`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 use predicates::prelude::*;
 use predicates::str::contains;
 
 #[test]
 fn test_simple_infer_lang() -> Result<()> {
   let dir = create_test_files([("a.ts", "console.log(123)"), ("b.rs", "console.log(456)")])?;
   Command::cargo_bin("sg")?
-    .env("AST_GREP_ALWAYS_TTY", "1")
+    .env("AST_GREP_NO_STDIN", "1")
     .current_dir(dir.path())
     .args(["-p", "console.log($A)"])
     .assert()
     .success()
     .stdout(contains("console.log(123)"))
     .stdout(contains("console.log(456)"));
   Ok(())
 }
 
 #[test]
 fn test_simple_specific_lang() -> Result<()> {
   let dir = create_test_files([("a.ts", "console.log(123)"), ("b.rs", "console.log(456)")])?;
   Command::cargo_bin("sg")?
-    .env("AST_GREP_ALWAYS_TTY", "1")
+    .env("AST_GREP_NO_STDIN", "1")
     .current_dir(dir.path())
     .args(["-p", "console.log($A)", "-l", "rs"])
     .assert()
     .success()
     .stdout(contains("console.log(123)").not())
     .stdout(contains("console.log(456)"));
   Ok(())
```

### Comparing `ast_grep_cli-0.7.1/crates/cli/tests/verify_test.rs` & `ast_grep_cli-0.7.2/crates/cli/tests/verify_test.rs`

 * *Files 10% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ("test.ts", "Some(123)"),
   ])?;
   assert!(dir.path().join("sgconfig.yml").exists());
   Ok(dir)
 }
 
 fn sg(s: &str) -> Result<()> {
-  println!("{}", s);
   let args = s.split(' ').map(String::from);
   main_with_args(args)
 }
 
 #[test]
 fn test_sg_test() -> Result<()> {
   let dir = setup()?;
```

### Comparing `ast_grep_cli-0.7.1/pyproject.toml` & `ast_grep_cli-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-cli"
-version = "0.7.1"
+version = "0.7.2"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_cli-0.7.1/crates/cli/Cargo.lock` & `ast_grep_cli-0.7.2/crates/cli/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -131,15 +131,15 @@
  "similar",
  "tempdir",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "serde",
@@ -147,38 +147,38 @@
  "tempdir",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.7.1"
+version = "0.7.2"
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
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "ast-grep-core",
  "ast-grep-tree-sitter-c-sharp",
  "ignore",
  "serde",
  "tree-sitter-c",
  "tree-sitter-cpp",
@@ -196,27 +196,27 @@
  "tree-sitter-swift",
  "tree-sitter-thrift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.7.1"
+version = "0.7.2"
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
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
@@ -277,15 +277,15 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "benches"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
 
@@ -320,15 +320,15 @@
 name = "bstr"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b45ea9b00a7b3f2988e9a65ad3917e62123c38dba709b666506207be96d1790b"
 dependencies = [
  "memchr",
  "once_cell",
- "regex-automata",
+ "regex-automata 0.1.10",
  "serde",
 ]
 
 [[package]]
 name = "bumpalo"
 version = "3.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -383,46 +383,45 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.8"
+version = "4.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9394150f5b4273a1763355bd1c2ec54cc5a2593f790587bcd6b2c947cfa9211"
+checksum = "1640e5cc7fb47dbb8338fd471b105e7ed6c3cb2aeb00c2e067127ffd3764a05d"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.8"
+version = "4.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a78fbdd3cc2914ddf37ba444114bc7765bbdcb55ec9cbe6fa054f0137400717"
+checksum = "98c59138d527eeaf9b53f35a77fcc1fad9d883116070c63d5de1c7dc7b00c72b"
 dependencies = [
  "anstream",
  "anstyle",
- "bitflags 1.3.2",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
 version = "4.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.10",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
@@ -575,15 +574,15 @@
 [[package]]
 name = "ctor"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd4056f63fce3b82d852c3da92b08ea59959890813a7f4ce9c0ff85b10cf301b"
 dependencies = [
  "quote",
- "syn 2.0.10",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "dashmap"
 version = "5.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
@@ -798,23 +797,14 @@
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
@@ -1106,19 +1096,19 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi 0.3.1",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1272,26 +1262,26 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.52"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d0e1ae9e836cc3beddd63db0df682593d7e2d3d891ae8c9083d2113e1744224"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.4.6"
@@ -1358,34 +1348,46 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.4"
+version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
 dependencies = [
  "aho-corasick 1.0.1",
  "memchr",
+ "regex-automata 0.3.2",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 
 [[package]]
+name = "regex-automata"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "83d3daa6976cffb758ec878f108ba0e062a45b2d6ca3a2cca965338855476caf"
+dependencies = [
+ "aho-corasick 1.0.1",
+ "memchr",
+ "regex-syntax",
+]
+
+[[package]]
 name = "regex-syntax"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "2ab07dc67230e4a4718e70fd5c20055a4334b121f1f9db8fe63ef39ce9b8c846"
 
 [[package]]
 name = "remove_dir_all"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
@@ -1431,37 +1433,37 @@
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.140"
+version = "1.0.167"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc855a42c7967b7c369eb5860f7164ef1f6f81c20c7cc1141f2a604e18723b03"
+checksum = "7daf513456463b42aa1d94cff7e0c24d682b429f020b9afa4f5ba5c40a22b237"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.140"
+version = "1.0.167"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f2122636b9fe3b81f1cb25099fcf2d3f542cdb1d45940d56c713158884a05da"
+checksum = "b69b106b68bc8054f0e974e70d19984040f8a5cf9215ca82626ea4853f82c4b9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.98",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.99"
+version = "1.0.100"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
+checksum = "0f1e14e89be7aa4c4b78bdbdc9eb5bf8517829a600ae8eaa39a6e1d960b5185c"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
@@ -1555,17 +1557,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.10"
+version = "2.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aad1363ed6d37b84299588d62d3a7d95b5a5c2d9aad5c85609fda12afaa1f40"
+checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1591,30 +1593,30 @@
 name = "termtree"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95059e91184749cb66be6dc994f67f182b6d897cb3df74a5bf66b5e709295fd8"
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.10",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5516c27b78311c50bf42c071425c560ac799b11c30b31f87e3081965fe5e0180"
@@ -1677,17 +1679,17 @@
 name = "toml_datetime"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7cda73e2f1397b1262d6dfdcef8aafae14d1de7748d66822d3bfeeb6d03e5e4b"
 
 [[package]]
 name = "toml_edit"
-version = "0.19.11"
+version = "0.19.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "266f016b7f039eec8a1a80dfe6156b633d208b9fccca5e4db1d6775b0c4e34a7"
+checksum = "c500344a19072298cd05a7224b3c0c629348b78692bf48466c5238656e315a78"
 dependencies = [
  "indexmap",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
```

### Comparing `ast_grep_cli-0.7.1/README.md` & `ast_grep_cli-0.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
    <img src="https://img.shields.io/github/forks/ast-grep/ast-grep?style=social" alt="Badge"/>
    <img alt="GitHub Sponsors" src="https://img.shields.io/github/sponsors/HerringtonDarkholme?style=social">
 </p>
 
 
 ## ast-grep(sg)
 
-ast-grep(sg) is a fast and polyglot tool for code structural search, lint and rewriting at large scale..
+ast-grep(sg) is a CLI tool for code structural search, lint, and rewriting.
 
 ## Introduction
 ast-grep is a AST-based tool to search code by pattern code. Think it as your old-friend `grep` but it matches AST nodes instead of text.
 You can write patterns as if you are writing ordinary code. It will match all code that has the same syntactical structure.
 You can use `$` sign + upper case letters as wildcard, e.g. `$MATCH`, to match any single AST node. Think it as REGEX dot `.`, except it is not textual.
 
 Try the [online playground](https://ast-grep.github.io/playground.html) for a taste!
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
                                   [ast-grep]
  [coverage badge] [https://codecov.io/gh/ast-grep/ast-grep/branch/main/graph/
     badge.svg?token=37VX8H2EWV] [Discord] [Badge] [Badge] [GitHub Sponsors]
-## ast-grep(sg) ast-grep(sg) is a fast and polyglot tool for code structural
-search, lint and rewriting at large scale.. ## Introduction ast-grep is a AST-
-based tool to search code by pattern code. Think it as your old-friend `grep`
-but it matches AST nodes instead of text. You can write patterns as if you are
-writing ordinary code. It will match all code that has the same syntactical
-structure. You can use `$` sign + upper case letters as wildcard, e.g.
-`$MATCH`, to match any single AST node. Think it as REGEX dot `.`, except it is
-not textual. Try the [online playground](https://ast-grep.github.io/
-playground.html) for a taste! ## Demo ![output](https://user-
-images.githubusercontent.com/2883231/183275066-8d9c342f-46cb-4fa5-aa4e-
-b98aac011869.gif) ## Installation You can install it from [npm](https://
-docs.npmjs.com/downloading-and-installing-node-js-and-npm), [pip](https://
-pypi.org/), [cargo](https://doc.rust-lang.org/cargo/getting-started/
+## ast-grep(sg) ast-grep(sg) is a CLI tool for code structural search, lint,
+and rewriting. ## Introduction ast-grep is a AST-based tool to search code by
+pattern code. Think it as your old-friend `grep` but it matches AST nodes
+instead of text. You can write patterns as if you are writing ordinary code. It
+will match all code that has the same syntactical structure. You can use `$`
+sign + upper case letters as wildcard, e.g. `$MATCH`, to match any single AST
+node. Think it as REGEX dot `.`, except it is not textual. Try the [online
+playground](https://ast-grep.github.io/playground.html) for a taste! ## Demo !
+[output](https://user-images.githubusercontent.com/2883231/183275066-8d9c342f-
+46cb-4fa5-aa4e-b98aac011869.gif) ## Installation You can install it from [npm]
+(https://docs.npmjs.com/downloading-and-installing-node-js-and-npm), [pip]
+(https://pypi.org/), [cargo](https://doc.rust-lang.org/cargo/getting-started/
 installation.html), [homebrew](https://brew.sh/) or [scoop](https://scoop.sh/)!
 ```bash npm install --global @ast-grep/cli pip install ast-grep-cli cargo
 install ast-grep # install via homebrew, thank @henryhchchc brew install ast-
 grep # install via scoop, thank @brian6932 scoop install main/ast-grep ``` Or
 you can build ast-grep from source. You need install rustup, clone the
 repository and then ```bash cargo install --path ./crates/cli ``` [Packages]
 (https://repology.org/project/ast-grep/versions) are available on other
```

### Comparing `ast_grep_cli-0.7.1/LICENSE` & `ast_grep_cli-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.1/PKG-INFO` & `ast_grep_cli-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ast-grep-cli
-Version: 0.7.1
+Version: 0.7.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
@@ -36,15 +36,15 @@
    <img src="https://img.shields.io/github/forks/ast-grep/ast-grep?style=social" alt="Badge"/>
    <img alt="GitHub Sponsors" src="https://img.shields.io/github/sponsors/HerringtonDarkholme?style=social">
 </p>
 
 
 ## ast-grep(sg)
 
-ast-grep(sg) is a fast and polyglot tool for code structural search, lint and rewriting at large scale..
+ast-grep(sg) is a CLI tool for code structural search, lint, and rewriting.
 
 ## Introduction
 ast-grep is a AST-based tool to search code by pattern code. Think it as your old-friend `grep` but it matches AST nodes instead of text.
 You can write patterns as if you are writing ordinary code. It will match all code that has the same syntactical structure.
 You can use `$` sign + upper case letters as wildcard, e.g. `$MATCH`, to match any single AST node. Think it as REGEX dot `.`, except it is not textual.
 
 Try the [online playground](https://ast-grep.github.io/playground.html) for a taste!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.7.1 Classifier: Development
+Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.7.2 Classifier: Development
 Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Rust Classifier: Topic :: Security Classifier: Topic :: Software Development
 :: Quality Assurance Classifier: Topic :: Software Development Classifier:
 Topic :: Text Processing License-File: LICENSE License-File: LICENSE Summary:
 Structural Search and Rewrite code at large scale using precise AST pattern.
@@ -15,27 +15,26 @@
 Type: text/markdown; charset=UTF-8; variant=GFM Project-URL: Repository, https:
 //github.com/ast-grep/ast-grep Project-URL: Documentation, https://ast-
 grep.github.io/ Project-URL: Changelog, https://github.com/ast-grep/ast-grep/
 blob/main/CHANGELOG.md
                                   [ast-grep]
  [coverage badge] [https://codecov.io/gh/ast-grep/ast-grep/branch/main/graph/
     badge.svg?token=37VX8H2EWV] [Discord] [Badge] [Badge] [GitHub Sponsors]
-## ast-grep(sg) ast-grep(sg) is a fast and polyglot tool for code structural
-search, lint and rewriting at large scale.. ## Introduction ast-grep is a AST-
-based tool to search code by pattern code. Think it as your old-friend `grep`
-but it matches AST nodes instead of text. You can write patterns as if you are
-writing ordinary code. It will match all code that has the same syntactical
-structure. You can use `$` sign + upper case letters as wildcard, e.g.
-`$MATCH`, to match any single AST node. Think it as REGEX dot `.`, except it is
-not textual. Try the [online playground](https://ast-grep.github.io/
-playground.html) for a taste! ## Demo ![output](https://user-
-images.githubusercontent.com/2883231/183275066-8d9c342f-46cb-4fa5-aa4e-
-b98aac011869.gif) ## Installation You can install it from [npm](https://
-docs.npmjs.com/downloading-and-installing-node-js-and-npm), [pip](https://
-pypi.org/), [cargo](https://doc.rust-lang.org/cargo/getting-started/
+## ast-grep(sg) ast-grep(sg) is a CLI tool for code structural search, lint,
+and rewriting. ## Introduction ast-grep is a AST-based tool to search code by
+pattern code. Think it as your old-friend `grep` but it matches AST nodes
+instead of text. You can write patterns as if you are writing ordinary code. It
+will match all code that has the same syntactical structure. You can use `$`
+sign + upper case letters as wildcard, e.g. `$MATCH`, to match any single AST
+node. Think it as REGEX dot `.`, except it is not textual. Try the [online
+playground](https://ast-grep.github.io/playground.html) for a taste! ## Demo !
+[output](https://user-images.githubusercontent.com/2883231/183275066-8d9c342f-
+46cb-4fa5-aa4e-b98aac011869.gif) ## Installation You can install it from [npm]
+(https://docs.npmjs.com/downloading-and-installing-node-js-and-npm), [pip]
+(https://pypi.org/), [cargo](https://doc.rust-lang.org/cargo/getting-started/
 installation.html), [homebrew](https://brew.sh/) or [scoop](https://scoop.sh/)!
 ```bash npm install --global @ast-grep/cli pip install ast-grep-cli cargo
 install ast-grep # install via homebrew, thank @henryhchchc brew install ast-
 grep # install via scoop, thank @brian6932 scoop install main/ast-grep ``` Or
 you can build ast-grep from source. You need install rustup, clone the
 repository and then ```bash cargo install --path ./crates/cli ``` [Packages]
 (https://repology.org/project/ast-grep/versions) are available on other
```

