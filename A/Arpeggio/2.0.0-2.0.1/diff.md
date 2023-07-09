# Comparing `tmp/Arpeggio-2.0.0.tar.gz` & `tmp/Arpeggio-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Arpeggio-2.0.0.tar", last modified: Sun Mar 20 16:43:02 2022, max compression
+gzip compressed data, was "Arpeggio-2.0.1.tar", last modified: Sun Jul  9 08:51:59 2023, max compression
```

## Comparing `Arpeggio-2.0.0.tar` & `Arpeggio-2.0.1.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.959197 Arpeggio-2.0.0/
--rw-r--r--   0 igor      (1000) users      (985)      325 2020-12-24 11:09:24.000000 Arpeggio-2.0.0/.editorconfig
--rw-r--r--   0 igor      (1000) users      (985)       43 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/.gitattributes
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.932530 Arpeggio-2.0.0/.github/
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.939197 Arpeggio-2.0.0/.github/workflows/
--rw-r--r--   0 igor      (1000) users      (985)      682 2022-03-20 16:32:09.000000 Arpeggio-2.0.0/.github/workflows/ci-linux-ubuntu.yml
--rw-r--r--   0 igor      (1000) users      (985)      502 2020-11-01 15:58:14.000000 Arpeggio-2.0.0/.gitignore
--rw-r--r--   0 igor      (1000) users      (985)      381 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/AUTHORS.md
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.939197 Arpeggio-2.0.0/Arpeggio.egg-info/
--rw-r--r--   0 igor      (1000) users      (985)     2133 2022-03-20 16:43:02.000000 Arpeggio-2.0.0/Arpeggio.egg-info/PKG-INFO
--rw-r--r--   0 igor      (1000) users      (985)     4496 2022-03-20 16:43:02.000000 Arpeggio-2.0.0/Arpeggio.egg-info/SOURCES.txt
--rw-r--r--   0 igor      (1000) users      (985)        1 2022-03-20 16:43:02.000000 Arpeggio-2.0.0/Arpeggio.egg-info/dependency_links.txt
--rw-r--r--   0 igor      (1000) users      (985)       72 2022-03-20 16:43:02.000000 Arpeggio-2.0.0/Arpeggio.egg-info/requires.txt
--rw-r--r--   0 igor      (1000) users      (985)        9 2022-03-20 16:43:02.000000 Arpeggio-2.0.0/Arpeggio.egg-info/top_level.txt
--rw-r--r--   0 igor      (1000) users      (985)    11186 2022-03-20 16:39:15.000000 Arpeggio-2.0.0/CHANGELOG.md
--rw-r--r--   0 igor      (1000) users      (985)     5113 2022-03-20 16:35:04.000000 Arpeggio-2.0.0/CONTRIBUTING.md
--rw-r--r--   0 igor      (1000) users      (985)     1218 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/LICENSE
--rw-r--r--   0 igor      (1000) users      (985)     2133 2022-03-20 16:43:02.959197 Arpeggio-2.0.0/PKG-INFO
--rw-r--r--   0 igor      (1000) users      (985)      660 2020-11-01 15:58:14.000000 Arpeggio-2.0.0/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 igor      (1000) users      (985)      935 2021-08-05 13:35:34.000000 Arpeggio-2.0.0/README.md
--rw-r--r--   0 igor      (1000) users      (985)      978 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/THANKS.md
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.939197 Arpeggio-2.0.0/arpeggio/
--rw-r--r--   0 igor      (1000) users      (985)    64606 2022-03-20 16:37:17.000000 Arpeggio-2.0.0/arpeggio/__init__.py
--rw-r--r--   0 igor      (1000) users      (985)     2867 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/cleanpeg.py
--rw-r--r--   0 igor      (1000) users      (985)     6689 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/export.py
--rw-r--r--   0 igor      (1000) users      (985)    10659 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/peg.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.942530 Arpeggio-2.0.0/arpeggio/tests/
--rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/__init__.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.942530 Arpeggio-2.0.0/arpeggio/tests/regressions/
--rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/__init__.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.942530 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_16/
--rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_16/__init__.py
--rw-r--r--   0 igor      (1000) users      (985)     2145 2022-03-20 16:28:33.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_16/test_issue_16.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.942530 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_20/
--rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_20/__init__.py
--rw-r--r--   0 igor      (1000) users      (985)      828 2020-10-11 15:43:47.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_20/test_issue_20.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.945863 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_22/
--rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_22/__init__.py
--rw-r--r--   0 igor      (1000) users      (985)      849 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_22/grammar1.peg
--rw-r--r--   0 igor      (1000) users      (985)      723 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_22/grammar2.peg
--rw-r--r--   0 igor      (1000) users      (985)      550 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_22/test_issue_22.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.945863 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_26/
--rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_26/__init__.py
--rw-r--r--   0 igor      (1000) users      (985)      407 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_26/test_issue_26.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.945863 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_31/
--rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_31/__init__.py
--rw-r--r--   0 igor      (1000) users      (985)      358 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_31/test_issue_31.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.945863 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_32/
--rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_32/__init__.py
--rw-r--r--   0 igor      (1000) users      (985)     8732 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_32/test_issue_32.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.945863 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_43/
--rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_43/__init__.py
--rw-r--r--   0 igor      (1000) users      (985)      562 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_43/test_issue43.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.945863 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_61/
--rw-r--r--   0 igor      (1000) users      (985)     1341 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_61/test_issue_61.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.945863 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_73/
--rw-r--r--   0 igor      (1000) users      (985)      966 2020-04-24 15:38:56.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/issue_73/test_issue_73.py
--rw-r--r--   0 igor      (1000) users      (985)      918 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/test_direct_rule_call.py
--rw-r--r--   0 igor      (1000) users      (985)     1527 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/regressions/test_memoization.py
--rw-r--r--   0 igor      (1000) users      (985)     1365 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_decorator_combine.py
--rw-r--r--   0 igor      (1000) users      (985)     2074 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_default_semantic_action.py
--rw-r--r--   0 igor      (1000) users      (985)     1000 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_eolterm.py
--rw-r--r--   0 igor      (1000) users      (985)     4568 2020-10-14 17:51:26.000000 Arpeggio-2.0.0/arpeggio/tests/test_error_reporting.py
--rw-r--r--   0 igor      (1000) users      (985)     1659 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_examples.py
--rw-r--r--   0 igor      (1000) users      (985)     1633 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_exporter.py
--rw-r--r--   0 igor      (1000) users      (985)     1968 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_flags.py
--rw-r--r--   0 igor      (1000) users      (985)     2958 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_parser_params.py
--rw-r--r--   0 igor      (1000) users      (985)      384 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_parser_resilience.py
--rw-r--r--   0 igor      (1000) users      (985)     9336 2021-04-19 14:54:48.000000 Arpeggio-2.0.0/arpeggio/tests/test_parsing_expressions.py
--rw-r--r--   0 igor      (1000) users      (985)     1015 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_pathologic_models.py
--rw-r--r--   0 igor      (1000) users      (985)     3574 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_peg_parser.py
--rw-r--r--   0 igor      (1000) users      (985)     1522 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_position.py
--rw-r--r--   0 igor      (1000) users      (985)     2342 2020-10-11 15:43:47.000000 Arpeggio-2.0.0/arpeggio/tests/test_ptnode_navigation_expressions.py
--rw-r--r--   0 igor      (1000) users      (985)     2100 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_python_parser.py
--rw-r--r--   0 igor      (1000) users      (985)     1744 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_reduce_tree.py
--rw-r--r--   0 igor      (1000) users      (985)     1713 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_semantic_action_results.py
--rw-r--r--   0 igor      (1000) users      (985)     1482 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_separators.py
--rw-r--r--   0 igor      (1000) users      (985)     2508 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_sequence_params.py
--rw-r--r--   0 igor      (1000) users      (985)     1835 2020-10-11 15:43:50.000000 Arpeggio-2.0.0/arpeggio/tests/test_suppression.py
--rw-r--r--   0 igor      (1000) users      (985)      751 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_unicode.py
--rw-r--r--   0 igor      (1000) users      (985)     1709 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/tests/test_visitor.py
--rw-r--r--   0 igor      (1000) users      (985)      416 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/arpeggio/utils.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.945863 Arpeggio-2.0.0/art/
--rw-r--r--   0 igor      (1000) users      (985)    11906 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/art/arpeggio-logo.png
--rw-r--r--   0 igor      (1000) users      (985)    14015 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/art/arpeggio-logo.svg
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.945863 Arpeggio-2.0.0/docs/
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.949197 Arpeggio-2.0.0/docs/about/
--rw-r--r--   0 igor      (1000) users      (985)      170 2020-11-01 15:58:14.000000 Arpeggio-2.0.0/docs/about/contributing.md
--rw-r--r--   0 igor      (1000) users      (985)      207 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/docs/about/discuss.md
--rw-r--r--   0 igor      (1000) users      (985)     1162 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/docs/about/license.md
--rw-r--r--   0 igor      (1000) users      (985)     5156 2020-10-11 15:43:50.000000 Arpeggio-2.0.0/docs/configuration.md
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.949197 Arpeggio-2.0.0/docs/css/
--rw-r--r--   0 igor      (1000) users      (985)       86 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/docs/css/version-select.css
--rw-r--r--   0 igor      (1000) users      (985)     4166 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/docs/debugging.md
--rw-r--r--   0 igor      (1000) users      (985)      386 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/docs/extra.css
--rw-r--r--   0 igor      (1000) users      (985)     5017 2021-04-19 14:54:48.000000 Arpeggio-2.0.0/docs/getting_started.md
--rw-r--r--   0 igor      (1000) users      (985)    12270 2020-11-26 17:04:20.000000 Arpeggio-2.0.0/docs/grammars.md
--rw-r--r--   0 igor      (1000) users      (985)     2386 2021-08-05 13:35:34.000000 Arpeggio-2.0.0/docs/handling_errors.md
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.949197 Arpeggio-2.0.0/docs/images/
--rw-r--r--   0 igor      (1000) users      (985)    14015 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/docs/images/arpeggio-logo.svg
--rw-r--r--   0 igor      (1000) users      (985)   169538 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/docs/images/calc_parse_tree.dot.png
--rw-r--r--   0 igor      (1000) users      (985)   140476 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/docs/images/calc_parse_tree_reduced.dot.png
--rw-r--r--   0 igor      (1000) users      (985)   130314 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/docs/images/calc_parser_model.dot.png
--rw-r--r--   0 igor      (1000) users      (985)   275117 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/docs/images/csvfile_parse_tree.dot.png
--rw-r--r--   0 igor      (1000) users      (985)     3320 2022-03-20 16:35:45.000000 Arpeggio-2.0.0/docs/index.md
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.949197 Arpeggio-2.0.0/docs/js/
--rw-r--r--   0 igor      (1000) users      (985)     2079 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/docs/js/version-select.js
--rw-r--r--   0 igor      (1000) users      (985)     6026 2020-10-11 15:43:50.000000 Arpeggio-2.0.0/docs/parse_trees.md
--rw-r--r--   0 igor      (1000) users      (985)     6336 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/docs/semantics.md
--rw-r--r--   0 igor      (1000) users      (985)     3533 2020-10-11 15:43:47.000000 Arpeggio-2.0.0/docs/troubleshooting.md
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.949197 Arpeggio-2.0.0/docs/tutorials/
--rw-r--r--   0 igor      (1000) users      (985)     6970 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/docs/tutorials/bibtex.md
--rw-r--r--   0 igor      (1000) users      (985)     6562 2020-10-11 15:43:47.000000 Arpeggio-2.0.0/docs/tutorials/calc.md
--rw-r--r--   0 igor      (1000) users      (985)    10399 2020-10-11 15:43:47.000000 Arpeggio-2.0.0/docs/tutorials/csv.md
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.949197 Arpeggio-2.0.0/examples/
--rw-r--r--   0 igor      (1000) users      (985)      971 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/README.md
--rw-r--r--   0 igor      (1000) users      (985)       35 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/__init__.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.949197 Arpeggio-2.0.0/examples/bibtex/
--rw-r--r--   0 igor      (1000) users      (985)      617 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/bibtex/README.md
--rw-r--r--   0 igor      (1000) users      (985)     4930 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/bibtex/bibtex.py
--rw-r--r--   0 igor      (1000) users      (985)     2639 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/bibtex/bibtex_example.bib
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.952530 Arpeggio-2.0.0/examples/calc/
--rw-r--r--   0 igor      (1000) users      (985)     1584 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/calc/README.md
--rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/calc/__init__.py
--rw-r--r--   0 igor      (1000) users      (985)      240 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/calc/calc.peg
--rw-r--r--   0 igor      (1000) users      (985)     3857 2020-10-11 15:43:47.000000 Arpeggio-2.0.0/examples/calc/calc.py
--rw-r--r--   0 igor      (1000) users      (985)      224 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/calc/calc_clean.peg
--rw-r--r--   0 igor      (1000) users      (985)     2403 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/calc/calc_cleanpeg.py
--rw-r--r--   0 igor      (1000) users      (985)     2379 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/calc/calc_peg.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.952530 Arpeggio-2.0.0/examples/csv/
--rw-r--r--   0 igor      (1000) users      (985)      880 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/csv/README.md
--rw-r--r--   0 igor      (1000) users      (985)        2 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/csv/__init__.py
--rw-r--r--   0 igor      (1000) users      (985)      210 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/csv/csv.peg
--rw-r--r--   0 igor      (1000) users      (985)     2595 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/csv/csv.py
--rw-r--r--   0 igor      (1000) users      (985)     1761 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/csv/csv_peg.py
--rw-r--r--   0 igor      (1000) users      (985)      219 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/csv/test_data.csv
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.952530 Arpeggio-2.0.0/examples/json/
--rw-r--r--   0 igor      (1000) users      (985)      744 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/json/README.md
--rw-r--r--   0 igor      (1000) users      (985)     2050 2022-03-20 16:28:33.000000 Arpeggio-2.0.0/examples/json/json.py
--rw-r--r--   0 igor      (1000) users      (985)      915 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/json/test.json
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.952530 Arpeggio-2.0.0/examples/peg_peg/
--rw-r--r--   0 igor      (1000) users      (985)     1732 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/peg_peg/README.md
--rw-r--r--   0 igor      (1000) users      (985)      649 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/peg_peg/peg.peg
--rw-r--r--   0 igor      (1000) users      (985)     2340 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/peg_peg/peg_peg.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.952530 Arpeggio-2.0.0/examples/robot/
--rw-r--r--   0 igor      (1000) users      (985)     1218 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/robot/README.md
--rw-r--r--   0 igor      (1000) users      (985)       52 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/robot/program.rbt
--rw-r--r--   0 igor      (1000) users      (985)      118 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/robot/robot.peg
--rw-r--r--   0 igor      (1000) users      (985)     3155 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/robot/robot.py
--rw-r--r--   0 igor      (1000) users      (985)     2039 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/robot/robot_peg.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.952530 Arpeggio-2.0.0/examples/simple/
--rw-r--r--   0 igor      (1000) users      (985)      654 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/examples/simple/README.md
--rw-r--r--   0 igor      (1000) users      (985)      186 2020-10-08 19:46:40.000000 Arpeggio-2.0.0/examples/simple/program.simple
--rw-r--r--   0 igor      (1000) users      (985)     2245 2022-03-20 16:28:33.000000 Arpeggio-2.0.0/examples/simple/simple.py
--rwxr-xr-x   0 igor      (1000) users      (985)       97 2020-11-01 15:58:14.000000 Arpeggio-2.0.0/install-dev.sh
--rwxr-xr-x   0 igor      (1000) users      (985)       80 2020-11-01 15:58:14.000000 Arpeggio-2.0.0/install-test.sh
--rw-r--r--   0 igor      (1000) users      (985)      931 2021-08-05 13:35:34.000000 Arpeggio-2.0.0/mkdocs.yml
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.955864 Arpeggio-2.0.0/perf-tests/
--rw-r--r--   0 igor      (1000) users      (985)     1460 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/grammar.py
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.955864 Arpeggio-2.0.0/perf-tests/reports/
--rw-r--r--   0 igor      (1000) users      (985)     1924 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/reports/_speed_report.txt
--rw-r--r--   0 igor      (1000) users      (985)     1320 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/reports/py2_memory_report_memoization.txt
--rw-r--r--   0 igor      (1000) users      (985)     1326 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/reports/py2_memory_report_nomemoization.txt
--rw-r--r--   0 igor      (1000) users      (985)     1913 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/reports/py2_speed_report.txt
--rw-r--r--   0 igor      (1000) users      (985)     1319 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/reports/py3_memory_report_memoization.txt
--rw-r--r--   0 igor      (1000) users      (985)     1325 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/reports/py3_memory_report_nomemoization.txt
--rw-r--r--   0 igor      (1000) users      (985)     1924 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/reports/py3_speed_report.txt
--rw-r--r--   0 igor      (1000) users      (985)       23 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/requirements.txt
--rwxr-xr-x   0 igor      (1000) users      (985)       52 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/run_all_py2.sh
--rwxr-xr-x   0 igor      (1000) users      (985)       52 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/run_all_py3.sh
--rwxr-xr-x   0 igor      (1000) users      (985)      333 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/run_memory.sh
--rwxr-xr-x   0 igor      (1000) users      (985)      138 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/run_speed.sh
-drwxr-xr-x   0 igor      (1000) users      (985)        0 2022-03-20 16:43:02.955864 Arpeggio-2.0.0/perf-tests/test_inputs/
--rw-r--r--   0 igor      (1000) users      (985)   672240 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/test_inputs/LightSwitch.rpy
--rw-r--r--   0 igor      (1000) users      (985)  1344081 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/test_inputs/LightSwitchDouble.rpy
--rw-r--r--   0 igor      (1000) users      (985)     1187 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/test_memory_memoization.py
--rw-r--r--   0 igor      (1000) users      (985)     1194 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/test_memory_nomemoization.py
--rw-r--r--   0 igor      (1000) users      (985)     2295 2019-12-07 15:58:44.000000 Arpeggio-2.0.0/perf-tests/test_speed.py
--rwxr-xr-x   0 igor      (1000) users      (985)      281 2020-11-01 15:58:14.000000 Arpeggio-2.0.0/runtests.sh
--rw-r--r--   0 igor      (1000) users      (985)     1556 2022-03-20 16:43:02.959197 Arpeggio-2.0.0/setup.cfg
--rw-r--r--   0 igor      (1000) users      (985)     1644 2020-11-26 17:04:20.000000 Arpeggio-2.0.0/setup.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.888053 Arpeggio-2.0.1/
+-rw-r--r--   0 igor      (1000) users      (985)      325 2020-12-24 11:09:24.000000 Arpeggio-2.0.1/.editorconfig
+-rw-r--r--   0 igor      (1000) users      (985)       43 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/.gitattributes
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.871386 Arpeggio-2.0.1/.github/
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.874719 Arpeggio-2.0.1/.github/workflows/
+-rw-r--r--   0 igor      (1000) users      (985)      755 2023-07-09 08:35:26.000000 Arpeggio-2.0.1/.github/workflows/ci-linux-ubuntu.yml
+-rw-r--r--   0 igor      (1000) users      (985)      538 2023-07-08 14:04:01.000000 Arpeggio-2.0.1/.gitignore
+-rw-r--r--   0 igor      (1000) users      (985)      381 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/AUTHORS.md
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.874719 Arpeggio-2.0.1/Arpeggio.egg-info/
+-rw-r--r--   0 igor      (1000) users      (985)     2128 2023-07-09 08:51:59.000000 Arpeggio-2.0.1/Arpeggio.egg-info/PKG-INFO
+-rw-r--r--   0 igor      (1000) users      (985)     4496 2023-07-09 08:51:59.000000 Arpeggio-2.0.1/Arpeggio.egg-info/SOURCES.txt
+-rw-r--r--   0 igor      (1000) users      (985)        1 2023-07-09 08:51:59.000000 Arpeggio-2.0.1/Arpeggio.egg-info/dependency_links.txt
+-rw-r--r--   0 igor      (1000) users      (985)       72 2023-07-09 08:51:59.000000 Arpeggio-2.0.1/Arpeggio.egg-info/requires.txt
+-rw-r--r--   0 igor      (1000) users      (985)        9 2023-07-09 08:51:59.000000 Arpeggio-2.0.1/Arpeggio.egg-info/top_level.txt
+-rw-r--r--   0 igor      (1000) users      (985)    11442 2023-07-09 08:47:44.000000 Arpeggio-2.0.1/CHANGELOG.md
+-rw-r--r--   0 igor      (1000) users      (985)     5113 2022-03-20 16:35:04.000000 Arpeggio-2.0.1/CONTRIBUTING.md
+-rw-r--r--   0 igor      (1000) users      (985)     1218 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/LICENSE
+-rw-r--r--   0 igor      (1000) users      (985)     2128 2023-07-09 08:51:59.888053 Arpeggio-2.0.1/PKG-INFO
+-rw-r--r--   0 igor      (1000) users      (985)      660 2020-11-01 15:58:14.000000 Arpeggio-2.0.1/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 igor      (1000) users      (985)      935 2021-08-05 13:35:34.000000 Arpeggio-2.0.1/README.md
+-rw-r--r--   0 igor      (1000) users      (985)      978 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/THANKS.md
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.878052 Arpeggio-2.0.1/arpeggio/
+-rw-r--r--   0 igor      (1000) users      (985)    64627 2023-07-09 08:47:59.000000 Arpeggio-2.0.1/arpeggio/__init__.py
+-rw-r--r--   0 igor      (1000) users      (985)     2867 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/cleanpeg.py
+-rw-r--r--   0 igor      (1000) users      (985)     6689 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/export.py
+-rw-r--r--   0 igor      (1000) users      (985)    10659 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/peg.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.878052 Arpeggio-2.0.1/arpeggio/tests/
+-rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/__init__.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.878052 Arpeggio-2.0.1/arpeggio/tests/regressions/
+-rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/__init__.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.878052 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_16/
+-rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_16/__init__.py
+-rw-r--r--   0 igor      (1000) users      (985)     2145 2022-03-20 16:28:33.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_16/test_issue_16.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.878052 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_20/
+-rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_20/__init__.py
+-rw-r--r--   0 igor      (1000) users      (985)      828 2023-07-09 08:46:28.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_20/test_issue_20.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.881386 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_22/
+-rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_22/__init__.py
+-rw-r--r--   0 igor      (1000) users      (985)      849 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_22/grammar1.peg
+-rw-r--r--   0 igor      (1000) users      (985)      723 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_22/grammar2.peg
+-rw-r--r--   0 igor      (1000) users      (985)      550 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_22/test_issue_22.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.881386 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_26/
+-rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_26/__init__.py
+-rw-r--r--   0 igor      (1000) users      (985)      407 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_26/test_issue_26.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.881386 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_31/
+-rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_31/__init__.py
+-rw-r--r--   0 igor      (1000) users      (985)      358 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_31/test_issue_31.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.881386 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_32/
+-rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_32/__init__.py
+-rw-r--r--   0 igor      (1000) users      (985)     8732 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_32/test_issue_32.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.881386 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_43/
+-rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_43/__init__.py
+-rw-r--r--   0 igor      (1000) users      (985)      562 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_43/test_issue43.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.881386 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_61/
+-rw-r--r--   0 igor      (1000) users      (985)     1341 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_61/test_issue_61.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.881386 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_73/
+-rw-r--r--   0 igor      (1000) users      (985)      966 2020-04-24 15:38:56.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/issue_73/test_issue_73.py
+-rw-r--r--   0 igor      (1000) users      (985)      918 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/test_direct_rule_call.py
+-rw-r--r--   0 igor      (1000) users      (985)     1527 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/regressions/test_memoization.py
+-rw-r--r--   0 igor      (1000) users      (985)     1365 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_decorator_combine.py
+-rw-r--r--   0 igor      (1000) users      (985)     2074 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_default_semantic_action.py
+-rw-r--r--   0 igor      (1000) users      (985)     1000 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_eolterm.py
+-rw-r--r--   0 igor      (1000) users      (985)     5938 2023-07-09 08:46:28.000000 Arpeggio-2.0.1/arpeggio/tests/test_error_reporting.py
+-rw-r--r--   0 igor      (1000) users      (985)     1659 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_examples.py
+-rw-r--r--   0 igor      (1000) users      (985)     1633 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_exporter.py
+-rw-r--r--   0 igor      (1000) users      (985)     1968 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_flags.py
+-rw-r--r--   0 igor      (1000) users      (985)     2958 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_parser_params.py
+-rw-r--r--   0 igor      (1000) users      (985)      384 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_parser_resilience.py
+-rw-r--r--   0 igor      (1000) users      (985)     9336 2023-07-09 08:46:28.000000 Arpeggio-2.0.1/arpeggio/tests/test_parsing_expressions.py
+-rw-r--r--   0 igor      (1000) users      (985)     1015 2023-07-09 08:46:28.000000 Arpeggio-2.0.1/arpeggio/tests/test_pathologic_models.py
+-rw-r--r--   0 igor      (1000) users      (985)     3574 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_peg_parser.py
+-rw-r--r--   0 igor      (1000) users      (985)     1522 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_position.py
+-rw-r--r--   0 igor      (1000) users      (985)     2342 2020-10-11 15:43:47.000000 Arpeggio-2.0.1/arpeggio/tests/test_ptnode_navigation_expressions.py
+-rw-r--r--   0 igor      (1000) users      (985)     2100 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_python_parser.py
+-rw-r--r--   0 igor      (1000) users      (985)     1744 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_reduce_tree.py
+-rw-r--r--   0 igor      (1000) users      (985)     1713 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_semantic_action_results.py
+-rw-r--r--   0 igor      (1000) users      (985)     1482 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_separators.py
+-rw-r--r--   0 igor      (1000) users      (985)     2508 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_sequence_params.py
+-rw-r--r--   0 igor      (1000) users      (985)     1835 2020-10-11 15:43:50.000000 Arpeggio-2.0.1/arpeggio/tests/test_suppression.py
+-rw-r--r--   0 igor      (1000) users      (985)      751 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_unicode.py
+-rw-r--r--   0 igor      (1000) users      (985)     1709 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/tests/test_visitor.py
+-rw-r--r--   0 igor      (1000) users      (985)      416 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/arpeggio/utils.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.881386 Arpeggio-2.0.1/art/
+-rw-r--r--   0 igor      (1000) users      (985)    11906 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/art/arpeggio-logo.png
+-rw-r--r--   0 igor      (1000) users      (985)    14015 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/art/arpeggio-logo.svg
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.881386 Arpeggio-2.0.1/docs/
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.881386 Arpeggio-2.0.1/docs/about/
+-rw-r--r--   0 igor      (1000) users      (985)      170 2020-11-01 15:58:14.000000 Arpeggio-2.0.1/docs/about/contributing.md
+-rw-r--r--   0 igor      (1000) users      (985)      207 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/docs/about/discuss.md
+-rw-r--r--   0 igor      (1000) users      (985)     1162 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/docs/about/license.md
+-rw-r--r--   0 igor      (1000) users      (985)     5156 2020-10-11 15:43:50.000000 Arpeggio-2.0.1/docs/configuration.md
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.881386 Arpeggio-2.0.1/docs/css/
+-rw-r--r--   0 igor      (1000) users      (985)       86 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/docs/css/version-select.css
+-rw-r--r--   0 igor      (1000) users      (985)     4166 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/docs/debugging.md
+-rw-r--r--   0 igor      (1000) users      (985)      386 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/docs/extra.css
+-rw-r--r--   0 igor      (1000) users      (985)     5017 2021-04-19 14:54:48.000000 Arpeggio-2.0.1/docs/getting_started.md
+-rw-r--r--   0 igor      (1000) users      (985)    12270 2020-11-26 17:04:20.000000 Arpeggio-2.0.1/docs/grammars.md
+-rw-r--r--   0 igor      (1000) users      (985)     2386 2021-08-05 13:35:34.000000 Arpeggio-2.0.1/docs/handling_errors.md
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.881386 Arpeggio-2.0.1/docs/images/
+-rw-r--r--   0 igor      (1000) users      (985)    14015 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/docs/images/arpeggio-logo.svg
+-rw-r--r--   0 igor      (1000) users      (985)   169538 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/docs/images/calc_parse_tree.dot.png
+-rw-r--r--   0 igor      (1000) users      (985)   140476 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/docs/images/calc_parse_tree_reduced.dot.png
+-rw-r--r--   0 igor      (1000) users      (985)   130314 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/docs/images/calc_parser_model.dot.png
+-rw-r--r--   0 igor      (1000) users      (985)   275117 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/docs/images/csvfile_parse_tree.dot.png
+-rw-r--r--   0 igor      (1000) users      (985)     3320 2023-07-09 08:46:28.000000 Arpeggio-2.0.1/docs/index.md
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.881386 Arpeggio-2.0.1/docs/js/
+-rw-r--r--   0 igor      (1000) users      (985)     2079 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/docs/js/version-select.js
+-rw-r--r--   0 igor      (1000) users      (985)     6026 2020-10-11 15:43:50.000000 Arpeggio-2.0.1/docs/parse_trees.md
+-rw-r--r--   0 igor      (1000) users      (985)     6336 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/docs/semantics.md
+-rw-r--r--   0 igor      (1000) users      (985)     3533 2020-10-11 15:43:47.000000 Arpeggio-2.0.1/docs/troubleshooting.md
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.884719 Arpeggio-2.0.1/docs/tutorials/
+-rw-r--r--   0 igor      (1000) users      (985)     6970 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/docs/tutorials/bibtex.md
+-rw-r--r--   0 igor      (1000) users      (985)     6562 2020-10-11 15:43:47.000000 Arpeggio-2.0.1/docs/tutorials/calc.md
+-rw-r--r--   0 igor      (1000) users      (985)    10399 2020-10-11 15:43:47.000000 Arpeggio-2.0.1/docs/tutorials/csv.md
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.884719 Arpeggio-2.0.1/examples/
+-rw-r--r--   0 igor      (1000) users      (985)      971 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/README.md
+-rw-r--r--   0 igor      (1000) users      (985)       35 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/__init__.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.884719 Arpeggio-2.0.1/examples/bibtex/
+-rw-r--r--   0 igor      (1000) users      (985)      617 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/bibtex/README.md
+-rw-r--r--   0 igor      (1000) users      (985)     4930 2023-07-08 11:04:39.000000 Arpeggio-2.0.1/examples/bibtex/bibtex.py
+-rw-r--r--   0 igor      (1000) users      (985)     2639 2023-04-20 16:18:51.000000 Arpeggio-2.0.1/examples/bibtex/bibtex_example.bib
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.884719 Arpeggio-2.0.1/examples/calc/
+-rw-r--r--   0 igor      (1000) users      (985)     1584 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/calc/README.md
+-rw-r--r--   0 igor      (1000) users      (985)        0 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/calc/__init__.py
+-rw-r--r--   0 igor      (1000) users      (985)      240 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/calc/calc.peg
+-rw-r--r--   0 igor      (1000) users      (985)     3857 2020-10-11 15:43:47.000000 Arpeggio-2.0.1/examples/calc/calc.py
+-rw-r--r--   0 igor      (1000) users      (985)      224 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/calc/calc_clean.peg
+-rw-r--r--   0 igor      (1000) users      (985)     2403 2023-02-10 10:59:59.000000 Arpeggio-2.0.1/examples/calc/calc_cleanpeg.py
+-rw-r--r--   0 igor      (1000) users      (985)     2379 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/calc/calc_peg.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.884719 Arpeggio-2.0.1/examples/csv/
+-rw-r--r--   0 igor      (1000) users      (985)      880 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/csv/README.md
+-rw-r--r--   0 igor      (1000) users      (985)        2 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/csv/__init__.py
+-rw-r--r--   0 igor      (1000) users      (985)      210 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/csv/csv.peg
+-rw-r--r--   0 igor      (1000) users      (985)     2595 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/csv/csv.py
+-rw-r--r--   0 igor      (1000) users      (985)     1761 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/csv/csv_peg.py
+-rw-r--r--   0 igor      (1000) users      (985)      219 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/csv/test_data.csv
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.884719 Arpeggio-2.0.1/examples/json/
+-rw-r--r--   0 igor      (1000) users      (985)      744 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/json/README.md
+-rw-r--r--   0 igor      (1000) users      (985)     2050 2022-03-20 16:28:33.000000 Arpeggio-2.0.1/examples/json/json.py
+-rw-r--r--   0 igor      (1000) users      (985)      915 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/json/test.json
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.884719 Arpeggio-2.0.1/examples/peg_peg/
+-rw-r--r--   0 igor      (1000) users      (985)     1732 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/peg_peg/README.md
+-rw-r--r--   0 igor      (1000) users      (985)      649 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/peg_peg/peg.peg
+-rw-r--r--   0 igor      (1000) users      (985)     2340 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/peg_peg/peg_peg.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.884719 Arpeggio-2.0.1/examples/robot/
+-rw-r--r--   0 igor      (1000) users      (985)     1218 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/robot/README.md
+-rw-r--r--   0 igor      (1000) users      (985)       52 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/robot/program.rbt
+-rw-r--r--   0 igor      (1000) users      (985)      118 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/robot/robot.peg
+-rw-r--r--   0 igor      (1000) users      (985)     3155 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/robot/robot.py
+-rw-r--r--   0 igor      (1000) users      (985)     2039 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/robot/robot_peg.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.884719 Arpeggio-2.0.1/examples/simple/
+-rw-r--r--   0 igor      (1000) users      (985)      654 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/examples/simple/README.md
+-rw-r--r--   0 igor      (1000) users      (985)      186 2023-07-08 11:04:39.000000 Arpeggio-2.0.1/examples/simple/program.simple
+-rw-r--r--   0 igor      (1000) users      (985)     2245 2023-07-08 11:04:39.000000 Arpeggio-2.0.1/examples/simple/simple.py
+-rwxr-xr-x   0 igor      (1000) users      (985)       97 2020-11-01 15:58:14.000000 Arpeggio-2.0.1/install-dev.sh
+-rwxr-xr-x   0 igor      (1000) users      (985)       80 2020-11-01 15:58:14.000000 Arpeggio-2.0.1/install-test.sh
+-rw-r--r--   0 igor      (1000) users      (985)      931 2021-08-05 13:35:34.000000 Arpeggio-2.0.1/mkdocs.yml
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.888053 Arpeggio-2.0.1/perf-tests/
+-rw-r--r--   0 igor      (1000) users      (985)     1460 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/grammar.py
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.888053 Arpeggio-2.0.1/perf-tests/reports/
+-rw-r--r--   0 igor      (1000) users      (985)     1924 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/reports/_speed_report.txt
+-rw-r--r--   0 igor      (1000) users      (985)     1320 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/reports/py2_memory_report_memoization.txt
+-rw-r--r--   0 igor      (1000) users      (985)     1326 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/reports/py2_memory_report_nomemoization.txt
+-rw-r--r--   0 igor      (1000) users      (985)     1913 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/reports/py2_speed_report.txt
+-rw-r--r--   0 igor      (1000) users      (985)     1319 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/reports/py3_memory_report_memoization.txt
+-rw-r--r--   0 igor      (1000) users      (985)     1325 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/reports/py3_memory_report_nomemoization.txt
+-rw-r--r--   0 igor      (1000) users      (985)     1924 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/reports/py3_speed_report.txt
+-rw-r--r--   0 igor      (1000) users      (985)       23 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/requirements.txt
+-rwxr-xr-x   0 igor      (1000) users      (985)       52 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/run_all_py2.sh
+-rwxr-xr-x   0 igor      (1000) users      (985)       52 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/run_all_py3.sh
+-rwxr-xr-x   0 igor      (1000) users      (985)      333 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/run_memory.sh
+-rwxr-xr-x   0 igor      (1000) users      (985)      138 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/run_speed.sh
+drwxr-xr-x   0 igor      (1000) users      (985)        0 2023-07-09 08:51:59.888053 Arpeggio-2.0.1/perf-tests/test_inputs/
+-rw-r--r--   0 igor      (1000) users      (985)   672240 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/test_inputs/LightSwitch.rpy
+-rw-r--r--   0 igor      (1000) users      (985)  1344081 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/test_inputs/LightSwitchDouble.rpy
+-rw-r--r--   0 igor      (1000) users      (985)     1187 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/test_memory_memoization.py
+-rw-r--r--   0 igor      (1000) users      (985)     1194 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/test_memory_nomemoization.py
+-rw-r--r--   0 igor      (1000) users      (985)     2295 2019-12-07 15:58:44.000000 Arpeggio-2.0.1/perf-tests/test_speed.py
+-rwxr-xr-x   0 igor      (1000) users      (985)      280 2023-07-09 08:37:40.000000 Arpeggio-2.0.1/runtests.sh
+-rw-r--r--   0 igor      (1000) users      (985)     1556 2023-07-09 08:51:59.891386 Arpeggio-2.0.1/setup.cfg
+-rw-r--r--   0 igor      (1000) users      (985)     1644 2020-11-26 17:04:20.000000 Arpeggio-2.0.1/setup.py
```

### Comparing `Arpeggio-2.0.0/.github/workflows/ci-linux-ubuntu.yml` & `Arpeggio-2.0.1/.github/workflows/ci-linux-ubuntu.yml`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,30 @@
     branches-ignore:
       - 'gh-pages'
   pull_request:
 
 jobs:
   build:
 
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-20.04
     strategy:
       matrix:
-        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install test dependencies
       run: |
         ./install-test.sh
     - name: Run unit tests
       run: |
         ./runtests.sh
     - name: Coveralls
       env:
         COVERALLS_REPO_TOKEN: ${{ secrets.COVERALLS_REPO_TOKEN }}
+        GITHUB_TOKEN: ${{secrets.GITHUB_TOKEN}}
       run: |
-        coveralls
+        coveralls --service=github
```

### Comparing `Arpeggio-2.0.0/Arpeggio.egg-info/PKG-INFO` & `Arpeggio-2.0.1/Arpeggio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: Arpeggio
-Version: 2.0.0
+Version: 2.0.1
 Summary: Packrat parser interpreter
 Home-page: https://github.com/textX/Arpeggio
+Download-URL: 
 Author: Igor R. Dejanovic
 Author-email: igor.dejanovic@gmail.com
 License: MIT
 Keywords: parser,PEG,packrat,library,interpreter
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -40,9 +40,7 @@
 Arpeggio is a recursive descent parser with memoization based on PEG grammars
 (aka Packrat parser).
 
 Documentation with tutorials is available [here](http://textx.github.io/Arpeggio/).
 
 **Note:** for a higher level parsing/language tool (i.e., a nicer interface to
 Arpeggio) see [textX](https://github.com/textX/textX).
-
-
```

### Comparing `Arpeggio-2.0.0/Arpeggio.egg-info/SOURCES.txt` & `Arpeggio-2.0.1/Arpeggio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/CHANGELOG.md` & `Arpeggio-2.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,27 @@
 Everything that is documented in the [official docs][ArpeggioDocs] is considered
 the part of the public API.
 
 Backward incompatible changes are marked with **(BIC)**. These changes are the
 reason for the major version increase so when upgrading between major versions
 please take a look at related PRs and issues and see if the change affects you.
 
-
 ## [Unreleased]
 
 
-[Unreleased]: https://github.com/textX/Arpeggio/compare/2.0.0...HEAD
+[Unreleased]: https://github.com/textX/Arpeggio/compare/2.0.1...HEAD
+
+
+## [2.0.1] (released: 2023-07-09)
+
+- fix: replace `\n` with `\\n` in error reports for matches [#99]. Thanks
+  @mettta and @stanislaw.
+
+[Unreleased]: https://github.com/textX/Arpeggio/compare/2.0.0...2.0.1
+[#99]: https://github.com/textX/Arpeggio/pull/99
 
 
 ## [2.0.0] (released: 2022-03-20)
 
 - Added `eval_attrs` call to `NoMatch` exceptions ([ebfd60]). See [the
   docs](https://textx.github.io/Arpeggio/latest/handling_errors/).
 - Dropped support for deprecated Python versions. The lowest supported version
```

### Comparing `Arpeggio-2.0.0/CONTRIBUTING.md` & `Arpeggio-2.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/LICENSE` & `Arpeggio-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/PKG-INFO` & `Arpeggio-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: Arpeggio
-Version: 2.0.0
+Version: 2.0.1
 Summary: Packrat parser interpreter
 Home-page: https://github.com/textX/Arpeggio
+Download-URL: 
 Author: Igor R. Dejanovic
 Author-email: igor.dejanovic@gmail.com
 License: MIT
 Keywords: parser,PEG,packrat,library,interpreter
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -40,9 +40,7 @@
 Arpeggio is a recursive descent parser with memoization based on PEG grammars
 (aka Packrat parser).
 
 Documentation with tutorials is available [here](http://textx.github.io/Arpeggio/).
 
 **Note:** for a higher level parsing/language tool (i.e., a nicer interface to
 Arpeggio) see [textX](https://github.com/textX/textX).
-
-
```

### Comparing `Arpeggio-2.0.0/PULL_REQUEST_TEMPLATE.md` & `Arpeggio-2.0.1/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/README.md` & `Arpeggio-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/THANKS.md` & `Arpeggio-2.0.1/THANKS.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/__init__.py` & `Arpeggio-2.0.1/arpeggio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from collections import OrderedDict
 import codecs
 import re
 import bisect
 from arpeggio.utils import isstr
 import types
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 if sys.version < '3':
     text = unicode
 else:
     text = str
 
 DEFAULT_WS = '\t\n\r '
@@ -82,15 +82,15 @@
             if hasattr(rule, '_exp_str'):
                 # Rule may override expected report string
                 return rule._exp_str
             elif rule.root:
                 return rule.rule_name
             elif isinstance(rule, Match) and \
                     not isinstance(rule, EndOfFile):
-                return "'{}'".format(rule.to_match)
+                return "'{}'".format(rule.to_match.replace('\n', '\\n'))
             else:
                 return rule.name
 
         if not self.rules:
             self.message = "Not expected input"
         else:
             what_is_expected = OrderedDict.fromkeys(
```

### Comparing `Arpeggio-2.0.0/arpeggio/cleanpeg.py` & `Arpeggio-2.0.1/arpeggio/cleanpeg.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/export.py` & `Arpeggio-2.0.1/arpeggio/export.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/peg.py` & `Arpeggio-2.0.1/arpeggio/peg.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/regressions/issue_16/test_issue_16.py` & `Arpeggio-2.0.1/arpeggio/tests/regressions/issue_16/test_issue_16.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/regressions/issue_20/test_issue_20.py` & `Arpeggio-2.0.1/arpeggio/tests/regressions/issue_20/test_issue_20.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/regressions/issue_22/grammar1.peg` & `Arpeggio-2.0.1/arpeggio/tests/regressions/issue_22/grammar1.peg`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/regressions/issue_22/grammar2.peg` & `Arpeggio-2.0.1/arpeggio/tests/regressions/issue_22/grammar2.peg`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/regressions/issue_22/test_issue_22.py` & `Arpeggio-2.0.1/arpeggio/tests/regressions/issue_22/test_issue_22.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/regressions/issue_32/test_issue_32.py` & `Arpeggio-2.0.1/arpeggio/tests/regressions/issue_32/test_issue_32.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/regressions/issue_43/test_issue43.py` & `Arpeggio-2.0.1/arpeggio/tests/regressions/issue_43/test_issue43.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/regressions/issue_61/test_issue_61.py` & `Arpeggio-2.0.1/arpeggio/tests/regressions/issue_61/test_issue_61.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/regressions/issue_73/test_issue_73.py` & `Arpeggio-2.0.1/arpeggio/tests/regressions/issue_73/test_issue_73.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/regressions/test_direct_rule_call.py` & `Arpeggio-2.0.1/arpeggio/tests/regressions/test_direct_rule_call.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/regressions/test_memoization.py` & `Arpeggio-2.0.1/arpeggio/tests/regressions/test_memoization.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_decorator_combine.py` & `Arpeggio-2.0.1/arpeggio/tests/test_decorator_combine.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_default_semantic_action.py` & `Arpeggio-2.0.1/arpeggio/tests/test_default_semantic_action.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_eolterm.py` & `Arpeggio-2.0.1/arpeggio/tests/test_eolterm.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_error_reporting.py` & `Arpeggio-2.0.1/arpeggio/tests/test_error_reporting.py`

 * *Files 16% similar despite different names*

```diff
@@ -164,7 +164,60 @@
     with pytest.raises(NoMatch) as e:
         parser.parse('   three ident')
     assert "Expected 'one' or 'two' at" in str(e.value)
 
     with pytest.raises(NoMatch) as e:
         parser.parse('   four ident')
     assert "Expected 'one' or 'two' at" in str(e.value)
+
+
+# HACK: Disabled just for this bugfix release as this require new handling of
+# infallibles
+def _test_not_succeed_in_ordered_choice():
+    """
+    Test that Not can succeed in ordered choice leading to ordered choice
+    to succeed.
+    See: https://github.com/textX/Arpeggio/issues/96
+    """
+
+    def grammar():
+        return [Not("a"), "a"], Optional("b")
+
+    parser = ParserPython(grammar)
+    parser.parse('b')
+
+
+def test_reporting_newline_symbols_when_not_matched():
+
+    # A case when a string match has newline
+    def grammar():
+        return "first", "\n"
+
+    parser = ParserPython(grammar, skipws=False)
+
+    with pytest.raises(NoMatch) as e:
+        _ = parser.parse('first')
+
+    assert "Expected '\\n' at position (1, 6)" in str(e.value)
+
+    # A case when regex match has newline
+    from arpeggio import RegExMatch
+    def grammar():
+        return "first", RegExMatch("\n")
+
+    parser = ParserPython(grammar, skipws=False)
+
+    with pytest.raises(NoMatch) as e:
+        _ = parser.parse('first')
+
+    assert "Expected '\\n' at position (1, 6)" in str(e.value)
+
+    # A case when the match is the root rule
+    def grammar():
+        return "root\nrule"
+
+    parser = ParserPython(grammar, skipws=False)
+
+    with pytest.raises(NoMatch) as e:
+        _ = parser.parse('something')
+
+    assert "Expected grammar at position (1, 1)" in str(e.value)
```

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_examples.py` & `Arpeggio-2.0.1/arpeggio/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_exporter.py` & `Arpeggio-2.0.1/arpeggio/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_flags.py` & `Arpeggio-2.0.1/arpeggio/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_parser_params.py` & `Arpeggio-2.0.1/arpeggio/tests/test_parser_params.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_parsing_expressions.py` & `Arpeggio-2.0.1/arpeggio/tests/test_parsing_expressions.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_pathologic_models.py` & `Arpeggio-2.0.1/arpeggio/tests/test_pathologic_models.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_peg_parser.py` & `Arpeggio-2.0.1/arpeggio/tests/test_peg_parser.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_position.py` & `Arpeggio-2.0.1/arpeggio/tests/test_position.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_ptnode_navigation_expressions.py` & `Arpeggio-2.0.1/arpeggio/tests/test_ptnode_navigation_expressions.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_python_parser.py` & `Arpeggio-2.0.1/arpeggio/tests/test_python_parser.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_reduce_tree.py` & `Arpeggio-2.0.1/arpeggio/tests/test_reduce_tree.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_semantic_action_results.py` & `Arpeggio-2.0.1/arpeggio/tests/test_semantic_action_results.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_separators.py` & `Arpeggio-2.0.1/arpeggio/tests/test_separators.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_sequence_params.py` & `Arpeggio-2.0.1/arpeggio/tests/test_sequence_params.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_suppression.py` & `Arpeggio-2.0.1/arpeggio/tests/test_suppression.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_unicode.py` & `Arpeggio-2.0.1/arpeggio/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/arpeggio/tests/test_visitor.py` & `Arpeggio-2.0.1/arpeggio/tests/test_visitor.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/art/arpeggio-logo.png` & `Arpeggio-2.0.1/art/arpeggio-logo.png`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/art/arpeggio-logo.svg` & `Arpeggio-2.0.1/art/arpeggio-logo.svg`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/about/license.md` & `Arpeggio-2.0.1/docs/about/license.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/configuration.md` & `Arpeggio-2.0.1/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/debugging.md` & `Arpeggio-2.0.1/docs/debugging.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/getting_started.md` & `Arpeggio-2.0.1/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/grammars.md` & `Arpeggio-2.0.1/docs/grammars.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/handling_errors.md` & `Arpeggio-2.0.1/docs/handling_errors.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/images/arpeggio-logo.svg` & `Arpeggio-2.0.1/docs/images/arpeggio-logo.svg`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/images/calc_parse_tree.dot.png` & `Arpeggio-2.0.1/docs/images/calc_parse_tree.dot.png`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/images/calc_parse_tree_reduced.dot.png` & `Arpeggio-2.0.1/docs/images/calc_parse_tree_reduced.dot.png`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/images/calc_parser_model.dot.png` & `Arpeggio-2.0.1/docs/images/calc_parser_model.dot.png`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/images/csvfile_parse_tree.dot.png` & `Arpeggio-2.0.1/docs/images/csvfile_parse_tree.dot.png`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/index.md` & `Arpeggio-2.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/js/version-select.js` & `Arpeggio-2.0.1/docs/js/version-select.js`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/parse_trees.md` & `Arpeggio-2.0.1/docs/parse_trees.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/semantics.md` & `Arpeggio-2.0.1/docs/semantics.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/troubleshooting.md` & `Arpeggio-2.0.1/docs/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/tutorials/bibtex.md` & `Arpeggio-2.0.1/docs/tutorials/bibtex.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/tutorials/calc.md` & `Arpeggio-2.0.1/docs/tutorials/calc.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/docs/tutorials/csv.md` & `Arpeggio-2.0.1/docs/tutorials/csv.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/README.md` & `Arpeggio-2.0.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/bibtex/README.md` & `Arpeggio-2.0.1/examples/bibtex/README.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/bibtex/bibtex.py` & `Arpeggio-2.0.1/examples/bibtex/bibtex.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/bibtex/bibtex_example.bib` & `Arpeggio-2.0.1/examples/bibtex/bibtex_example.bib`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/calc/README.md` & `Arpeggio-2.0.1/examples/calc/README.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/calc/calc.py` & `Arpeggio-2.0.1/examples/calc/calc.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/calc/calc_cleanpeg.py` & `Arpeggio-2.0.1/examples/calc/calc_cleanpeg.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/calc/calc_peg.py` & `Arpeggio-2.0.1/examples/calc/calc_peg.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/csv/README.md` & `Arpeggio-2.0.1/examples/csv/README.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/csv/csv.py` & `Arpeggio-2.0.1/examples/csv/csv.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/csv/csv_peg.py` & `Arpeggio-2.0.1/examples/csv/csv_peg.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/json/README.md` & `Arpeggio-2.0.1/examples/json/README.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/json/json.py` & `Arpeggio-2.0.1/examples/json/json.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/json/test.json` & `Arpeggio-2.0.1/examples/json/test.json`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/peg_peg/README.md` & `Arpeggio-2.0.1/examples/peg_peg/README.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/peg_peg/peg.peg` & `Arpeggio-2.0.1/examples/peg_peg/peg.peg`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/peg_peg/peg_peg.py` & `Arpeggio-2.0.1/examples/peg_peg/peg_peg.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/robot/README.md` & `Arpeggio-2.0.1/examples/robot/README.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/robot/robot.py` & `Arpeggio-2.0.1/examples/robot/robot.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/robot/robot_peg.py` & `Arpeggio-2.0.1/examples/robot/robot_peg.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/simple/README.md` & `Arpeggio-2.0.1/examples/simple/README.md`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/examples/simple/simple.py` & `Arpeggio-2.0.1/examples/simple/simple.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/mkdocs.yml` & `Arpeggio-2.0.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/perf-tests/grammar.py` & `Arpeggio-2.0.1/perf-tests/grammar.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/perf-tests/reports/_speed_report.txt` & `Arpeggio-2.0.1/perf-tests/reports/_speed_report.txt`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/perf-tests/reports/py2_memory_report_memoization.txt` & `Arpeggio-2.0.1/perf-tests/reports/py2_memory_report_memoization.txt`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/perf-tests/reports/py2_memory_report_nomemoization.txt` & `Arpeggio-2.0.1/perf-tests/reports/py2_memory_report_nomemoization.txt`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/perf-tests/reports/py2_speed_report.txt` & `Arpeggio-2.0.1/perf-tests/reports/py2_speed_report.txt`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/perf-tests/reports/py3_memory_report_memoization.txt` & `Arpeggio-2.0.1/perf-tests/reports/py3_memory_report_memoization.txt`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/perf-tests/reports/py3_memory_report_nomemoization.txt` & `Arpeggio-2.0.1/perf-tests/reports/py3_memory_report_nomemoization.txt`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/perf-tests/reports/py3_speed_report.txt` & `Arpeggio-2.0.1/perf-tests/reports/py3_speed_report.txt`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/perf-tests/test_inputs/LightSwitch.rpy` & `Arpeggio-2.0.1/perf-tests/test_inputs/LightSwitch.rpy`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/perf-tests/test_inputs/LightSwitchDouble.rpy` & `Arpeggio-2.0.1/perf-tests/test_inputs/LightSwitchDouble.rpy`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/perf-tests/test_memory_memoization.py` & `Arpeggio-2.0.1/perf-tests/test_memory_memoization.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/perf-tests/test_memory_nomemoization.py` & `Arpeggio-2.0.1/perf-tests/test_memory_nomemoization.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/perf-tests/test_speed.py` & `Arpeggio-2.0.1/perf-tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/setup.cfg` & `Arpeggio-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `Arpeggio-2.0.0/setup.py` & `Arpeggio-2.0.1/setup.py`

 * *Files identical despite different names*

